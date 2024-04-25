# Comparing `tmp/tinyrv-0.0.2.tar.gz` & `tmp/tinyrv-0.0.3.tar.gz`

## Comparing `tinyrv-0.0.2.tar` & `tinyrv-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,6 @@
--rw-r--r--   0        0        0    15845 2020-02-02 00:00:00.000000 tinyrv-0.0.2/tinyrv.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 tinyrv-0.0.2/riscv-opcodes/arg_lut.csv
--rw-r--r--   0        0        0     7855 2020-02-02 00:00:00.000000 tinyrv-0.0.2/riscv-opcodes/constants.py
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 tinyrv-0.0.2/riscv-opcodes/csrs.csv
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 tinyrv-0.0.2/riscv-opcodes/csrs32.csv
--rw-r--r--   0        0        0   236488 2020-02-02 00:00:00.000000 tinyrv-0.0.2/riscv-opcodes/instr_dict.yaml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 tinyrv-0.0.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tinyrv-0.0.2/LICENSE
--rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 tinyrv-0.0.2/README.md
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 tinyrv-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 tinyrv-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    16686 2020-02-02 00:00:00.000000 tinyrv-0.0.3/tinyrv.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 tinyrv-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tinyrv-0.0.3/LICENSE
+-rw-r--r--   0        0        0     7785 2020-02-02 00:00:00.000000 tinyrv-0.0.3/README.md
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 tinyrv-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 tinyrv-0.0.3/PKG-INFO
```

### Comparing `tinyrv-0.0.2/tinyrv.py` & `tinyrv-0.0.3/tinyrv.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import os, re, csv, struct, array, collections, struct, yaml, importlib.resources, pathlib
 
 try:
-    base = pathlib.Path('.') if pathlib.Path('riscv-opcodes').exists() else importlib.resources.files('tinyrv') / 'tinyrv'
-    opcodes = yaml.safe_load(open(base / 'riscv-opcodes/instr_dict.yaml'))
+    base = pathlib.Path('.') if pathlib.Path('tinyrv-opcodes').exists() else importlib.resources.files('tinyrv')
+    opcodes = yaml.safe_load(open(base / 'tinyrv-opcodes/instr_dict.yaml'))
     for aname, op in opcodes.items(): op['name'] = aname
     mask_match = [(int(op['mask'], 16), int(op['match'], 16), op) for op in opcodes.values()]
     def dr(h,l): return list(range(h,l-1,-1))
-    arg_bits = dict((a, dr(int(h),int(l))) for a, h, l in csv.reader(open(base / 'riscv-opcodes/arg_lut.csv'), skipinitialspace=True))
-    for s in open(base / 'riscv-opcodes/constants.py').readlines():  # immediate scrambling from latex_mapping. Some better way?
+    arg_bits = dict((a, dr(int(h),int(l))) for a, h, l in csv.reader(open(base / 'tinyrv-opcodes/arg_lut.csv'), skipinitialspace=True))
+    for s in open(base / 'tinyrv-opcodes/constants.py').readlines():  # immediate scrambling from latex_mapping. Some better way?
         if m := re.match(r"latex_mapping\[['\"](.*?)['\"]\] = ['\"][^\[]*\[([^\]]*)\]['\"]", s):
             fbits = sum([(dr(*(int(i) for i in part.split(':'))) if ':' in part else [int(part)]) for part in m[2].split('$\\\\vert$')], [])
             locs = [-1] * (max(fbits)+1)
             for i, b in enumerate(fbits): locs[-b-1] = arg_bits[m[1]][i]
             arg_bits[m[1]] = [31] * (32-len(locs)) + locs if locs[0] == 31 else locs  # sign extension
-    csrs = dict((int(a, 16), n) for fn in ['riscv-opcodes/csrs.csv', 'riscv-opcodes/csrs32.csv'] for a, n in csv.reader(open(base / fn), skipinitialspace=True))
+    csrs = dict((int(a, 16), n) for fn in ['tinyrv-opcodes/csrs.csv', 'tinyrv-opcodes/csrs32.csv'] for a, n in csv.reader(open(base / fn), skipinitialspace=True))
     csrs_addrs = dict((n, a) for a, n in csrs.items())
     iregs = 'zero,ra,sp,gp,tp,t0,t1,t2,fp,s1,a0,a1,a2,a3,a4,a5,a6,a7,s2,s3,s4,s5,s6,s7,s8,s9,s10,s11,t3,t4,t5,t6'.split(',')
-    fregs = 'ft0,ft1,ft2,ft3,ft4,ft5,ft6,ft7,fs0,fs1,fa0,fa1,fa2,fa3,fa4,fa5,fa6,fa7,fs2,fs3,fs4,fs5,fs6,fs7,fs8,fs9,fs10,fs11,ft8,ft9,ft10,ft11'.split(',')
     st = 'sb,sh,sw,sd'.split(','); ldst = 'lb,lh,lw,ld,lbu,lhu,lwu'.split(',') + st
     fence_flags = ',w,r,rw,o,ow,or,orw,i,iw,ir,irw,io,iow,ior,iorw'.split(',')
-    customs = {0b0001011: 'custom-0', 0b0101011: 'custom-1', 0b1011011: 'custom-2', 0b1111011: 'custom-3'}  # RISC-V spec ch. 34, table 70
+    customs = {0b0001011: 'custom0', 0b0101011: 'custom1', 0b1011011: 'custom2', 0b1111011: 'custom3'}  # RISC-V spec ch. 34, table 70
 except Exception as e: raise Exception("Unable to load RISC-V specs. Do:\n"
-                                       "git clone https://github.com/riscv/riscv-opcodes.git\n"
-                                       "cd riscv-opcodes; make")
+                                       "git clone https://github.com/riscv/riscv-opcodes.git tinyrv-opcodes\n"
+                                       "cd tinyrv-opcodes; make")
+
+def xfmt(d, xlen): return f'{{:0{xlen//4}x}}'.format(d&((1<<xlen)-1))
 
 class rvop:
     def __init__(self, **kwargs): [setattr(self, k, v) for k, v in kwargs.items()]
     def arg_str(self):
         args = [None]*4
         for k, v in self.args.items():  # hand-coded argument formats
             k = k.replace('c_','').replace('_n0','')
@@ -35,16 +36,16 @@
             elif self.name == 'fence' and k != 'fm': pass
             elif self.name.startswith('c.') or self.name.startswith('f'): args.append(f'{k}={v}')  # TODO: compressed and fp registers
             elif k == 'rd': args[0] = iregs[v]
             elif k == 'csr': args[1] = csrs.get(v, hex(v))
             elif k == 'rs1': args[2] = f"{self.args['imm12']}({iregs[v]})" if self.name in ldst + ['jalr'] else iregs[v]
             elif k == 'rs2': args[3] = iregs[v]
             elif k in ['imm12', 'zimm']: args.append(f'{v}' if self.name not in ldst + ['jalr'] else None)
-            elif k in ['jimm20', 'bimm12']: args.append(f'.{v:+d}')
-            elif k in ['imm20']: args.append(hex(v))
+            elif k in ['jimm20', 'bimm12']: args.append(xfmt(self.addr+v, 32))
+            elif k in ['imm20']: args.append(xfmt(v, 32))
             elif 'sham' in k: args.append(f'{v}')
             else: args.append(f'{k}={v}')  # fallback
         args = args[::-1] if self.name in st else args  # snowflake sb/sh/sw/sd arg order: <src>, <dst>
         return ', '.join([a for a in args if a is not None])
     def valid(self): return min([not('nz' in k or 'n0' in k) or v!=0 for k, v in self.args.items()] + [hasattr(self, 'extension')])
     def __repr__(self): return f'{self.name.replace("_","."):10} {self.arg_str()}'
 
@@ -73,119 +74,124 @@
                     if '_p' in vf: args[vf.replace('_p','')] = args[vf]+8  # reg aliases for some compressed instructions
                     if '_n0' in vf: args[vf.replace('_n0','')] = args[vf]
                 [setattr(o,k,v) for k,v in (op|args).items()]
                 o.args = dict(args)
                 break
         yield o
 
-def xfmt(d, xlen): return f'{{:0{xlen//4}x}}'.format(d&((1<<xlen)-1))
-
 def rvprint(*data, base=0, xlen=64):  # prints listing of decoded instructions.
-    for op in rvdecoder(*data, base=base): print(f'{xfmt(op.addr,xlen)}: {str(op):40} # {", ".join(op.extension) if op.valid() else "INVALID"}')
+    for op in rvdecoder(*data, base=base): print(f'{xfmt(op.addr,32)}: {str(op):40} # {", ".join(op.extension) if op.valid() else "INVALID"}')
 
 class rvmem:
     def __init__(self, xlen=64):
         self.psize, self.pages, self.xlen = 2<<12, {}, xlen
         self.fmt_sizes = {'q': 8, 'Q': 8, 'i': 4, 'I': 4, 'h': 2, 'H': 2, 'b': 1, 'B': 1}
         self.trace = []
-    def load(self, file, base=0): [self.s(i+base, b, 'B') for i, b in enumerate(open(file, 'rb').read())]
+    def read(self, file, base=0): [self.store(i+base, b, 'B') for i, b in enumerate(open(file, 'rb').read())]
     def _page_pa(self, addr):
         pb, pa = addr&~(self.psize-1), addr&(self.psize-1)
         if pb not in self.pages: self.pages[pb] = bytearray(self.psize)
         return self.pages[pb], pa
-    def s(self, addr, data, fmt=None):
+    def store(self, addr, data, fmt=None):
         page, pa = self._page_pa(addr)
         fmt = fmt or ('i' if self.xlen==32 else 'q')
         page[pa:pa+self.fmt_sizes[fmt]] = struct.pack(fmt, data)
         self.trace.append(f'mem[{xfmt(addr, self.xlen)}] <- {xfmt(data, self.fmt_sizes[fmt]*8)}')
-    def l(self, addr, fmt=None):
+    def load(self, addr, fmt=None):
         page, pa = self._page_pa(addr)
         fmt = fmt or ('i' if self.xlen==32 else 'q')
         data = struct.unpack(fmt, page[pa:pa+self.fmt_sizes[fmt]])[0]
         self.trace.append(f'mem[{xfmt(addr, self.xlen)}] -> {xfmt(data, self.fmt_sizes[fmt]*8)}')
         return data
 
 class rvregs:  # normal list, but ignore writes to x[0]
     def __init__(self): self._x = [0]*32
     def __getitem__(self, i): return self._x[i]
     def __setitem__(self, i, d): self._x[i] = d if i else 0
 
-class rvsim:  # simulates RV32I, RV64I and some additional instructions
+class rvsim:  # simulates RV32IZicsr_Zifencei, RV64IZicsr_Zifencei and some additional instructions
     def __init__(self, mem, xlen=64):
         self.mem, self.xlen = mem, xlen
         self.pc, self.x, self.f, self.csr = 0, rvregs(), [0]*32, [0]*4096
         self.xlenmask = (1<<self.xlen)-1
-        self.u32mask = (1<<32)-1
         [setattr(self, n, i) for i, n in enumerate(iregs)]
         [setattr(self, n, a) for a, n in csrs.items()]
     def __repr__(self): return '\n'.join(['  '.join([f'x{r+rr:02d}({(iregs[r+rr])[-2:]})={xfmt(self.x[r+rr], self.xlen)}' for r in range(0, 32, 8)]) for rr in range(8)])
+    def addop(self, _opfn): setattr(self, _opfn.__name__, _opfn.__get__(self, rvsim))
     def sext(self,v,l=None): l = l or self.xlen; return v|~((1<<l)-1) if v&(1<<(l-1)) else v&((1<<l)-1)
-    def newop(self, _opfn):
-        setattr(self, _opfn.__name__, _opfn.__get__(self, rvsim))
+    def checked_store(self, addr, rs2, fmt, mask, alignmask):
+        if addr&alignmask == 0: self.mem.store(addr&self.xlenmask, self.x[rs2]&mask, fmt); self.pc += 4
+        else: self.csr[self.mtval], self.csr[self.mepc], self.csr[self.mcause], self.pc = addr&self.xlenmask, self.pc, 6, self.csr[self.mtvec] & (~3) & self.xlenmask
+    def checked_load (self, rd, addr, fmt, alignmask):
+        if addr&alignmask == 0: self.x[rd] = self.mem.load(addr&self.xlenmask, fmt); self.pc += 4
+        else: self.csr[self.mtval], self.csr[self.mepc], self.csr[self.mcause], self.pc = addr&self.xlenmask, self.pc, 4, self.csr[self.mtvec] & (~3) & self.xlenmask
     def _auipc (self, rd, imm20,  **_): self.x[rd] = self.sext(self.pc+imm20); self.pc+=4
     def _lui   (self, rd, imm20,  **_): self.x[rd] = imm20; self.pc+=4
     def _jal   (self, rd, jimm20, **_): self.x[rd] = self.pc+4; self.pc = (self.pc+jimm20)&self.xlenmask
-    def _jalr  (self, rd, rs1, imm12, **_): self.x[rd], self.pc = self.pc+4, (self.x[rs1]+imm12)&self.xlenmask
+    def _jalr  (self, rd, rs1, imm12, **_): self.x[rd], self.pc = self.pc+4, (self.x[rs1]+imm12)&self.xlenmask&(-2)  # LSB=0
     def _beq   (self, rs1, rs2, bimm12, **_): self.pc = (self.pc+bimm12) if self.x[rs1] == self.x[rs2] else self.pc+4
     def _bne   (self, rs1, rs2, bimm12, **_): self.pc = (self.pc+bimm12) if self.x[rs1] != self.x[rs2] else self.pc+4
     def _blt   (self, rs1, rs2, bimm12, **_): self.pc = (self.pc+bimm12) if self.x[rs1] < self.x[rs2] else self.pc+4
     def _bge   (self, rs1, rs2, bimm12, **_): self.pc = (self.pc+bimm12) if self.x[rs1] >= self.x[rs2] else self.pc+4
     def _bltu  (self, rs1, rs2, bimm12, **_): self.pc = (self.pc+bimm12) if self.x[rs1]&self.xlenmask < self.x[rs2]&self.xlenmask else self.pc+4
     def _bgeu  (self, rs1, rs2, bimm12, **_): self.pc = (self.pc+bimm12) if self.x[rs1]&self.xlenmask >= self.x[rs2]&self.xlenmask else self.pc+4
-    def _sb    (self, rs1, rs2, imm12, **_): self.mem.s((self.x[rs1]+imm12)&self.xlenmask, self.x[rs2]&((1<<8)-1), 'B'); self.pc+=4
-    def _sh    (self, rs1, rs2, imm12, **_): self.mem.s((self.x[rs1]+imm12)&self.xlenmask, self.x[rs2]&((1<<16)-1), 'H'); self.pc+=4
-    def _sw    (self, rs1, rs2, imm12, **_): self.mem.s((self.x[rs1]+imm12)&self.xlenmask, self.x[rs2]&((1<<32)-1), 'I'); self.pc+=4
-    def _sd    (self, rs1, rs2, imm12, **_): self.mem.s((self.x[rs1]+imm12)&self.xlenmask, self.x[rs2]&((1<<64)-1), 'Q'); self.pc+=4
-    def _lb    (self, rd, rs1, imm12,  **_): self.x[rd] = self.mem.l((self.x[rs1]+imm12)&self.xlenmask, 'b'); self.pc+=4
-    def _lh    (self, rd, rs1, imm12,  **_): self.x[rd] = self.mem.l((self.x[rs1]+imm12)&self.xlenmask, 'h'); self.pc+=4
-    def _lw    (self, rd, rs1, imm12,  **_): self.x[rd] = self.mem.l((self.x[rs1]+imm12)&self.xlenmask, 'i'); self.pc+=4
-    def _ld    (self, rd, rs1, imm12,  **_): self.x[rd] = self.mem.l((self.x[rs1]+imm12)&self.xlenmask, 'q'); self.pc+=4
-    def _lbu   (self, rd, rs1, imm12,  **_): self.x[rd] = self.mem.l((self.x[rs1]+imm12)&self.xlenmask, 'B'); self.pc+=4
-    def _lhu   (self, rd, rs1, imm12,  **_): self.x[rd] = self.mem.l((self.x[rs1]+imm12)&self.xlenmask, 'H'); self.pc+=4
-    def _lwu   (self, rd, rs1, imm12,  **_): self.x[rd] = self.mem.l((self.x[rs1]+imm12)&self.xlenmask, 'I'); self.pc+=4
+    def _sb    (self, rs1, rs2, imm12, **_): self.mem.store((self.x[rs1]+imm12)&self.xlenmask, self.x[rs2]&((1<<8)-1), 'B'); self.pc+=4
+    def _sh    (self, rs1, rs2, imm12, **_): self.checked_store((self.x[rs1]+imm12)&self.xlenmask, rs2, 'H', (1<<16)-1, 1)
+    def _sw    (self, rs1, rs2, imm12, **_): self.checked_store((self.x[rs1]+imm12)&self.xlenmask, rs2, 'I', (1<<32)-1, 3)
+    def _sd    (self, rs1, rs2, imm12, **_): self.checked_store((self.x[rs1]+imm12)&self.xlenmask, rs2, 'Q', (1<<64)-1, 7)
+    def _lb    (self, rd, rs1, imm12,  **_): self.x[rd] = self.mem.load((self.x[rs1]+imm12)&self.xlenmask, 'b'); self.pc+=4
+    def _lh    (self, rd, rs1, imm12,  **_): self.checked_load(rd, self.x[rs1]+imm12, 'h', 1)
+    def _lw    (self, rd, rs1, imm12,  **_): self.checked_load(rd, self.x[rs1]+imm12, 'i', 3)
+    def _ld    (self, rd, rs1, imm12,  **_): self.checked_load(rd, self.x[rs1]+imm12, 'q', 7)
+    def _lbu   (self, rd, rs1, imm12,  **_): self.x[rd] = self.mem.load((self.x[rs1]+imm12)&self.xlenmask, 'B'); self.pc+=4
+    def _lhu   (self, rd, rs1, imm12,  **_): self.checked_load(rd, self.x[rs1]+imm12, 'H', 1)
+    def _lwu   (self, rd, rs1, imm12,  **_): self.checked_load(rd, self.x[rs1]+imm12, 'I', 3)
     def _addi  (self, rd, rs1, imm12,  **_): self.x[rd] = self.sext(self.x[rs1] + imm12); self.pc+=4
     def _slti  (self, rd, rs1, imm12,  **_): self.x[rd] = self.x[rs1] < imm12; self.pc+=4
     def _sltiu (self, rd, rs1, imm12,  **_): self.x[rd] = (self.x[rs1]&self.xlenmask) < (self.sext(imm12, 32)&self.xlenmask); self.pc+=4
     def _xori  (self, rd, rs1, imm12,  **_): self.x[rd] = self.sext(self.x[rs1] ^ imm12); self.pc+=4
     def _ori   (self, rd, rs1, imm12,  **_): self.x[rd] = self.sext(self.x[rs1] | imm12); self.pc+=4
     def _andi  (self, rd, rs1, imm12,  **_): self.x[rd] = self.sext(self.x[rs1] & imm12); self.pc+=4
     def _slli  (self, rd, rs1, shamtd, **_): self.x[rd] = self.sext(self.x[rs1] << shamtd); self.pc+=4  # shared with RV64I
     def _srli  (self, rd, rs1, shamtd, **_): self.x[rd] = self.sext((self.x[rs1]&self.xlenmask) >> shamtd); self.pc+=4  # shared with RV64I
     def _srai  (self, rd, rs1, shamtd, **_): self.x[rd] = self.sext(self.x[rs1] >> shamtd); self.pc+=4  # shared with RV64I
     def _add   (self, rd, rs1, rs2,    **_): self.x[rd] = self.sext(self.x[rs1] + self.x[rs2]); self.pc+=4
     def _sub   (self, rd, rs1, rs2,    **_): self.x[rd] = self.sext(self.x[rs1] - self.x[rs2]); self.pc+=4
-    def _sll   (self, rd, rs1, rs2,    **_): self.x[rd] = self.sext(self.x[rs1] << (self.x[rs2]&63)); self.pc+=4
+    def _sll   (self, rd, rs1, rs2,    **_): self.x[rd] = self.sext(self.x[rs1] << (self.x[rs2]&(self.xlen-1))); self.pc+=4
     def _slt   (self, rd, rs1, rs2,    **_): self.x[rd] = self.x[rs1] < self.x[rs2]; self.pc+=4
     def _sltu  (self, rd, rs1, rs2,    **_): self.x[rd] = (self.x[rs1]&self.xlenmask) < (self.x[rs2]&self.xlenmask); self.pc+=4
     def _xor   (self, rd, rs1, rs2,    **_): self.x[rd] = self.sext(self.x[rs1] ^ self.x[rs2]); self.pc+=4
-    def _srl   (self, rd, rs1, rs2,    **_): self.x[rd] = self.sext((self.x[rs1]&self.xlenmask) >> (self.x[rs2]&63)); self.pc+=4
-    def _sra   (self, rd, rs1, rs2,    **_): self.x[rd] = self.sext(self.x[rs1] >> (self.x[rs2]&63)); self.pc+=4
+    def _srl   (self, rd, rs1, rs2,    **_): self.x[rd] = self.sext((self.x[rs1]&self.xlenmask) >> (self.x[rs2]&(self.xlen-1))); self.pc+=4
+    def _sra   (self, rd, rs1, rs2,    **_): self.x[rd] = self.sext(self.x[rs1] >> (self.x[rs2]&(self.xlen-1))); self.pc+=4
     def _or    (self, rd, rs1, rs2,    **_): self.x[rd] = self.sext(self.x[rs1] | self.x[rs2]); self.pc+=4
     def _and   (self, rd, rs1, rs2,    **_): self.x[rd] = self.sext(self.x[rs1] & self.x[rs2]); self.pc+=4  # mostly RV32I until here
     def _addiw (self, rd, rs1, imm12,  **_): self.x[rd] = self.sext(self.x[rs1] + imm12, 32); self.pc+=4  # RV64I from here
     def _slliw (self, rd, rs1, shamtw, **_): self.x[rd] = self.sext(self.x[rs1] << shamtw, 32); self.pc+=4
-    def _srliw (self, rd, rs1, shamtw, **_): self.x[rd] = self.sext((self.x[rs1]&self.u32mask) >> shamtw, 32); self.pc+=4
+    def _srliw (self, rd, rs1, shamtw, **_): self.x[rd] = self.sext((self.x[rs1]&((1<<32)-1)) >> shamtw, 32); self.pc+=4
     def _sraiw (self, rd, rs1, shamtw, **_): self.x[rd] = self.sext(self.sext(self.x[rs1], 32) >> shamtw, 32); self.pc+=4
     def _addw  (self, rd, rs1, rs2,    **_): self.x[rd] = self.sext(self.sext(self.x[rs1], 32) + self.sext(self.x[rs2], 32), 32); self.pc+=4
     def _subw  (self, rd, rs1, rs2,    **_): self.x[rd] = self.sext(self.sext(self.x[rs1], 32) - self.sext(self.x[rs2], 32), 32); self.pc+=4
     def _sllw  (self, rd, rs1, rs2,    **_): self.x[rd] = self.sext(self.sext(self.x[rs1], 32) << (self.x[rs2]&31), 32); self.pc+=4
-    def _srlw  (self, rd, rs1, rs2,    **_): self.x[rd] = self.sext((self.x[rs1]&self.u32mask) >> (self.x[rs2]&31), 32); self.pc+=4
+    def _srlw  (self, rd, rs1, rs2,    **_): self.x[rd] = self.sext((self.x[rs1]&((1<<32)-1)) >> (self.x[rs2]&31), 32); self.pc+=4
     def _sraw  (self, rd, rs1, rs2,    **_): self.x[rd] = self.sext(self.sext(self.x[rs1], 32) >> (self.x[rs2]&31), 32); self.pc+=4
     def _mul   (self, rd, rs1, rs2,    **_): self.x[rd] = self.sext(self.x[rs1] * self.x[rs2]); self.pc+=4  # RV32M
     def _mulw  (self, rd, rs1, rs2,    **_): self.x[rd] = self.sext(self.sext(self.x[rs1], 32) * self.sext(self.x[rs2], 32), 32); self.pc+=4  # RV64M
     def _fence (self,                  **_): self.pc+=4
+    def _fence_i(self,                 **_): self.pc+=4
     def _csrrwi(self, rd, csr, zimm,   **_): self.x[rd], self.csr[csr] = self.csr[csr], zimm if (csr&0xc00)!=0xc00 else self.csr[csr]; self.pc+=4
     def _csrrs (self, rd, csr, rs1,    **_): self.x[rd], self.csr[csr] = self.csr[csr], (self.csr[csr]|self.x[rs1]) if (csr&0xc00)!=0xc00 else self.csr[csr]; self.pc+=4
     def _csrrc (self, rd, csr, rs1,    **_): self.x[rd], self.csr[csr] = self.csr[csr], (self.csr[csr]&~self.x[rs1]) if (csr&0xc00)!=0xc00 else self.csr[csr]; self.pc+=4
     def _csrrw (self, rd, csr, rs1,    **_): self.x[rd], self.csr[csr] = self.csr[csr], self.x[rs1] if (csr&0xc00)!=0xc00 else self.csr[csr]; self.pc+=4
-    def _mret  (self,                  **_): self.pc = self.csr[csrs_addrs['mepc']]
+    def _mret  (self,                  **_): self.pc = self.csr[self.mepc] & self.xlenmask
+    def _ecall (self,                  **_):                                 self.csr[self.mepc] = self.pc; self.csr[self.mcause] = 11; self.pc = self.csr[self.mtvec] & (~3) & self.xlenmask
+    def _ebreak(self,                  **_): self.csr[self.mtval] = self.pc; self.csr[self.mepc] = self.pc; self.csr[self.mcause] = 3;  self.pc = self.csr[self.mtvec] & (~3) & self.xlenmask
+    def _c_addi(self, rd_rs1, nzimm6,  **_): self.x[rd_rs1] += nzimm6; self.pc+=2  # needed for c.nop in test rv32i_m/privilege/src/misalign-jal-01.S
     def step(self, steps=1, bpts=set()):
         for _ in range(steps):
-            self.op = next(rvdecoder(self.mem.l(self.pc, 'I'), base=self.pc))
+            self.op = next(rvdecoder(self.mem.load(self.pc, 'I'), base=self.pc))
             self.mem.trace = []
-            if hasattr(self, '_'+self.op.name): getattr(self, '_'+self.op.name)(**self.op.args)
+            if hasattr(self, '_'+self.op.name): getattr(self, '_'+self.op.name)(**self.op.args)  # dispatch instruction
             else: print(f'{xfmt(self.op.addr, self.xlen)}: {str(self.op):40} # {self.op.extension if self.op.valid() else "UNKNOWN"}  # halted: unimplemented op'); break
-            fp = (self.op.name.startswith('f') or self.op.name.startswith('c.f')) and not self.op.name.startswith('fence')
-            rdinfo = f'{fregs[self.op.rd] if fp else iregs[self.op.rd]} = {xfmt(self.f[self.op.rd] if fp else self.x[self.op.rd], self.xlen)}' if 'rd' in self.op.args and self.op.rd != 0 else ''
+            rdinfo = f'{iregs[self.op.rd]} = {xfmt(self.x[self.op.rd], self.xlen)}' if 'rd' in self.op.args and self.op.rd != 0 else ''
             print(f'{xfmt(self.op.addr, self.xlen)}: {str(self.op):40} # {rdinfo}', ' '.join(self.mem.trace))
             if self.pc-self.op.addr not in (2, 4): print()
             if self.op.addr in bpts|{self.pc}: break
```

### Comparing `tinyrv-0.0.2/LICENSE` & `tinyrv-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyrv-0.0.2/PKG-INFO` & `tinyrv-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,41 @@
-Metadata-Version: 2.3
-Name: tinyrv
-Version: 0.0.2
-Summary: A tiny RISC-V instruction decoder and emulator
-Project-URL: Homepage, https://github.com/s-holst/tinyrv
-Project-URL: Issues, https://github.com/s-holst/tinyrv/issues
-Author-email: Stefan Holst <mail@s-holst.de>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # tinyRV
 
-A RISC-V instruction decoder and emulator in less than 200 lines of pure python3.
+A RISC-V instruction decoder and instruction set simulator in less than 200 lines of python.
 
 - Uses official RISC-V specs to decode *every* specified RISC-V instruction.
-- Emulates at least the base ISAs RV32I/RV64I and is easily extendable.
+- Emulates at least the base ISAs and is easily extendable.
+- RV32IZicsr_Zifencei and RV64IZicsr_Zifencei compliance validated using RISCOF (see Testing below).
 
 ## Getting Started
 
 ```sh
 pip install tinyrv
 ```
 
 Print all RISC-V instructions in a binary:
 ```py
 from tinyrv import rvprint
 rvprint('firmware.bin', xlen=32)  # xlen just for output formatting
 ```
 Outputs for `firmware.bin` from [picorv32](https://github.com/YosysHQ/picorv32/tree/main):
 ```
-00000000: custom-0   raw=0x0800400b                # INVALID
-00000004: custom-0   raw=0x0600600b                # INVALID
-00000008: jal        zero, .+984                   # rv_i
+00000000: custom0    raw=0x0800400b                # INVALID
+00000004: custom0    raw=0x0600600b                # INVALID
+00000008: jal        zero, 000003e0                # rv_i
 0000000c: addi       zero, zero, 0                 # rv_i
-00000010: custom-0   raw=0x0200a10b                # INVALID
-00000014: custom-0   raw=0x0201218b                # INVALID
-00000018: lui        ra, 0x0                       # rv_i
+00000010: custom0    raw=0x0200a10b                # INVALID
+00000014: custom0    raw=0x0201218b                # INVALID
+00000018: lui        ra, 00000000                  # rv_i
 0000001c: addi       ra, ra, 352                   # rv_i
-00000020: custom-0   raw=0x0000410b                # INVALID
+00000020: custom0    raw=0x0000410b                # INVALID
 00000024: sw         sp, 0(ra)                     # rv_i
-00000028: custom-0   raw=0x0001410b                # INVALID
+00000028: custom0    raw=0x0001410b                # INVALID
 0000002c: sw         sp, 4(ra)                     # rv_i
-00000030: custom-0   raw=0x0001c10b                # INVALID
+00000030: custom0    raw=0x0001c10b                # INVALID
 00000034: sw         sp, 8(ra)                     # rv_i
 00000038: sw         gp, 12(ra)                    # rv_i
 0000003c: sw         tp, 16(ra)                    # rv_i
 ...
 ```
 picorv32 uses some custom instructions for IRQ handling.
 
@@ -96,15 +83,15 @@
 x04(tp)=00000000  x12(a2)=00000000  x20(s4)=00000000  x28(t3)=00000000
 x05(t0)=00000000  x13(a3)=00000000  x21(s5)=00000000  x29(t4)=00000000
 x06(t1)=00000000  x14(a4)=00000000  x22(s6)=00000000  x30(t5)=00000000
 x07(t2)=00000000  x15(a5)=00000000  x23(s7)=00000000  x31(t6)=00000000
 
 00000000: custom-0   raw=0x0800400b                # UNKNOWN  # halted: unimplemented op
 ```
-Simulation steps at the first instruction that is not implemented. Just set the pc and carry on:
+Simulation halts at the first instruction that is not implemented. Just set the pc and carry on:
 ```py
 rv.pc = 8
 rv.step(50)
 ```
 ```
 00000008: jal        zero, .+984                   #  
 
@@ -155,16 +142,64 @@
 ## Dev Setup
 
 All code is in `tinyrv.py`.
 No dependencies, except [pyyaml](https://pypi.org/project/PyYAML/).
 However, tinyRV needs to load opcode specs from [riscv-opcodes](https://github.com/riscv/riscv-opcodes).
 Do this:
 ```sh
-git clone https://github.com/riscv/riscv-opcodes.git
-cd riscv-opcodes; make
+git clone https://github.com/riscv/riscv-opcodes.git tinyrv-opcodes
+cd tinyrv-opcodes; make
+```
+The necessary opcode specs are also bundled in the PyPI package. If there is a `tinyrv-opcodes` in the current directory, tinyRV will try to use those instead of the packaged ones.
+
+## Testing
+
+Need python (duh!) and [riscv-gnu-toolchain](https://github.com/riscv/riscv-gnu-toolchain). Tested on MacOS.
+
+Install [the RISC-V compatibility framework RISCOF](https://github.com/riscv-software-src/riscof):
+```sh
+pip3 install setuptools wheel
+git clone https://github.com/riscv/riscof.git
+cd riscof
+pip3 install -e .
+```
+
+Install the [Sail ISA specification language](https://github.com/rems-project/sail):
+```sh
+brew install opam zlib z3 pkg-config
+opam init
+opam switch create ocaml-base-compiler
+opam install sail
+eval $(opam config env)
+```
+
+Install the [RISCV Sail Model](https://github.com/riscv/sail-riscv):
+```sh
+git clone https://github.com/riscv/sail-riscv.git
+cd sail-riscv
+ARCH=RV32 make c_emulator/riscv_sim_RV32
+ARCH=RV64 make c_emulator/riscv_sim_RV64
+# copy / link c_emulator/riscv_sim_RV{32,64} into $PATH location
+```
+
+Optionally, install [Spike RISC-V ISA Simulator](https://github.com/riscv-software-src/riscv-isa-sim):
+```sh
+git clone https://github.com/riscv-software-src/riscv-isa-sim.git
+cd riscv-isa-sim
+mkdir build
+cd build
+../configure --prefix=/path/to/install  # /path/to/install/bin must be in $PATH
+make
+make install
+spike  # test
+```
+Then, run the tests:
+```sh
+cd tests
+riscof --verbose info arch-test --clone
+riscof run --config=config.ini --suite=riscv-arch-test/riscv-test-suite/ --env=riscv-arch-test/riscv-test-suite/env
 ```
-The necessary opcode specs are also bundled in the PyPI package. If there is a `riscv-opcodes` in the current directory, tinyRV will try to use those instead of the packaged ones.
 
 ## Related
 
 - [TinyFive](https://github.com/OpenMachine-ai/tinyfive)
 - [mini-rv32ima](https://github.com/cnlohr/mini-rv32ima)
```

