# Comparing `tmp/PyCatFile-0.7.8.tar.gz` & `tmp/pycatfile-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCatFile-0.7.8.tar", last modified: Sat Apr 13 01:28:31 2024, max compression
+gzip compressed data, was "pycatfile-0.8.2.tar", last modified: Thu Apr 25 00:13:58 2024, max compression
```

## Comparing `PyCatFile-0.7.8.tar` & `pycatfile-0.8.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:28:31.939092 PyCatFile-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-13 01:28:23.000000 PyCatFile-0.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-13 01:28:31.939092 PyCatFile-0.7.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:28:31.939092 PyCatFile-0.7.8/PyCatFile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-13 01:28:31.000000 PyCatFile-0.7.8/PyCatFile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-13 01:28:31.000000 PyCatFile-0.7.8/PyCatFile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 01:28:31.000000 PyCatFile-0.7.8/PyCatFile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-13 01:28:31.000000 PyCatFile-0.7.8/PyCatFile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 01:28:31.000000 PyCatFile-0.7.8/PyCatFile.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-13 01:28:23.000000 PyCatFile-0.7.8/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     7310 2024-04-13 01:28:23.000000 PyCatFile-0.7.8/catfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4969 2024-04-13 01:28:23.000000 PyCatFile-0.7.8/neocatfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   322887 2024-04-13 01:28:23.000000 PyCatFile-0.7.8/pycatfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-13 01:28:31.939092 PyCatFile-0.7.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     5451 2024-04-13 01:28:23.000000 PyCatFile-0.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:13:58.785832 pycatfile-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-25 00:13:50.000000 pycatfile-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-25 00:13:58.785832 pycatfile-0.8.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:13:58.785832 pycatfile-0.8.2/PyCatFile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-25 00:13:58.000000 pycatfile-0.8.2/PyCatFile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-25 00:13:58.000000 pycatfile-0.8.2/PyCatFile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 00:13:58.000000 pycatfile-0.8.2/PyCatFile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 00:13:58.000000 pycatfile-0.8.2/PyCatFile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 00:13:58.000000 pycatfile-0.8.2/PyCatFile.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-25 00:13:50.000000 pycatfile-0.8.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7289 2024-04-25 00:13:50.000000 pycatfile-0.8.2/catfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4969 2024-04-25 00:13:50.000000 pycatfile-0.8.2/neocatfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   356309 2024-04-25 00:13:50.000000 pycatfile-0.8.2/pycatfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-25 00:13:58.785832 pycatfile-0.8.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5451 2024-04-25 00:13:50.000000 pycatfile-0.8.2/setup.py
```

### Comparing `PyCatFile-0.7.8/LICENSE` & `pycatfile-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCatFile-0.7.8/PKG-INFO` & `pycatfile-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCatFile
-Version: 0.7.8
+Version: 0.8.2
 Summary: A tar like file format name catfile after unix cat command (concatenate files) .
 Home-page: https://github.com/GameMaker2k/PyCatFile
 Download-URL: https://github.com/GameMaker2k/PyCatFile/archive/master.tar.gz
 Author: Kazuki Przyborowski
 Author-email: kazuki.przyborowski@gmail.com
 Maintainer: Kazuki Przyborowski
 Maintainer-email: kazuki.przyborowski@gmail.com
```

### Comparing `PyCatFile-0.7.8/PyCatFile.egg-info/PKG-INFO` & `pycatfile-0.8.2/PyCatFile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCatFile
-Version: 0.7.8
+Version: 0.8.2
 Summary: A tar like file format name catfile after unix cat command (concatenate files) .
 Home-page: https://github.com/GameMaker2k/PyCatFile
 Download-URL: https://github.com/GameMaker2k/PyCatFile/archive/master.tar.gz
 Author: Kazuki Przyborowski
 Author-email: kazuki.przyborowski@gmail.com
 Maintainer: Kazuki Przyborowski
 Maintainer-email: kazuki.przyborowski@gmail.com
```

### Comparing `PyCatFile-0.7.8/catfile.py` & `pycatfile-0.8.2/catfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: catfile.py - Last Update: 4/12/2024 Ver. 0.7.8 RC 1 - Author: cooldude2k $
+    $FileInfo: catfile.py - Last Update: 4/24/2024 Ver. 0.8.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import argparse, pycatfile, binascii;
 
 rarfile_support = pycatfile.rarfile_support;
 
@@ -66,19 +66,18 @@
 getargs = argparser.parse_args()
 
 fname = getargs.format;
 fnamelower = fname.lower();
 fnamemagic = fname;
 fnamelen = len(fname);
 fnamehex = binascii.hexlify(fname.encode("UTF-8")).decode("UTF-8");
-fnamever = getargs.formatver;
 fnamesty = __use_new_style__;
 fnamelst = __use_advanced_list__;
 fnameino = __use_alt_inode__;
-fnamelist = [fname, fnamemagic, fnamelower, fnamelen, fnamehex, getargs.delimiter, fnamever, fnamesty, fnamelst, fnameino];
+fnamelist = [fname, fnamemagic, fnamelower, fnamelen, fnamehex, getargs.delimiter, getargs.formatver, fnamesty, fnamelst, fnameino];
 
 # Determine actions based on user input
 should_create = getargs.create and not getargs.extract and not getargs.list;
 should_extract = getargs.extract and not getargs.create and not getargs.list;
 should_list = getargs.list and not getargs.create and not getargs.extract;
 should_repack = getargs.create and getargs.repack;
 should_validate = getargs.validate;
```

### Comparing `PyCatFile-0.7.8/neocatfile.py` & `pycatfile-0.8.2/neocatfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: neocatfile.py - Last Update: 4/12/2024 Ver. 0.7.8 RC 1 - Author: cooldude2k $
+    $FileInfo: neocatfile.py - Last Update: 4/24/2024 Ver. 0.8.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 import argparse
 import pycatfile
 
 # Compatibility layer for Python 2 and 3 input
```

### Comparing `PyCatFile-0.7.8/pycatfile.py` & `pycatfile-0.8.2/pycatfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: pycatfile.py - Last Update: 4/12/2024 Ver. 0.7.8 RC 1 - Author: cooldude2k $
+    $FileInfo: pycatfile.py - Last Update: 4/24/2024 Ver. 0.8.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import io, os, re, sys, time, stat, zlib, base64, shutil, socket, hashlib, datetime, logging, binascii, tempfile, zipfile, platform;
 from ftplib import FTP, FTP_TLS;
 if(sys.version[0]=="2"):
  from urlparse import urlparse, urlunparse;
@@ -60,14 +60,21 @@
 rarfile_support = False;
 try:
  import rarfile;
  rarfile_support = True;
 except ImportError:
  rarfile_support = False;
 
+py7zr_support = False;
+try:
+ import py7zr;
+ py7zr_support = True;
+except ImportError:
+ py7zr_support = False;
+
 try:
  from safetar import is_tarfile;
 except ImportError:
  try:
   from xtarfile import is_tarfile;
  except ImportError:
   from tarfile import is_tarfile;
@@ -160,19 +167,19 @@
 __file_format_ver__ = "001";
 __use_new_style__ = True;
 __use_advanced_list__ = True;
 __use_alt_inode__ = False;
 __file_format_list__ = [__file_format_name__, __file_format_magic__, __file_format_lower__, __file_format_len__, __file_format_hex__, __file_format_delimiter__, __file_format_ver__, __use_new_style__, __use_advanced_list__, __use_alt_inode__];
 __project__ = __program_name__;
 __project_url__ = "https://github.com/GameMaker2k/PyCatFile";
-__version_info__ = (0, 7, 8, "RC 1", 1);
-__version_date_info__ = (2024, 4, 12, "RC 1", 1);
+__version_info__ = (0, 8, 2, "RC 1", 1);
+__version_date_info__ = (2024, 4, 24, "RC 1", 1);
 __version_date__ = str(__version_date_info__[0]) + "." + str(__version_date_info__[1]).zfill(2) + "." + str(__version_date_info__[2]).zfill(2);
 __revision__ = __version_info__[3];
-__revision_id__ = "$Id: 08fb47c714ff74769abf5a6def7842a572a87a9a $";
+__revision_id__ = "$Id: d755dda2624960ee460c73d9a2e0b0394df919e5 $";
 if(__version_info__[4] is not None):
  __version_date_plusrc__ = __version_date__ + "-" + str(__version_date_info__[4]);
 if(__version_info__[4] is None):
  __version_date_plusrc__ = __version_date__;
 if(__version_info__[3] is not None):
  __version__ = str(__version_info__[0]) + "." + str(__version_info__[1]) + "." + str(__version_info__[2]) + " " + str(__version_info__[3]);
 if(__version_info__[3] is None):
@@ -1679,14 +1686,16 @@
  prefp = catfp.read(5);
  if(prefp==binascii.unhexlify("7573746172")):
   filetype = "tarfile";
  catfp.seek(0, 0);
  prefp = catfp.read(6);
  if(prefp==binascii.unhexlify("fd377a585a00")):
   filetype = "lzma";
+ if(prefp==binascii.unhexlify("377abcaf271c")):
+  filetype = "7zipfile";
  catfp.seek(0, 0);
  prefp = catfp.read(7);
  if(prefp==binascii.unhexlify("526172211a0700")):
   filetype = "rarfile";
  if(prefp==binascii.unhexlify("43617446696c65")):
   filetype = "catfile";
  catfp.seek(0, 0);
@@ -1952,14 +1961,18 @@
   return "catfile";
  if(compresscheck==formatspecs[2]):
   return formatspecs[2];
  if(compresscheck=="tarfile"):
   return "tarfile";
  if(compresscheck=="zipfile"):
   return "zipfile";
+ if(rarfile_support and compresscheck=="rarfile"):
+  return "rarfile";
+ if(py7zr_support and compresscheck=="7zipfile"):
+  return "7zipfile";
  if(hasattr(infile, "read") or hasattr(infile, "write")):
   catfp = UncompressArchiveFile(infile, formatspecs[2]);
  else:
   try:
    if(compresscheck=="gzip"):
     try:
      import gzip;
@@ -3536,26 +3549,305 @@
    return catfp
   else:
    catfp.close()
    return True;
 
 create_alias_function("Pack", __file_format_name__, "FromRarFile", PackArchiveFileFromRarFile);
 
+if(not py7zr_support):
+ def PackArchiveFileFromSevenZipFile(infile, outfile, compression="auto", compressionlevel=None, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False, returnfp=False):
+  return False
+
+if(py7zr_support):
+ def PackArchiveFileFromSevenZipFile(infile, outfile, compression="auto", compressionlevel=None, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False, returnfp=False):
+  if(outfile!="-" and not hasattr(outfile, "read") and not hasattr(outfile, "write")):
+   outfile = RemoveWindowsPath(outfile);
+  checksumtype = checksumtype.lower();
+  if(not CheckSumSupport(checksumtype, hashlib_guaranteed)):
+   checksumtype="crc32";
+  if(checksumtype=="none"):
+   checksumtype = "";
+  if(not compression or compression or compression=="catfile" or compression==formatspecs[2]):
+   compression = None;
+  if(compression not in compressionlist and compression is None):
+   compression = "auto";
+  if(verbose):
+   logging.basicConfig(format="%(message)s", stream=sys.stdout, level=logging.DEBUG);
+  if(outfile!="-" and not hasattr(outfile, "read") and not hasattr(outfile, "write")):
+   if(os.path.exists(outfile)):
+    os.unlink(outfile);
+  if(outfile=="-"):
+   verbose = False;
+   catfp = BytesIO();
+  elif(hasattr(outfile, "read") or hasattr(outfile, "write")):
+   catfp = outfile;
+  elif(re.findall(r"^(ftp|ftps|sftp)\:\/\/", str(outfile))):
+   catfp = BytesIO();
+  else:
+   fbasename = os.path.splitext(outfile)[0];
+   fextname = os.path.splitext(outfile)[1];
+   catfp = CompressOpenFile(outfile, compressionlevel);
+  catver = formatspecs[6];
+  fileheaderver = str(int(catver.replace(".", "")));
+  fileheader = AppendNullByte(formatspecs[1] + fileheaderver, formatspecs[5]);
+  catfp.write(fileheader.encode('UTF-8'));
+  curinode = 0;
+  curfid = 0;
+  inodelist = [];
+  inodetofile = {};
+  filetoinode = {};
+  inodetocatinode = {};
+  if(not os.path.exists(infile) or not os.path.isfile(infile)):
+   return False;
+  szpfp = py7zr.SevenZipFile(infile, mode="r");
+  file_content = szpfp.readall();
+  #sztest = szpfp.testzip();
+  sztestalt = szpfp.test();
+  if(sztestalt):
+   VerbosePrintOut("Bad file found!");
+  numfiles = int(len(szpfp.list()));
+  fnumfiles = format(int(len(szpfp.list())), 'x').lower();
+  fnumfilesa = AppendNullBytes([fnumfiles, checksumtype], formatspecs[5]);
+  if(checksumtype=="none" or checksumtype==""):
+   catfileheadercshex = format(0, 'x').lower();
+  elif(checksumtype=="crc16" or checksumtype=="crc16_ansi" or checksumtype=="crc16_ibm"):
+   catfileheadercshex = format(crc16(str(fileheader + fnumfilesa).encode('UTF-8')) & 0xffff, '04x').lower();
+  elif(checksumtype=="crc16_ccitt"):
+   catfileheadercshex = format(crc16_ccitt(str(fileheader + fnumfilesa).encode('UTF-8')) & 0xffff, '04x').lower();
+  elif(checksumtype=="adler32"):
+   catfileheadercshex = format(zlib.adler32(str(fileheader + fnumfilesa).encode('UTF-8')) & 0xffffffff, '08x').lower();
+  elif(checksumtype=="crc32"):
+   catfileheadercshex = format(crc32(str(fileheader + fnumfilesa).encode('UTF-8')) & 0xffffffff, '08x').lower();
+  elif(checksumtype=="crc64_ecma"):
+   catfileheadercshex = format(crc64_ecma(str(fileheader + fnumfilesa).encode('UTF-8')) & 0xffffffffffffffff, '016x').lower();
+  elif(checksumtype=="crc64" or checksumtype=="crc64_iso"):
+   catfileheadercshex = format(crc64_iso(str(fileheader + fnumfilesa).encode('UTF-8')) & 0xffffffffffffffff, '016x').lower();
+  elif(CheckSumSupportAlt(checksumtype, hashlib_guaranteed)):
+   checksumoutstr = hashlib.new(checksumtype);
+   checksumoutstr.update(str(fileheader + fnumfilesa).encode('UTF-8'));
+   catfileheadercshex = checksumoutstr.hexdigest().lower();
+  else:
+   catfileheadercshex = format(0, 'x').lower();
+  fnumfilesa = fnumfilesa + AppendNullByte(catfileheadercshex, formatspecs[5]);
+  catfp.write(fnumfilesa.encode('UTF-8'));
+  try:
+   catfp.flush();
+   os.fsync(catfp.fileno());
+  except io.UnsupportedOperation:
+   pass;
+  except AttributeError:
+   pass;
+  for member in sorted(szpfp.list(), key=lambda x: x.filename):
+   catfhstart = catfp.tell();
+   if(re.findall("^[.|/]", member.filename)):
+    fname = member.filename;
+   else:
+    fname = "./"+member.filename;
+   if(verbose):
+    VerbosePrintOut(fname);
+   if(not member.is_directory):
+    fpremode = int(stat.S_IFREG + 438);
+   elif(member.is_directory):
+    fpremode = int(stat.S_IFDIR + 511);
+   fwinattributes = format(int(0), 'x').lower();
+   flinkcount = 0;
+   ftype = 0;
+   if(member.is_directory):
+    ftype = 5;
+   else:
+    ftype = 0;
+   flinkname = "";
+   fcurfid = format(int(curfid), 'x').lower();
+   fcurinode = format(int(curfid), 'x').lower();
+   curfid = curfid + 1;
+   fdev_minor = format(int(0), 'x').lower();
+   fdev_major = format(int(0), 'x').lower();
+   frdev_minor = format(int(0), 'x').lower();
+   frdev_major = format(int(0), 'x').lower();
+   if(ftype==5):
+    fsize = format(int("0"), 'x').lower();
+   fatime = format(int(member.creationtime.timestamp()), 'x').lower();
+   fmtime = format(int(member.creationtime.timestamp()), 'x').lower();
+   fctime = format(int(member.creationtime.timestamp()), 'x').lower();
+   fbtime = format(int(member.creationtime.timestamp()), 'x').lower();
+   if(member.is_directory):
+    fmode = format(int(stat.S_IFDIR + 511), 'x').lower();
+    fchmode = format(int(stat.S_IMODE(int(stat.S_IFDIR + 511))), 'x').lower();
+    ftypemod = format(int(stat.S_IFMT(int(stat.S_IFDIR + 511))), 'x').lower();
+   else:
+    fmode = format(int(stat.S_IFREG + 438), 'x').lower();
+    fchmode = format(int(stat.S_IMODE(int(stat.S_IFREG + 438))), 'x').lower();
+    ftypemod = format(int(stat.S_IFMT(int(stat.S_IFREG + 438))), 'x').lower();
+   try:
+    fuid = format(int(os.getuid()), 'x').lower();
+   except AttributeError:
+    fuid = format(int(0), 'x').lower();
+   except KeyError:
+    fuid = format(int(0), 'x').lower();
+   try:
+    fgid = format(int(os.getgid()), 'x').lower();
+   except AttributeError:
+    fgid = format(int(0), 'x').lower();
+   except KeyError:
+    fgid = format(int(0), 'x').lower();
+   try:
+    import pwd;
+    try:
+     userinfo = pwd.getpwuid(os.getuid());
+     funame = userinfo.pw_name;
+    except KeyError:
+     funame = "";
+    except AttributeError:
+     funame = "";
+   except ImportError:
+    funame = "";
+   fgname = "";
+   try:
+    import grp;
+    try:
+     groupinfo = grp.getgrgid(os.getgid());
+     fgname = groupinfo.gr_name;
+    except KeyError:
+     fgname = "";
+    except AttributeError:
+     fgname = "";
+   except ImportError:
+    fgname = "";
+   fcontents = "".encode('UTF-8');
+   if(ftype==0):
+    fcontents = file_content[member.filename].read();
+    fsize = format(len(fcontents), 'x').lower();
+    file_content[member.filename].close();
+   ftypehex = format(ftype, 'x').lower();
+   extrafields = format(len(extradata), 'x').lower();
+   extrasizestr = AppendNullByte(extrafields, formatspecs[5]);
+   if(len(extradata)>0):
+    extrasizestr = extrasizestr + AppendNullBytes(extradata, formatspecs[5]);
+   extrasizelen = format(len(extrasizestr), 'x').lower();
+   catoutlist = [ftypehex, fname, flinkname, fsize, fatime, fmtime, fctime, fbtime, fmode, fwinattributes, fuid, funame, fgid, fgname, fcurfid, fcurinode, flinkcount, fdev_minor, fdev_major, frdev_minor, frdev_major, extrasizelen, extrafields];
+   catoutlen = len(catoutlist) + len(extradata) + 3;
+   catoutlenhex = format(catoutlen, 'x').lower();
+   catoutlist.insert(0, catoutlenhex);
+   catfileoutstr = AppendNullBytes(catoutlist, formatspecs[5]);
+   if(len(extradata)>0):
+    catfileoutstr = catfileoutstr + AppendNullBytes(extradata, formatspecs[5]);
+   catfileoutstr = catfileoutstr + AppendNullByte(checksumtype, formatspecs[5]);
+   catfhend = (catfp.tell() - 1) + len(catfileoutstr);
+   catfcontentstart = catfp.tell() + len(catfileoutstr);
+   if(checksumtype=="none" or checksumtype==""):
+    catfileheadercshex = format(0, 'x').lower();
+    catfilecontentcshex = format(0, 'x').lower();
+   elif(checksumtype=="crc16" or checksumtype=="crc16_ansi" or checksumtype=="crc16_ibm"):
+    catfileheadercshex = format(crc16("".encode('UTF-8')) & 0xffff, '04x').lower();
+    catfilecontentcshex = format(crc16(fcontents) & 0xffff, '04x').lower();
+   elif(checksumtype=="crc16_ccitt"):
+    catfileheadercshex = format(crc16_ccitt("".encode('UTF-8')) & 0xffff, '04x').lower();
+    catfilecontentcshex = format(crc16_ccitt(fcontents) & 0xffff, '04x').lower();
+   elif(checksumtype=="adler32"):
+    catfileheadercshex = format(zlib.adler32("".encode('UTF-8')) & 0xffffffff, '08x').lower();
+    catfilecontentcshex = format(zlib.adler32(fcontents) & 0xffffffff, '08x').lower();
+   elif(checksumtype=="crc32"):
+    catfileheadercshex = format(crc32("".encode('UTF-8')) & 0xffffffff, '08x').lower();
+    catfilecontentcshex = format(crc32(fcontents) & 0xffffffff, '08x').lower();
+   elif(checksumtype=="crc64_ecma"):
+    catfileheadercshex = format(crc64_ecma("".encode('UTF-8')) & 0xffffffffffffffff, '016x').lower();
+    catfilecontentcshex = format(crc64_ecma(fcontents) & 0xffffffffffffffff, '016x').lower();
+   elif(checksumtype=="crc64" or checksumtype=="crc64_iso"):
+    catfileheadercshex = format(crc64_iso("".encode('UTF-8')) & 0xffffffffffffffff, '016x').lower();
+    catfilecontentcshex = format(crc64_iso(fcontents) & 0xffffffffffffffff, '016x').lower();
+   elif(CheckSumSupportAlt(checksumtype, hashlib_guaranteed)):
+    checksumoutstr = hashlib.new(checksumtype);
+    checksumoutstr.update("".encode('UTF-8'));
+    catfileheadercshex = checksumoutstr.hexdigest().lower();
+    checksumoutstr = hashlib.new(checksumtype);
+    checksumoutstr.update(fcontents);
+    catfilecontentcshex = checksumoutstr.hexdigest().lower();
+   else:
+    catfileheadercshex = format(0, 'x').lower();
+    catfilecontentcshex = format(0, 'x').lower();
+   tmpfileoutstr = catfileoutstr + AppendNullBytes([catfileheadercshex, catfilecontentcshex], formatspecs[5]);
+   catheaersize = format(int(len(tmpfileoutstr) - 1), 'x').lower()
+   catfileoutstr = AppendNullByte(catheaersize, formatspecs[5]) + catfileoutstr
+   if(checksumtype=="none" or checksumtype==""):
+    catfileheadercshex = format(0, 'x').lower()
+   elif(checksumtype=="crc16" or checksumtype=="crc16_ansi" or checksumtype=="crc16_ibm"):
+    catfileheadercshex = format(crc16(catfileoutstr.encode('UTF-8')) & 0xffff, '04x').lower()
+   elif(checksumtype=="crc16_ccitt"):
+    catfileheadercshex = format(crc16_ccitt(catfileoutstr.encode('UTF-8')) & 0xffff, '04x').lower()
+   elif(checksumtype=="adler32"):
+    catfileheadercshex = format(zlib.adler32(catfileoutstr.encode('UTF-8')) & 0xffffffff, '08x').lower()
+   elif(checksumtype=="crc32"):
+    catfileheadercshex = format(crc32(catfileoutstr.encode('UTF-8')) & 0xffffffff, '08x').lower()
+   elif(checksumtype=="crc64_ecma"):
+    catfileheadercshex = format(crc64_ecma(catfileoutstr.encode('UTF-8')) & 0xffffffffffffffff, '016x').lower()
+   elif(checksumtype=="crc64" or checksumtype=="crc64_iso"):
+    catfileheadercshex = format(crc64_iso(catfileoutstr.encode('UTF-8')) & 0xffffffffffffffff, '016x').lower()
+   elif(CheckSumSupportAlt(checksumtype, hashlib_guaranteed)):
+    checksumoutstr = hashlib.new(checksumtype)
+    checksumoutstr.update(catfileoutstr.encode('UTF-8'))
+    catfileheadercshex = checksumoutstr.hexdigest().lower()
+   else:
+    catfileheadercshex = format(0, 'x').lower()
+   catfileoutstr = catfileoutstr + AppendNullBytes([catfileheadercshex, catfilecontentcshex], formatspecs[5])
+   catfileoutstrecd = catfileoutstr.encode('UTF-8')
+   nullstrecd = formatspecs[5].encode('UTF-8')
+   catfileout = catfileoutstrecd + fcontents + nullstrecd
+   catfcontentend = (catfp.tell() - 1) + len(catfileout)
+   catfp.write(catfileout)
+   try:
+    catfp.flush()
+    os.fsync(catfp.fileno())
+   except io.UnsupportedOperation:
+    pass
+   except AttributeError:
+    pass
+  if(numfiles>0):
+   catfp.write(AppendNullBytes([0, 0], formatspecs[5]).encode("UTF-8"));
+  if(outfile=="-" or hasattr(outfile, "read") or hasattr(outfile, "write")):
+   catfp = CompressArchiveFile(catfp, compression, formatspecs)
+   try:
+    catfp.flush()
+    os.fsync(catfp.fileno())
+   except io.UnsupportedOperation:
+    pass
+   except AttributeError:
+    pass
+  if(outfile=="-"):
+   catfp.seek(0, 0)
+   if(hasattr(sys.stdout, "buffer")):
+    shutil.copyfileobj(catfp, sys.stdout.buffer);
+   else:
+    shutil.copyfileobj(catfp, sys.stdout);
+  elif(re.findall(r"^(ftp|ftps|sftp)\:\/\/", str(outfile))):
+   catfp = CompressArchiveFile(catfp, compression, formatspecs);
+   catfp.seek(0, 0);
+   upload_file_to_internet_file(catfp, outfile);
+  if(returnfp):
+   catfp.seek(0, 0)
+   return catfp
+  else:
+   catfp.close()
+   return True;
+
+create_alias_function("Pack", __file_format_name__, "FromSevenZipFile", PackArchiveFileFromSevenZipFile);
+
 def ArchiveFileSeekToFileNum(infile, seekto=0, skipchecksum=False, formatspecs=__file_format_list__, returnfp=False):
  if(hasattr(infile, "read") or hasattr(infile, "write")):
   catfp = infile;
   catfp.seek(0, 0);
   catfp = UncompressArchiveFile(catfp, formatspecs);
   checkcompressfile = CheckCompressionSubType(catfp, formatspecs);
   if(checkcompressfile=="tarfile"):
    return TarFileToArray(infile, 0, 0, listonly, skipchecksum, formatspecs, returnfp);
   if(checkcompressfile=="zipfile"):
    return ZipFileToArray(infile, 0, 0, listonly, skipchecksum, formatspecs, returnfp);
   if(rarfile_support and checkcompressfile=="rarfile"):
    return RarFileToArray(infile, 0, 0, listonly, skipchecksum, formatspecs, returnfp);
+  if(py7zr_support and checkcompressfile=="7zipfile"):
+   return SevenZipFileToArray(infile, 0, 0, listonly, skipchecksum, formatspecs, returnfp);
   if(checkcompressfile!="catfile" and checkcompressfile!=formatspecs[2]):
    return False;
   if(not catfp):
    return False;
   catfp.seek(0, 0);
  elif(infile=="-"):
   catfp = BytesIO();
@@ -3580,14 +3872,16 @@
   checkcompressfile = CheckCompressionSubType(infile, formatspecs);
   if(checkcompressfile=="tarfile"):
    return TarFileToArray(infile, 0, 0, listonly, skipchecksum, formatspecs, returnfp);
   if(checkcompressfile=="zipfile"):
    return ZipFileToArray(infile, 0, 0, listonly, skipchecksum, formatspecs, returnfp);
   if(rarfile_support and checkcompressfile=="rarfile"):
    return RarFileToArray(infile, 0, 0, listonly, skipchecksum, formatspecs, returnfp);
+  if(py7zr_support and checkcompressfile=="7zipfile"):
+   return SevenZipFileToArray(infile, 0, 0, listonly, skipchecksum, formatspecs, returnfp);
   if(checkcompressfile!="catfile" and checkcompressfile!=formatspecs[2]):
    return False;
   compresscheck = CheckCompressionType(infile, formatspecs, True);
   if(not compresscheck):
    fextname = os.path.splitext(infile)[1];
    if(fextname==".gz"):
     compresscheck = "gzip";
@@ -3773,14 +4067,16 @@
   checkcompressfile = CheckCompressionSubType(catfp, formatspecs);
   if(checkcompressfile=="tarfile"):
    return TarFileToArray(infile, 0, 0, listonly, skipchecksum, formatspecs, returnfp);
   if(checkcompressfile=="zipfile"):
    return ZipFileToArray(infile, 0, 0, listonly, skipchecksum, formatspecs, returnfp);
   if(rarfile_support and checkcompressfile=="rarfile"):
    return RarFileToArray(infile, 0, 0, listonly, skipchecksum, formatspecs, returnfp);
+  if(py7zr_support and checkcompressfile=="7zipfile"):
+   return SevenZipFileToArray(infile, 0, 0, listonly, skipchecksum, formatspecs, returnfp);
   if(checkcompressfile!="catfile" and checkcompressfile!=formatspecs[2]):
    return False;
   if(not catfp):
    return False;
   catfp.seek(0, 0);
  elif(infile=="-"):
   catfp = BytesIO();
@@ -3805,14 +4101,16 @@
   checkcompressfile = CheckCompressionSubType(infile, formatspecs);
   if(checkcompressfile=="tarfile"):
    return TarFileToArray(infile, 0, 0, listonly, skipchecksum, formatspecs, returnfp);
   if(checkcompressfile=="zipfile"):
    return ZipFileToArray(infile, 0, 0, listonly, skipchecksum, formatspecs, returnfp);
   if(rarfile_support and checkcompressfile=="rarfile"):
    return RarFileToArray(infile, 0, 0, listonly, skipchecksum, formatspecs, returnfp);
+  if(py7zr_support and checkcompressfile=="7zipfile"):
+   return SevenZipFileToArray(infile, 0, 0, listonly, skipchecksum, formatspecs, returnfp);
   if(checkcompressfile!="catfile" and checkcompressfile!=formatspecs[2]):
    return False;
   compresscheck = CheckCompressionType(infile, formatspecs, True);
   if(not compresscheck):
    fextname = os.path.splitext(infile)[1];
    if(fextname==".gz"):
     compresscheck = "gzip";
@@ -4010,14 +4308,16 @@
   checkcompressfile = CheckCompressionSubType(catfp, formatspecs);
   if(checkcompressfile=="tarfile"):
    return TarFileToArray(infile, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
   if(checkcompressfile=="zipfile"):
    return ZipFileToArray(infile, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
   if(rarfile_support and checkcompressfile=="rarfile"):
    return RarFileToArray(infile, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
+  if(py7zr_support and checkcompressfile=="7zipfile"):
+   return SevenZipFileToArray(infile, 0, 0, listonly, skipchecksum, formatspecs, returnfp);
   if(checkcompressfile!="catfile" and checkcompressfile!=formatspecs[2]):
    return False;
   if(not catfp):
    return False;
   catfp.seek(0, 0);
  elif(infile=="-"):
   catfp = BytesIO();
@@ -4042,14 +4342,16 @@
   checkcompressfile = CheckCompressionSubType(infile, formatspecs);
   if(checkcompressfile=="tarfile"):
    return TarFileToArray(infile, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
   if(checkcompressfile=="zipfile"):
    return ZipFileToArray(infile, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
   if(rarfile_support and checkcompressfile=="rarfile"):
    return RarFileToArray(infile, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
+  if(py7zr_support and checkcompressfile=="7zipfile"):
+   return SevenZipFileToArray(infile, 0, 0, listonly, skipchecksum, formatspecs, returnfp);
   if(checkcompressfile!="catfile" and checkcompressfile!=formatspecs[2]):
    return False;
   compresscheck = CheckCompressionType(infile, formatspecs, True);
   if(not compresscheck):
    fextname = os.path.splitext(infile)[1];
    if(fextname==".gz"):
     compresscheck = "gzip";
@@ -4243,14 +4545,16 @@
   checkcompressfile = CheckCompressionSubType(catfp, formatspecs);
   if(checkcompressfile=="tarfile"):
    return TarFileToArray(infile, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
   if(checkcompressfile=="zipfile"):
    return ZipFileToArray(infile, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
   if(rarfile_support and checkcompressfile=="rarfile"):
    return RarFileToArray(infile, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
+  if(py7zr_support and checkcompressfile=="7zipfile"):
+   return SevenZipFileToArray(infile, 0, 0, listonly, skipchecksum, formatspecs, returnfp);
   if(checkcompressfile!="catfile" and checkcompressfile!=formatspecs[2]):
    return False;
   if(not catfp):
    return False;
   catfp.seek(0, 0);
  elif(infile=="-"):
   catfp = BytesIO();
@@ -4275,14 +4579,16 @@
   checkcompressfile = CheckCompressionSubType(infile, formatspecs);
   if(checkcompressfile=="tarfile"):
    return TarFileToArray(infile, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
   if(checkcompressfile=="zipfile"):
    return ZipFileToArray(infile, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
   if(rarfile_support and checkcompressfile=="rarfile"):
    return RarFileToArray(infile, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
+  if(py7zr_support and checkcompressfile=="7zipfile"):
+   return SevenZipFileToArray(infile, 0, 0, listonly, skipchecksum, formatspecs, returnfp);
   if(checkcompressfile!="catfile" and checkcompressfile!=formatspecs[2]):
    return False;
   compresscheck = CheckCompressionType(infile, formatspecs, True);
   if(not compresscheck):
    fextname = os.path.splitext(infile)[1];
    if(fextname==".gz"):
     compresscheck = "gzip";
@@ -5186,36 +5492,36 @@
   else:
    fsize = member.file_size;
   fatime = time.mktime(member.date_time + (0, 0, -1));
   fmtime = time.mktime(member.date_time + (0, 0, -1));
   fctime = time.mktime(member.date_time + (0, 0, -1));
   fbtime = time.mktime(member.date_time + (0, 0, -1));
   if(zipinfo.create_system==0 or zipinfo.create_system==10):
-   fwinattributes = format(int(zipinfo.external_attr), 'x').lower();
+   fwinattributes = int(zipinfo.external_attr);
    if(not member.is_dir()):
-    fmode = format(int(stat.S_IFREG + 438), 'x').lower();
-    fchmode = format(int(stat.S_IMODE(int(stat.S_IFREG + 438))), 'x').lower();
-    ftypemod = format(int(stat.S_IFMT(int(stat.S_IFREG + 438))), 'x').lower();
+    fmode = int(stat.S_IFREG + 438);
+    fchmode = int(stat.S_IMODE(int(stat.S_IFREG + 438)));
+    ftypemod = int(stat.S_IFMT(int(stat.S_IFREG + 438)));
    elif(member.is_dir()):
-    fmode = format(int(stat.S_IFDIR + 511), 'x').lower();
-    fchmode = format(int(stat.S_IMODE(int(stat.S_IFDIR + 511))), 'x').lower();
-    ftypemod = format(int(stat.S_IFMT(int(stat.S_IFDIR + 511))), 'x').lower();
+    fmode = int(stat.S_IFDIR + 511);
+    fchmode = int(stat.S_IMODE(int(stat.S_IFDIR + 511)));
+    ftypemod = int(stat.S_IFMT(int(stat.S_IFDIR + 511)));
   elif(zipinfo.create_system==3):
-   fwinattributes = format(int(0), 'x').lower();
-   fmode = format(int(zipinfo.external_attr), 'x').lower();
+   fwinattributes = int(0);
+   fmode = int(zipinfo.external_attr);
   else:
-   fwinattributes = format(int(0), 'x').lower();
+   fwinattributes = int(0);
    if(not member.is_dir()):
-    fmode = format(int(stat.S_IFREG + 438), 'x').lower();
-    fchmode = format(int(stat.S_IMODE(int(stat.S_IFREG + 438))), 'x').lower();
-    ftypemod = format(int(stat.S_IFMT(int(stat.S_IFREG + 438))), 'x').lower();
+    fmode = int(stat.S_IFREG + 438);
+    fchmode = int(stat.S_IMODE(int(stat.S_IFREG + 438)));
+    ftypemod = int(stat.S_IFMT(int(stat.S_IFREG + 438)));
    elif(member.is_dir()):
-    fmode = format(int(stat.S_IFDIR + 511), 'x').lower();
-    fchmode = format(int(stat.S_IMODE(int(stat.S_IFDIR + 511))), 'x').lower();
-    ftypemod = format(int(stat.S_IFMT(int(stat.S_IFDIR + 511))), 'x').lower();
+    fmode = int(stat.S_IFDIR + 511);
+    fchmode = int(stat.S_IMODE(int(stat.S_IFDIR + 511)));
+    ftypemod = int(stat.S_IFMT(int(stat.S_IFDIR + 511)));
   try:
    fuid = os.getuid();
   except AttributeError:
    fuid = 0;
   except KeyError:
    fuid = 0;
   try:
@@ -5471,17 +5777,17 @@
      fctime = int(member.ctime.timestamp());
     else:
      fctime = int(member.mtime.timestamp());
    except AttributeError:
     fctime = int(member.mtime.timestamp());
    fbtime = int(member.mtime.timestamp());
    if(is_unix and member.external_attr !=0):
-    fmode = format(int(member.external_attr), 'x').lower();
-    fchmode = format(int(stat.S_IMODE(member.external_attr)), 'x').lower();
-    ftypemod = format(int(stat.S_IFMT(member.external_attr)), 'x').lower();
+    fmode = int(member.external_attr);
+    fchmode = int(stat.S_IMODE(member.external_attr));
+    ftypemod = int(stat.S_IFMT(member.external_attr));
    elif(member.is_file()):
     fmode = int(stat.S_IFREG + 438)
     fchmode = int(stat.S_IMODE(stat.S_IFREG + 438));
     ftypemod = int(stat.S_IFMT(stat.S_IFREG + 438));
    elif(member.is_symlink()):
     fmode = int(stat.S_IFLNK + 438)
     fchmode = int(stat.S_IMODE(stat.S_IFREG + 438));
@@ -5614,14 +5920,234 @@
    if(int(fsize)>0 and listonly):
     fcontents = "";
     pyhascontents = False;
    catlist['ffilelist'].update({fileidnum: {'fid': fileidnum, 'fidalt': fileidnum, 'fheadersize': int(catheaersize, 16), 'fhstart': catfhstart, 'fhend': catfhend, 'ftype': ftype, 'fname': fname, 'fbasedir': fbasedir, 'flinkname': flinkname, 'fsize': fsize, 'fatime': fatime, 'fmtime': fmtime, 'fctime': fctime, 'fbtime': fbtime, 'fmode': fmode, 'fchmode': fchmode, 'ftypemod': ftypemod, 'fwinattributes': fwinattributes, 'fuid': fuid, 'funame': funame, 'fgid': fgid, 'fgname': fgname, 'finode': finode, 'flinkcount': flinkcount, 'fminor': fdev_minor, 'fmajor': fdev_major, 'frminor': frdev_minor, 'frmajor': frdev_major, 'fchecksumtype': checksumtype, 'fnumfields': catfnumfields + 2, 'frawheader': catheaderdata, 'fextrafields': catfextrafields, 'fextrafieldsize': extrasizelen, 'fextralist': extrafieldslist, 'fheaderchecksum': int(catfileheadercshex, 16), 'fcontentchecksum': int(catfilecontentcshex, 16), 'fhascontents': pyhascontents, 'fcontentstart': catfcontentstart, 'fcontentend': catfcontentend, 'fcontents': fcontents} });
    fileidnum = fileidnum + 1;
   return catlist;
 
+if(not py7zr_support):
+ def SevenZipFileToArrayAlt(infiles, listonly=False, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False):
+  return False;
+
+if(py7zr_support):
+ def SevenZipFileToArrayAlt(infiles, listonly=False, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False):
+  curinode = 0;
+  curfid = 0;
+  inodelist = [];
+  inodetofile = {};
+  filetoinode = {};
+  inodetocatinode = {};
+  fileidnum = 0;
+  szpfp = py7zr.SevenZipFile(infile, mode="r");
+  file_content = szpfp.readall();
+  #sztest = szpfp.testzip();
+  sztestalt = szpfp.test();
+  if(sztestalt):
+   VerbosePrintOut("Bad file found!");
+  numfiles = int(len(szpfp.list()));
+  catver = formatspecs[6];
+  fileheaderver = str(int(catver.replace(".", "")));
+  fileheader = AppendNullByte(formatspecs[1] + fileheaderver, formatspecs[5]);
+  catversion = re.findall(r"([\d]+)$", fileheader);
+  catversions = re.search(r'(.*?)(\d+)$', catstring).groups();
+  fnumfileshex = format(int(fnumfiles), 'x').lower();
+  fileheader = fileheader + AppendNullBytes([fnumfileshex, checksumtype], formatspecs[5]);
+  if(checksumtype=="none" or checksumtype==""):
+   catfileheadercshex = format(0, 'x').lower();
+  elif(checksumtype=="crc16" or checksumtype=="crc16_ansi" or checksumtype=="crc16_ibm"):
+   catfileheadercshex = format(crc16(fileheader.encode('UTF-8')) & 0xffff, '04x').lower();
+  elif(checksumtype=="crc16_ccitt"):
+   catfileheadercshex = format(crc16_ccitt(fileheader.encode('UTF-8')) & 0xffff, '04x').lower();
+  elif(checksumtype=="adler32"):
+   catfileheadercshex = format(zlib.adler32(fileheader.encode('UTF-8')) & 0xffffffff, '08x').lower();
+  elif(checksumtype=="crc32"):
+   catfileheadercshex = format(crc32(fileheader.encode('UTF-8')) & 0xffffffff, '08x').lower();
+  elif(checksumtype=="crc64_ecma"):
+   catfileheadercshex = format(crc64_ecma(fileheader.encode('UTF-8')) & 0xffffffffffffffff, '016x').lower();
+  elif(checksumtype=="crc64" or checksumtype=="crc64_iso"):
+   catfileheadercshex = format(crc64_iso(fileheader.encode('UTF-8')) & 0xffffffffffffffff, '016x').lower();
+  elif(CheckSumSupportAlt(checksumtype, hashlib_guaranteed)):
+   checksumoutstr = hashlib.new(checksumtype);
+   checksumoutstr.update(fileheader.encode('UTF-8'));
+   catfileheadercshex = checksumoutstr.hexdigest().lower();
+  else:
+   catfileheadercshex = format(0, 'x').lower();
+  fileheader = fileheader + AppendNullByte(catfileheadercshex, formatspecs[5]);
+  fheadtell = len(fileheader);
+  catlist = {'fnumfiles': fnumfiles, 'fformat': catversions[0], 'fversion': catversions[1], 'fformatspecs': formatspecs, 'fchecksumtype': checksumtype, 'fheaderchecksum': catfileheadercshex, 'ffilelist': {}};
+  for member in sorted(szpfp.list(), key=lambda x: x.filename):
+   if(re.findall("^[.|/]", member.filename)):
+    fname = member.filename;
+   else:
+    fname = "./"+member.filename;
+   if(not member.is_directory):
+    fpremode = int(stat.S_IFREG + 438);
+   elif(member.is_directory):
+    fpremode = int(stat.S_IFDIR + 511);
+   fwinattributes = int(0);
+   flinkcount = 0;
+   ftype = 0;
+   if(member.is_directory):
+    ftype = 5;
+   else:
+    ftype = 0;
+   flinkname = "";
+   fbasedir = os.path.dirname(fname);
+   fcurfid = curfid;
+   fcurinode = curfid;
+   finode = fcurinode;
+   curfid = curfid + 1;
+   fdev_minor = 0;
+   fdev_major = 0;
+   frdev_minor = 0;
+   frdev_major = 0;
+   if(ftype==5):
+    fsize = "0";
+   fatime = int(member.creationtime.timestamp());
+   fmtime = int(member.creationtime.timestamp());
+   fctime = int(member.creationtime.timestamp());
+   fbtime = int(member.creationtime.timestamp());
+   if(member.is_directory):
+    fmode = int(stat.S_IFDIR + 511)
+    fchmode = int(stat.S_IMODE(stat.S_IFDIR + 511));
+    ftypemod = int(stat.S_IFMT(stat.S_IFDIR + 511));
+   else:
+    fmode = int(stat.S_IFLNK + 438)
+    fchmode = int(stat.S_IMODE(stat.S_IFREG + 438));
+    ftypemod = int(stat.S_IFMT(stat.S_IFREG + 438));
+   try:
+    fuid = os.getuid();
+   except AttributeError:
+    fuid = 0;
+   except KeyError:
+    fuid = 0;
+   try:
+    fgid = os.getgid();
+   except AttributeError:
+    fgid = 0;
+   except KeyError:
+    fgid = 0;
+   try:
+    import pwd;
+    try:
+     userinfo = pwd.getpwuid(os.getuid());
+     funame = userinfo.pw_name;
+    except KeyError:
+     funame = "";
+    except AttributeError:
+     funame = "";
+   except ImportError:
+    funame = "";
+   fgname = "";
+   try:
+    import grp;
+    try:
+     groupinfo = grp.getgrgid(os.getgid());
+     fgname = groupinfo.gr_name;
+    except KeyError:
+     fgname = "";
+    except AttributeError:
+     fgname = "";
+   except ImportError:
+    fgname = "";
+   fcontents = "".encode('UTF-8');
+   if(ftype==0):
+    fcontents = file_content[member.filename].read();
+    fsize = format(len(fcontents), 'x').lower();
+    fileop.close();
+   ftypehex = format(ftype, 'x').lower();
+   extrafields = len(extradata);
+   extrafieldslist = extradata;
+   catfextrafields = extrafields;
+   extrasizestr = AppendNullByte(extrafields, formatspecs[5]);
+   if(len(extradata)>0):
+    extrasizestr = extrasizestr + AppendNullBytes(extradata, formatspecs[5]);
+   extrasizelen = len(extrasizestr);
+   extrasizelenhex = format(extrasizelen, 'x').lower();
+   catoutlist = [ftypehex, fname, flinkname, format(int(fsize), 'x').lower(), format(int(fatime), 'x').lower(), format(int(fmtime), 'x').lower(), format(int(fctime), 'x').lower(), format(int(fbtime), 'x').lower(), format(int(fmode), 'x').lower(), format(int(fwinattributes), 'x').lower(), format(int(fuid), 'x').lower(), funame, format(int(fgid), 'x').lower(), fgname, format(int(fcurfid), 'x').lower(), format(int(fcurinode), 'x').lower(), format(int(flinkcount), 'x').lower(), format(int(fdev_minor), 'x').lower(), format(int(fdev_major), 'x').lower(), format(int(frdev_minor), 'x').lower(), format(int(frdev_major), 'x').lower(), extrasizelenhex, format(catfextrafields, 'x').lower()];
+   catoutlen = len(catoutlist) + len(extradata) + 3;
+   catoutlenhex = format(catoutlen, 'x').lower();
+   catoutlist.insert(0, catoutlenhex);
+   catfileoutstr = AppendNullBytes(catoutlist, formatspecs[5]);
+   if(len(extradata)>0):
+    catfileoutstr = catfileoutstr + AppendNullBytes(extradata, formatspecs[5]);
+   catfileoutstr = catfileoutstr + AppendNullByte(checksumtype, formatspecs[5]);
+   catfnumfields = 24 + catfextrafields;
+   if(checksumtype=="none" or checksumtype==""):
+    catfileheadercshex = format(0, 'x').lower();
+    catfilecontentcshex = format(0, 'x').lower();
+   elif(checksumtype=="crc16" or checksumtype=="crc16_ansi" or checksumtype=="crc16_ibm"):
+    catfileheadercshex = format(crc16(catfileoutstr.encode('UTF-8')) & 0xffff, '04x').lower();
+    catfilecontentcshex = format(crc16(fcontents) & 0xffff, '04x').lower();
+   elif(checksumtype=="crc16_ccitt"):
+    catfileheadercshex = format(crc16_ccitt(catfileoutstr.encode('UTF-8')) & 0xffff, '04x').lower();
+    catfilecontentcshex = format(crc16_ccitt(fcontents) & 0xffff, '04x').lower();
+   elif(checksumtype=="adler32"):
+    catfileheadercshex = format(zlib.adler32(catfileoutstr.encode('UTF-8')) & 0xffffffff, '08x').lower();
+    catfilecontentcshex = format(zlib.adler32(fcontents) & 0xffffffff, '08x').lower();
+   elif(checksumtype=="crc32"):
+    catfileheadercshex = format(crc32(catfileoutstr.encode('UTF-8')) & 0xffffffff, '08x').lower();
+    catfilecontentcshex = format(crc32(fcontents) & 0xffffffff, '08x').lower();
+   elif(checksumtype=="crc64_ecma"):
+    catfileheadercshex = format(crc64_ecma(catfileoutstr.encode('UTF-8')) & 0xffffffffffffffff, '016x').lower();
+    catfilecontentcshex = format(crc64_ecma(fcontents) & 0xffffffffffffffff, '016x').lower();
+   elif(checksumtype=="crc64" or checksumtype=="crc64_iso"):
+    catfileheadercshex = format(crc64_iso(catfileoutstr.encode('UTF-8')) & 0xffffffffffffffff, '016x').lower();
+    catfilecontentcshex = format(crc64_iso(fcontents) & 0xffffffffffffffff, '016x').lower();
+   elif(CheckSumSupportAlt(checksumtype, hashlib_guaranteed)):
+    checksumoutstr = hashlib.new(checksumtype);
+    checksumoutstr.update(catfileoutstr.encode('UTF-8'));
+    catfileheadercshex = checksumoutstr.hexdigest().lower();
+   else:
+    catfileheadercshex = format(0, 'x').lower();
+    catfilecontentcshex = format(0, 'x').lower();
+   catfhstart = fheadtell;
+   fheadtell += len(catfileoutstr);
+   catfhend = fheadtell - 1;
+   catfcontentstart = fheadtell;
+   tmpfileoutstr = catfileoutstr + AppendNullBytes([catfileheadercshex, catfilecontentcshex], formatspecs[5]);
+   catheaersize = format(int(len(tmpfileoutstr) - 1), 'x').lower()
+   catfileoutstr = AppendNullByte(catheaersize, formatspecs[5]) + catfileoutstr;
+   catheaderdata = [catheaersize] + catoutlist + extradata + [checksumtype, catfileheadercshex, catfilecontentcshex];
+   if(checksumtype=="none" or checksumtype==""):
+    catfileheadercshex = format(0, 'x').lower();
+   elif(checksumtype=="crc16" or checksumtype=="crc16_ansi" or checksumtype=="crc16_ibm"):
+    catfileheadercshex = format(crc16(catfileoutstr.encode('UTF-8')) & 0xffff, '04x').lower();
+   elif(checksumtype=="crc16_ccitt"):
+    catfileheadercshex = format(crc16_ccitt(catfileoutstr.encode('UTF-8')) & 0xffff, '04x').lower();
+   elif(checksumtype=="adler32"):
+    catfileheadercshex = format(zlib.adler32(catfileoutstr.encode('UTF-8')) & 0xffffffff, '08x').lower();
+   elif(checksumtype=="crc32"):
+    catfileheadercshex = format(crc32(catfileoutstr.encode('UTF-8')) & 0xffffffff, '08x').lower();
+   elif(checksumtype=="crc64_ecma"):
+    catfileheadercshex = format(crc64_ecma(catfileoutstr.encode('UTF-8')) & 0xffffffffffffffff, '016x').lower();
+   elif(checksumtype=="crc64" or checksumtype=="crc64_iso"):
+    catfileheadercshex = format(crc64_iso(catfileoutstr.encode('UTF-8')) & 0xffffffffffffffff, '016x').lower();
+   elif(CheckSumSupportAlt(checksumtype, hashlib_guaranteed)):
+    checksumoutstr = hashlib.new(checksumtype);
+    checksumoutstr.update(catfileoutstr.encode('UTF-8'));
+    catfileheadercshex = checksumoutstr.hexdigest().lower();
+   else:
+    catfileheadercshex = format(0, 'x').lower();
+   catfileoutstr = catfileoutstr + AppendNullBytes([catfileheadercshex, catfilecontentcshex], formatspecs[5]);
+   catfileoutstrecd = catfileoutstr.encode('UTF-8');
+   nullstrecd = formatspecs[5].encode('UTF-8');
+   fheadtell += len(catfileoutstr) + 1;
+   catfcontentend = fheadtell - 1;
+   catfileout = catfileoutstrecd + fcontents + nullstrecd;
+   pyhascontents = False;
+   if(int(fsize)>0 and not listonly):
+    pyhascontents = True;
+   if(int(fsize)>0 and listonly):
+    fcontents = "";
+    pyhascontents = False;
+   catlist['ffilelist'].update({fileidnum: {'fid': fileidnum, 'fidalt': fileidnum, 'fheadersize': int(catheaersize, 16), 'fhstart': catfhstart, 'fhend': catfhend, 'ftype': ftype, 'fname': fname, 'fbasedir': fbasedir, 'flinkname': flinkname, 'fsize': fsize, 'fatime': fatime, 'fmtime': fmtime, 'fctime': fctime, 'fbtime': fbtime, 'fmode': fmode, 'fchmode': fchmode, 'ftypemod': ftypemod, 'fwinattributes': fwinattributes, 'fuid': fuid, 'funame': funame, 'fgid': fgid, 'fgname': fgname, 'finode': finode, 'flinkcount': flinkcount, 'fminor': fdev_minor, 'fmajor': fdev_major, 'frminor': frdev_minor, 'frmajor': frdev_major, 'fchecksumtype': checksumtype, 'fnumfields': catfnumfields + 2, 'frawheader': catheaderdata, 'fextrafields': catfextrafields, 'fextrafieldsize': extrasizelen, 'fextralist': extrafieldslist, 'fheaderchecksum': int(catfileheadercshex, 16), 'fcontentchecksum': int(catfilecontentcshex, 16), 'fhascontents': pyhascontents, 'fcontentstart': catfcontentstart, 'fcontentend': catfcontentend, 'fcontents': fcontents} });
+   fileidnum = fileidnum + 1;
+  return catlist;
+
 def ListDirToArray(infiles, dirlistfromtxt=False, compression="auto", compressionlevel=None, followlink=False, seekstart=0, seekend=0, listonly=False, skipchecksum=False, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False, returnfp=False):
  outarray = BytesIO();
  packcat = PackArchiveFile(infiles, outarray, dirlistfromtxt, compression, compressionlevel, followlink, checksumtype, extradata, formatspecs, verbose, True);
  listcatfiles = ArchiveFileToArray(outarray, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
  return listcatfiles;
 
 def ArchiveFileToArrayIndex(infile, seekstart=0, seekend=0, listonly=False, skipchecksum=False, formatspecs=__file_format_list__, returnfp=False):
@@ -5889,14 +6415,70 @@
     catarray['filetypes']['symlinks']['filetoid'].update(filetoidarray);
     catarray['filetypes']['symlinks']['idtofile'].update(idtofilearray);
     catarray['filetypes']['devices']['filetoid'].update(filetoidarray);
     catarray['filetypes']['devices']['idtofile'].update(idtofilearray);
    lcfi = lcfi + 1;
   return catarray;
 
+if(not py7zr_support):
+ def SevenZipFileToArrayIndexAlt(infiles, seekstart=0, seekend=0, listonly=False, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False):
+  return False;
+
+if(py7zr_support):
+ def SevenZipFileToArrayIndexAlt(infiles, seekstart=0, seekend=0, listonly=False, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False):
+  listcatfiles = SevenZipFileToArrayAlt(infiles, listonly, checksumtype, extradata, formatspecs, verbose);
+  if(not listcatfiles):
+   return False;
+  catarray = {'list': listcatfiles, 'filetoid': {}, 'idtofile': {}, 'filetypes': {'directories': {'filetoid': {}, 'idtofile': {}}, 'files': {'filetoid': {}, 'idtofile': {}}, 'links': {'filetoid': {}, 'idtofile': {}}, 'symlinks': {'filetoid': {}, 'idtofile': {}}, 'hardlinks': {'filetoid': {}, 'idtofile': {}}, 'character': {'filetoid': {}, 'idtofile': {}}, 'block': {'filetoid': {}, 'idtofile': {}}, 'fifo': {'filetoid': {}, 'idtofile': {}}, 'devices': {'filetoid': {}, 'idtofile': {}}}};
+  lenlist = len(listcatfiles['ffilelist']);
+  lcfi = 0;
+  lcfx = int(listcatfiles['fnumfiles']);
+  if(lenlist>listcatfiles['fnumfiles'] or lenlist<listcatfiles['fnumfiles']):
+   lcfx = int(lenlist);
+  else:
+   lcfx = int(listcatfiles['fnumfiles']);
+  while(lcfi < lcfx):
+   filetoidarray = {listcatfiles['ffilelist'][lcfi]['fname']: listcatfiles['ffilelist'][lcfi]['fid']};
+   idtofilearray = {listcatfiles['ffilelist'][lcfi]['fid']: listcatfiles['ffilelist'][lcfi]['fname']};
+   catarray['filetoid'].update(filetoidarray);
+   catarray['idtofile'].update(idtofilearray);
+   if(listcatfiles['ffilelist'][lcfi]['ftype']==0 or listcatfiles['ffilelist'][lcfi]['ftype']==7):
+    catarray['filetypes']['files']['filetoid'].update(filetoidarray);
+    catarray['filetypes']['files']['idtofile'].update(idtofilearray);
+   if(listcatfiles['ffilelist'][lcfi]['ftype']==1):
+    catarray['filetypes']['hardlinks']['filetoid'].update(filetoidarray);
+    catarray['filetypes']['hardlinks']['idtofile'].update(idtofilearray);
+    catarray['filetypes']['links']['filetoid'].update(filetoidarray);
+    catarray['filetypes']['links']['idtofile'].update(idtofilearray);
+   if(listcatfiles['ffilelist'][lcfi]['ftype']==2):
+    catarray['filetypes']['symlinks']['filetoid'].update(filetoidarray);
+    catarray['filetypes']['symlinks']['idtofile'].update(idtofilearray);
+    catarray['filetypes']['links']['filetoid'].update(filetoidarray);
+    catarray['filetypes']['links']['idtofile'].update(idtofilearray);
+   if(listcatfiles['ffilelist'][lcfi]['ftype']==3):
+    catarray['filetypes']['character']['filetoid'].update(filetoidarray);
+    catarray['filetypes']['character']['idtofile'].update(idtofilearray);
+    catarray['filetypes']['devices']['filetoid'].update(filetoidarray);
+    catarray['filetypes']['devices']['idtofile'].update(idtofilearray);
+   if(listcatfiles['ffilelist'][lcfi]['ftype']==4):
+    catarray['filetypes']['block']['filetoid'].update(filetoidarray);
+    catarray['filetypes']['block']['idtofile'].update(idtofilearray);
+    catarray['filetypes']['devices']['filetoid'].update(filetoidarray);
+   catarray['filetypes']['devices']['idtofile'].update(idtofilearray);
+   if(listcatfiles['ffilelist'][lcfi]['ftype']==5):
+    catarray['filetypes']['directories']['filetoid'].update(filetoidarray);
+    catarray['filetypes']['directories']['idtofile'].update(idtofilearray);
+   if(listcatfiles['ffilelist'][lcfi]['ftype']==6):
+    catarray['filetypes']['symlinks']['filetoid'].update(filetoidarray);
+    catarray['filetypes']['symlinks']['idtofile'].update(idtofilearray);
+    catarray['filetypes']['devices']['filetoid'].update(filetoidarray);
+    catarray['filetypes']['devices']['idtofile'].update(idtofilearray);
+   lcfi = lcfi + 1;
+  return catarray;
+
 def ArchiveFileStringToArrayIndex(catstr, seekstart=0, seekend=0, listonly=False, skipchecksum=False, formatspecs=__file_format_list__, returnfp=False):
  catfp = BytesIO(catstr);
  listcatfiles = ArchiveFileToArrayIndex(catfp, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
  return listcatfiles;
 
 create_alias_function("", __file_format_name__, "StringToArrayIndex", ArchiveFileStringToArrayIndex);
 
@@ -5919,14 +6501,25 @@
 if(rarfile_support):
  def RarFileToArrayIndex(infile, seekstart=0, seekend=0, listonly=False, skipchecksum=False, formatspecs=__file_format_list__, returnfp=False):
   catfp = BytesIO();
   catfp = PackArchiveFileFromRarFile(infile, catfp, "auto", None, "crc32", [], formatspecs, False, True);
   listcatfiles = ArchiveFileToArrayIndex(catfp, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
   return listcatfiles;
 
+if(not rarfile_support):
+ def SevenZipFileToArrayIndex(infile, seekstart=0, seekend=0, listonly=False, skipchecksum=False, formatspecs=__file_format_list__, returnfp=False):
+  return False;
+
+if(rarfile_support):
+ def SevenZipFileToArrayIndex(infile, seekstart=0, seekend=0, listonly=False, skipchecksum=False, formatspecs=__file_format_list__, returnfp=False):
+  catfp = BytesIO();
+  catfp = PackArchiveFileFromSevenZipFile(infile, catfp, "auto", None, "crc32", [], formatspecs, False, True);
+  listcatfiles = ArchiveFileToArrayIndex(catfp, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
+  return listcatfiles;
+
 def ListDirToArrayIndex(infiles, dirlistfromtxt=False, compression="auto", compressionlevel=None, followlink=False, seekstart=0, seekend=0, listonly=False, skipchecksum=False, checksumtype="crc32", formatspecs=__file_format_list__, verbose=False, returnfp=False):
  outarray = BytesIO();
  packcat = PackArchiveFile(infiles, outarray, dirlistfromtxt, compression, compressionlevel, followlink, checksumtype, formatspecs, verbose, True);
  listcatfiles = ArchiveFileToArrayIndex(outarray, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp)
  return listcatfiles;
 
 def RePackArchiveFile(infile, outfile, compression="auto", compressionlevel=None, followlink=False, seekstart=0, seekend=0, checksumtype="crc32", skipchecksum=False, extradata=[], formatspecs=__file_format_list__, verbose=False, returnfp=False):
@@ -6986,14 +7579,119 @@
     VerbosePrintOut(PrintPermissionString(fmode, ftype) + " " + str(str(fuprint) + "/" + str(fgprint) + " " + str(member.file_size).rjust(15) + " " + member.mtime.strftime('%Y-%m-%d %H:%M') + " " + printfname));
    lcfi = lcfi + 1;
   if(returnfp):
    return listcatfiles['catfp'];
   else:
    return True;
 
+if(not py7zr_support):
+ def SevenZipFileListFiles(infile, verbose=False, returnfp=False):
+  logging.basicConfig(format="%(message)s", stream=sys.stdout, level=logging.DEBUG);
+  if(not os.path.exists(infile) or not os.path.isfile(infile)):
+   return False;
+
+if(py7zr_support):
+ def SevenZipFileListFiles(infile, verbose=False, returnfp=False):
+  logging.basicConfig(format="%(message)s", stream=sys.stdout, level=logging.DEBUG);
+  if(not os.path.exists(infile) or not os.path.isfile(infile)):
+   return False;
+  lcfi = 0;
+  returnval = {};
+  szpfp = py7zr.SevenZipFile(infile, mode="r");
+  file_content = szpfp.readall();
+  #sztest = szpfp.testzip();
+  sztestalt = szpfp.test();
+  if(sztestalt):
+   VerbosePrintOut("Bad file found!");
+  for member in sorted(szpfp.list(), key=lambda x: x.filename):
+   if(re.findall("^[.|/]", member.filename)):
+    fname = member.filename;
+   else:
+    fname = "./"+member.filename;
+   if(not member.is_directory):
+    fpremode = int(stat.S_IFREG + 438);
+   elif(member.is_directory):
+    fpremode = int(stat.S_IFDIR + 511);
+   fwinattributes = int(0);
+   if(member.is_directory):
+    fmode = int(stat.S_IFDIR + 511);
+    fchmode = int(stat.S_IMODE(int(stat.S_IFDIR + 511)));
+    ftypemod = int(stat.S_IFMT(int(stat.S_IFDIR + 511)));
+   else:
+    fmode = int(stat.S_IFLNK + 438);
+    fchmode = int(stat.S_IMODE(int(stat.S_IFLNK + 438)));
+    ftypemod = int(stat.S_IFMT(int(stat.S_IFLNK + 438)));
+   returnval.update({lcfi: member.filename});
+   if(not verbose):
+    VerbosePrintOut(member.filename);
+   if(verbose):
+    permissions = { 'access': { '0': ('---'), '1': ('--x'), '2': ('-w-'), '3': ('-wx'), '4': ('r--'), '5': ('r-x'), '6': ('rw-'), '7': ('rwx') }, 'roles': { 0: 'owner', 1: 'group', 2: 'other' } };
+    permissionstr = "";
+    for fmodval in str(oct(fmode))[-3:]:
+     permissionstr = permissionstr + permissions['access'].get(fmodval, '---');
+    fsize = int("0");
+    if(not member.is_directory):
+     ftype = 0;
+     permissionstr = "-" + permissionstr;
+     printfname = member.filename;
+    elif(member.is_directory):
+     ftype = 5;
+     permissionstr = "d" + permissionstr;
+     printfname = member.filename;
+    if(ftype==0):
+     fsize = len(file_content[member.filename].read());
+     file_content[member.filename].close();
+    try:
+     fuid = int(os.getuid());
+    except AttributeError:
+     fuid = int(0);
+    except KeyError:
+     fuid = int(0);
+    try:
+     fgid = int(os.getgid());
+    except AttributeError:
+     fgid = int(0);
+    except KeyError:
+     fgid = int(0);
+    try:
+     import pwd;
+     try:
+      userinfo = pwd.getpwuid(os.getuid());
+      funame = userinfo.pw_name;
+     except KeyError:
+      funame = "";
+     except AttributeError:
+      funame = "";
+    except ImportError:
+     funame = "";
+    fgname = "";
+    try:
+     import grp;
+     try:
+      groupinfo = grp.getgrgid(os.getgid());
+      fgname = groupinfo.gr_name;
+     except KeyError:
+      fgname = "";
+     except AttributeError:
+      fgname = "";
+    except ImportError:
+     fgname = "";
+    fuprint = funame;
+    if(len(fuprint)<=0):
+     fuprint = str(fuid);
+    fgprint = fgname;
+    if(len(fgprint)<=0):
+     fgprint = str(fgid);
+    VerbosePrintOut(PrintPermissionString(fmode, ftype) + " " + str(str(fuprint) + "/" + str(fgprint) + " " + str(fsize).rjust(15) + " " + member.creationtime.strftime('%Y-%m-%d %H:%M') + " " + printfname));
+   lcfi = lcfi + 1;
+  if(returnfp):
+   return listcatfiles['catfp'];
+  else:
+   return True;
+
 def ListDirListFiles(infiles, dirlistfromtxt=False, compression="auto", compressionlevel=None, followlink=False, seekstart=0, seekend=0, skipchecksum=False, checksumtype="crc32", formatspecs=__file_format_list__, verbose=False, returnfp=False):
  outarray = BytesIO();
  packcat = PackArchiveFile(infiles, outarray, dirlistfromtxt, compression, compressionlevel, followlink, checksumtype, formatspecs, False, True);
  listcatfiles = ArchiveFileListFiles(outarray, seekstart, seekend, skipchecksum, formatspecs, verbose, returnfp);
  return listcatfiles;
 
 def ListDirListFilesAlt(infiles, dirlistfromtxt=False, followlink=False, listonly=True, seekstart=0, seekend=0, skipchecksum=False, checksumtype="crc32", formatspecs=__file_format_list__, verbose=False, returnfp=False):
```

### Comparing `PyCatFile-0.7.8/setup.py` & `pycatfile-0.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2016-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2016-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2016-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: setup.py - Last Update: 4/12/2024 Ver. 0.7.8 RC 1 - Author: cooldude2k $
+    $FileInfo: setup.py - Last Update: 4/24/2024 Ver. 0.8.2 RC 1 - Author: cooldude2k $
 '''
 
 import os, re, sys, pkg_resources;
 from setuptools import setup;
 
 verinfofilename = os.path.realpath("."+os.path.sep+os.path.sep+"pycatfile.py");
 verinfofile = open(verinfofilename, "r");
```

