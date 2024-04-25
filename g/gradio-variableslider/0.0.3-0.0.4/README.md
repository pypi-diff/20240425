# Comparing `tmp/gradio_variableslider-0.0.3.tar.gz` & `tmp/gradio_variableslider-0.0.4.tar.gz`

## Comparing `gradio_variableslider-0.0.3.tar` & `gradio_variableslider-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0       74 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.3/backend/gradio_variableslider/__init__.py
--rwxr-xr-x   0        0        0     5220 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.3/backend/gradio_variableslider/variableslider.py
--rwxr-xr-x   0        0        0    20521 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.3/backend/gradio_variableslider/variableslider.pyi
--rwxr-xr-x   0        0        0    56761 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.3/backend/gradio_variableslider/templates/component/index.js
--rwxr-xr-x   0        0        0    15152 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.3/backend/gradio_variableslider/templates/component/style.css
--rwxr-xr-x   0        0        0     1549 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.3/backend/gradio_variableslider/templates/example/index.js
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.3/backend/gradio_variableslider/templates/example/style.css
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.3/demo/__init__.py
--rwxr-xr-x   0        0        0      772 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.3/demo/app.py
--rwxr-xr-x   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.3/demo/css.css
--rwxr-xr-x   0        0        0     8381 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.3/demo/space.py
--rwxr-xr-x   0        0        0      306 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.3/frontend/Example.svelte
--rwxr-xr-x   0        0        0     6549 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.3/frontend/Index.svelte
--rwxr-xr-x   0        0        0    33833 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.3/frontend/package-lock.json
--rwxr-xr-x   0        0        0      446 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.3/frontend/package.json
--rwxr-xr-x   0        0        0       79 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.3/.gitignore
--rwxr-xr-x   0        0        0     7715 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.3/README.md
--rwxr-xr-x   0        0        0     1594 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     8880 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0       74 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.4/backend/gradio_variableslider/__init__.py
+-rwxr-xr-x   0        0        0     5220 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.4/backend/gradio_variableslider/variableslider.py
+-rwxr-xr-x   0        0        0    20521 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.4/backend/gradio_variableslider/variableslider.pyi
+-rwxr-xr-x   0        0        0    56589 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.4/backend/gradio_variableslider/templates/component/index.js
+-rwxr-xr-x   0        0        0    15152 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.4/backend/gradio_variableslider/templates/component/style.css
+-rwxr-xr-x   0        0        0     1549 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.4/backend/gradio_variableslider/templates/example/index.js
+-rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.4/backend/gradio_variableslider/templates/example/style.css
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.4/demo/__init__.py
+-rwxr-xr-x   0        0        0      772 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.4/demo/app.py
+-rwxr-xr-x   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.4/demo/css.css
+-rwxr-xr-x   0        0        0     8381 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.4/demo/space.py
+-rwxr-xr-x   0        0        0      306 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.4/frontend/Example.svelte
+-rwxr-xr-x   0        0        0     6203 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.4/frontend/Index.svelte
+-rwxr-xr-x   0        0        0    33833 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.4/frontend/package-lock.json
+-rwxr-xr-x   0        0        0      446 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.4/frontend/package.json
+-rwxr-xr-x   0        0        0       79 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.4/.gitignore
+-rwxr-xr-x   0        0        0     7715 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.4/README.md
+-rwxr-xr-x   0        0        0     1637 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8880 2020-02-02 00:00:00.000000 gradio_variableslider-0.0.4/PKG-INFO
```

### Comparing `gradio_variableslider-0.0.3/backend/gradio_variableslider/variableslider.py` & `gradio_variableslider-0.0.4/backend/gradio_variableslider/variableslider.py`

 * *Files identical despite different names*

### Comparing `gradio_variableslider-0.0.3/backend/gradio_variableslider/variableslider.pyi` & `gradio_variableslider-0.0.4/backend/gradio_variableslider/variableslider.pyi`

 * *Files identical despite different names*

### Comparing `gradio_variableslider-0.0.3/backend/gradio_variableslider/templates/component/index.js` & `gradio_variableslider-0.0.4/backend/gradio_variableslider/templates/component/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -8,15 +8,15 @@
     get_slot_changes: pt,
     get_spread_update: kt,
     init: yt,
     insert: vt,
     safe_not_equal: qt,
     set_dynamic_element_data: Me,
     set_style: V,
-    toggle_class: B,
+    toggle_class: A,
     transition_in: nt,
     transition_out: it,
     update_slot_base: Ft
 } = window.__gradio__svelte__internal;
 
 function Ct(l) {
     let t, e, n;
@@ -52,35 +52,35 @@
         c() {
             t = ht(
                 /*tag*/
                 l[14]
             ), f && f.c(), Me(
                 /*tag*/
                 l[14]
-            )(t, _), B(
+            )(t, _), A(
                 t,
                 "hidden",
                 /*visible*/
                 l[10] === !1
-            ), B(
+            ), A(
                 t,
                 "padded",
                 /*padding*/
                 l[6]
-            ), B(
+            ), A(
                 t,
                 "border_focus",
                 /*border_mode*/
                 l[5] === "focus"
-            ), B(
+            ), A(
                 t,
                 "border_contrast",
                 /*border_mode*/
                 l[5] === "contrast"
-            ), B(t, "hide-container", ! /*explicit_call*/
+            ), A(t, "hide-container", ! /*explicit_call*/
                 l[8] && ! /*container*/
                 l[9]), V(
                 t,
                 "height",
                 /*get_dimension*/
                 l[15](
                     /*height*/
@@ -152,35 +152,35 @@
                         )
                     },
                     (!n || a & /*elem_classes*/
                         8 && e !== (e = "block " + /*elem_classes*/
                             s[3].join(" ") + " svelte-nl1om8")) && {
                         class: e
                     }
-                ])), B(
+                ])), A(
                     t,
                     "hidden",
                     /*visible*/
                     s[10] === !1
-                ), B(
+                ), A(
                     t,
                     "padded",
                     /*padding*/
                     s[6]
-                ), B(
+                ), A(
                     t,
                     "border_focus",
                     /*border_mode*/
                     s[5] === "focus"
-                ), B(
+                ), A(
                     t,
                     "border_contrast",
                     /*border_mode*/
                     s[5] === "contrast"
-                ), B(t, "hide-container", ! /*explicit_call*/
+                ), A(t, "hide-container", ! /*explicit_call*/
                     s[8] && ! /*container*/
                     s[9]), a & /*height*/
                 1 && V(
                     t,
                     "height",
                     /*get_dimension*/
                     s[15](
@@ -270,56 +270,56 @@
     } = t, {
         elem_classes: s = []
     } = t, {
         variant: a = "solid"
     } = t, {
         border_mode: u = "base"
     } = t, {
-        padding: c = !0
+        padding: d = !0
     } = t, {
         type: k = "normal"
     } = t, {
         test_id: m = void 0
     } = t, {
         explicit_call: y = !1
     } = t, {
         container: S = !0
     } = t, {
         visible: F = !0
     } = t, {
         allow_overflow: N = !0
     } = t, {
-        scale: d = null
+        scale: c = null
     } = t, {
         min_width: r = 0
     } = t, v = k === "fieldset" ? "fieldset" : "div";
     const C = (b) => {
         if (b !== void 0) {
             if (typeof b == "number")
                 return b + "px";
             if (typeof b == "string")
                 return b;
         }
     };
     return l.$$set = (b) => {
-        "height" in b && e(0, f = b.height), "width" in b && e(1, o = b.width), "elem_id" in b && e(2, _ = b.elem_id), "elem_classes" in b && e(3, s = b.elem_classes), "variant" in b && e(4, a = b.variant), "border_mode" in b && e(5, u = b.border_mode), "padding" in b && e(6, c = b.padding), "type" in b && e(16, k = b.type), "test_id" in b && e(7, m = b.test_id), "explicit_call" in b && e(8, y = b.explicit_call), "container" in b && e(9, S = b.container), "visible" in b && e(10, F = b.visible), "allow_overflow" in b && e(11, N = b.allow_overflow), "scale" in b && e(12, d = b.scale), "min_width" in b && e(13, r = b.min_width), "$$scope" in b && e(17, i = b.$$scope);
+        "height" in b && e(0, f = b.height), "width" in b && e(1, o = b.width), "elem_id" in b && e(2, _ = b.elem_id), "elem_classes" in b && e(3, s = b.elem_classes), "variant" in b && e(4, a = b.variant), "border_mode" in b && e(5, u = b.border_mode), "padding" in b && e(6, d = b.padding), "type" in b && e(16, k = b.type), "test_id" in b && e(7, m = b.test_id), "explicit_call" in b && e(8, y = b.explicit_call), "container" in b && e(9, S = b.container), "visible" in b && e(10, F = b.visible), "allow_overflow" in b && e(11, N = b.allow_overflow), "scale" in b && e(12, c = b.scale), "min_width" in b && e(13, r = b.min_width), "$$scope" in b && e(17, i = b.$$scope);
     }, [
         f,
         o,
         _,
         s,
         a,
         u,
-        c,
+        d,
         m,
         y,
         S,
         F,
         N,
-        d,
+        c,
         r,
         v,
         C,
         k,
         i,
         n
     ];
@@ -346,99 +346,99 @@
     }
 }
 const {
     SvelteComponent: Nt,
     attr: Vt,
     create_slot: Mt,
     detach: zt,
-    element: At,
-    get_all_dirty_from_scope: It,
-    get_slot_changes: Pt,
-    init: Tt,
-    insert: Zt,
-    safe_not_equal: Bt,
-    transition_in: Dt,
-    transition_out: Et,
-    update_slot_base: Rt
+    element: It,
+    get_all_dirty_from_scope: Pt,
+    get_slot_changes: Tt,
+    init: Zt,
+    insert: Bt,
+    safe_not_equal: At,
+    transition_in: Et,
+    transition_out: Dt,
+    update_slot_base: Ot
 } = window.__gradio__svelte__internal;
 
-function Ut(l) {
+function Rt(l) {
     let t, e;
     const n = (
             /*#slots*/
             l[1].default
         ),
         i = Mt(
             n,
             l,
             /*$$scope*/
             l[0],
             null
         );
     return {
         c() {
-            t = At("div"), i && i.c(), Vt(t, "class", "svelte-1hnfib2");
+            t = It("div"), i && i.c(), Vt(t, "class", "svelte-1hnfib2");
         },
         m(f, o) {
-            Zt(f, t, o), i && i.m(t, null), e = !0;
+            Bt(f, t, o), i && i.m(t, null), e = !0;
         },
         p(f, [o]) {
             i && i.p && (!e || o & /*$$scope*/
-                1) && Rt(
+                1) && Ot(
                 i,
                 n,
                 f,
                 /*$$scope*/
                 f[0],
-                e ? Pt(
+                e ? Tt(
                     n,
                     /*$$scope*/
                     f[0],
                     o,
                     null
-                ) : It(
+                ) : Pt(
                     /*$$scope*/
                     f[0]
                 ),
                 null
             );
         },
         i(f) {
-            e || (Dt(i, f), e = !0);
+            e || (Et(i, f), e = !0);
         },
         o(f) {
-            Et(i, f), e = !1;
+            Dt(i, f), e = !1;
         },
         d(f) {
             f && zt(t), i && i.d(f);
         }
     };
 }
 
-function Ot(l, t, e) {
+function Ut(l, t, e) {
     let {
         $$slots: n = {},
         $$scope: i
     } = t;
     return l.$$set = (f) => {
         "$$scope" in f && e(0, i = f.$$scope);
     }, [i, n];
 }
 class Xt extends Nt {
     constructor(t) {
-        super(), Tt(this, t, Ot, Ut, Bt, {});
+        super(), Zt(this, t, Ut, Rt, At, {});
     }
 }
 const {
     SvelteComponent: Yt,
     attr: ze,
     check_outros: Gt,
-    create_component: Kt,
-    create_slot: Ht,
-    destroy_component: Jt,
+    create_component: Ht,
+    create_slot: Jt,
+    destroy_component: Kt,
     detach: ge,
     element: Qt,
     empty: Wt,
     get_all_dirty_from_scope: xt,
     get_slot_changes: $t,
     group_outros: el,
     init: tl,
@@ -450,28 +450,28 @@
     text: fl,
     toggle_class: Q,
     transition_in: se,
     transition_out: we,
     update_slot_base: ol
 } = window.__gradio__svelte__internal;
 
-function Ae(l) {
+function Ie(l) {
     let t, e;
     return t = new Xt({
         props: {
             $$slots: {
                 default: [_l]
             },
             $$scope: {
                 ctx: l
             }
         }
     }), {
         c() {
-            Kt(t.$$.fragment);
+            Ht(t.$$.fragment);
         },
         m(n, i) {
             ll(t, n, i), e = !0;
         },
         p(n, i) {
             const f = {};
             i & /*$$scope, info*/
@@ -483,15 +483,15 @@
         i(n) {
             e || (se(t.$$.fragment, n), e = !0);
         },
         o(n) {
             we(t.$$.fragment, n), e = !1;
         },
         d(n) {
-            Jt(t, n);
+            Kt(t, n);
         }
     };
 }
 
 function _l(l) {
     let t;
     return {
@@ -520,24 +520,24 @@
 
 function al(l) {
     let t, e, n, i;
     const f = (
             /*#slots*/
             l[2].default
         ),
-        o = Ht(
+        o = Jt(
             f,
             l,
             /*$$scope*/
             l[3],
             null
         );
     let _ = (
         /*info*/
-        l[1] && Ae(l)
+        l[1] && Ie(l)
     );
     return {
         c() {
             t = Qt("span"), o && o.c(), e = sl(), _ && _.c(), n = Wt(), ze(t, "data-testid", "block-info"), ze(t, "class", "svelte-22c38v"), Q(t, "sr-only", ! /*show_label*/
                 l[0]), Q(t, "hide", ! /*show_label*/
                 l[0]), Q(
                 t,
@@ -576,15 +576,15 @@
                     2) && Q(
                     t,
                     "has-info",
                     /*info*/
                     s[1] != null
                 ), /*info*/
                 s[1] ? _ ? (_.p(s, a), a & /*info*/
-                    2 && se(_, 1)) : (_ = Ae(s), _.c(), se(_, 1), _.m(n.parentNode, n)) : _ && (el(), we(_, 1, 1, () => {
+                    2 && se(_, 1)) : (_ = Ie(s), _.c(), se(_, 1), _.m(n.parentNode, n)) : _ && (el(), we(_, 1, 1, () => {
                     _ = null;
                 }), Gt());
         },
         i(s) {
             i || (se(o, s), se(_), i = !0);
         },
         o(s) {
@@ -654,15 +654,15 @@
         primary: 500,
         secondary: 100
     }, {
         color: "pink",
         primary: 600,
         secondary: 100
     }],
-    Ie = {
+    Pe = {
         inherit: "inherit",
         current: "currentColor",
         transparent: "transparent",
         black: "#000",
         white: "#fff",
         slate: {
             50: "#f8fafc",
@@ -955,56 +955,56 @@
     (l, {
         color: t,
         primary: e,
         secondary: n
     }) => ({
         ...l,
         [t]: {
-            primary: Ie[t][e],
-            secondary: Ie[t][n]
+            primary: Pe[t][e],
+            secondary: Pe[t][n]
         }
     }), {}
 );
 
-function $(l) {
+function x(l) {
     let t = ["", "k", "M", "G", "T", "P", "E", "Z"],
         e = 0;
     for (; l > 1e3 && e < t.length - 1;)
         l /= 1e3, e++;
     let n = t[e];
     return (Number.isInteger(l) ? l : l.toFixed(1)) + n;
 }
 
 function pe() {}
 
 function dl(l, t) {
     return l != l ? t == t : l !== t || l && typeof l == "object" || typeof l == "function";
 }
 const st = typeof window < "u";
-let Pe = st ? () => window.performance.now() : () => Date.now(),
+let Te = st ? () => window.performance.now() : () => Date.now(),
     ft = st ? (l) => requestAnimationFrame(l) : pe;
-const ee = /* @__PURE__ */ new Set();
+const $ = /* @__PURE__ */ new Set();
 
 function ot(l) {
-    ee.forEach((t) => {
-        t.c(l) || (ee.delete(t), t.f());
-    }), ee.size !== 0 && ft(ot);
+    $.forEach((t) => {
+        t.c(l) || ($.delete(t), t.f());
+    }), $.size !== 0 && ft(ot);
 }
 
 function ml(l) {
     let t;
-    return ee.size === 0 && ft(ot), {
+    return $.size === 0 && ft(ot), {
         promise: new Promise((e) => {
-            ee.add(t = {
+            $.add(t = {
                 c: l,
                 f: e
             });
         }),
         abort() {
-            ee.delete(t);
+            $.delete(t);
         }
     };
 }
 const W = [];
 
 function bl(l, t = pe) {
     let e;
@@ -1036,27 +1036,27 @@
     return {
         set: i,
         update: f,
         subscribe: o
     };
 }
 
-function Te(l) {
+function Ze(l) {
     return Object.prototype.toString.call(l) === "[object Date]";
 }
 
 function qe(l, t, e, n) {
-    if (typeof e == "number" || Te(e)) {
+    if (typeof e == "number" || Ze(e)) {
         const i = n - e,
             f = (e - t) / (l.dt || 1 / 60),
             o = l.opts.stiffness * i,
             _ = l.opts.damping * f,
             s = (o - _) * l.inv_mass,
             a = (f + s) * l.dt;
-        return Math.abs(a) < l.opts.precision && Math.abs(i) < l.opts.precision ? n : (l.settled = !1, Te(e) ? new Date(e.getTime() + a) : e + a);
+        return Math.abs(a) < l.opts.precision && Math.abs(i) < l.opts.precision ? n : (l.settled = !1, Ze(e) ? new Date(e.getTime() + a) : e + a);
     } else {
         if (Array.isArray(e))
             return e.map(
                 (i, f) => qe(l, t[f], e[f], n[f])
             );
         if (typeof e == "object") {
             const i = {};
@@ -1064,45 +1064,45 @@
                 i[f] = qe(l, t[f], e[f], n[f]);
             return i;
         } else
             throw new Error(`Cannot spring ${typeof e} values`);
     }
 }
 
-function Ze(l, t = {}) {
+function Be(l, t = {}) {
     const e = bl(l),
         {
             stiffness: n = 0.15,
             damping: i = 0.8,
             precision: f = 0.01
         } = t;
     let o, _, s, a = l,
         u = l,
-        c = 1,
+        d = 1,
         k = 0,
         m = !1;
 
     function y(F, N = {}) {
         u = F;
-        const d = s = {};
-        return l == null || N.hard || S.stiffness >= 1 && S.damping >= 1 ? (m = !0, o = Pe(), a = F, e.set(l = u), Promise.resolve()) : (N.soft && (k = 1 / ((N.soft === !0 ? 0.5 : +N.soft) * 60), c = 0), _ || (o = Pe(), m = !1, _ = ml((r) => {
+        const c = s = {};
+        return l == null || N.hard || S.stiffness >= 1 && S.damping >= 1 ? (m = !0, o = Te(), a = F, e.set(l = u), Promise.resolve()) : (N.soft && (k = 1 / ((N.soft === !0 ? 0.5 : +N.soft) * 60), d = 0), _ || (o = Te(), m = !1, _ = ml((r) => {
             if (m)
                 return m = !1, _ = null, !1;
-            c = Math.min(c + k, 1);
+            d = Math.min(d + k, 1);
             const v = {
-                    inv_mass: c,
+                    inv_mass: d,
                     opts: S,
                     settled: !0,
                     dt: (r - o) * 60 / 1e3
                 },
                 C = qe(v, a, l, u);
             return o = r, a = l, e.set(l = C), v.settled && (_ = null), !v.settled;
         })), new Promise((r) => {
             _.promise.then(() => {
-                d === s && r();
+                c === s && r();
             });
         }));
     }
     const S = {
         set: y,
         update: (F, N) => y(F(u, l), N),
         subscribe: e.subscribe,
@@ -1110,312 +1110,312 @@
         damping: i,
         precision: f
     };
     return S;
 }
 const {
     SvelteComponent: gl,
-    append: A,
+    append: I,
     attr: q,
-    component_subscribe: Be,
+    component_subscribe: Ae,
     detach: hl,
     element: wl,
     init: pl,
     insert: kl,
-    noop: De,
+    noop: Ee,
     safe_not_equal: yl,
     set_style: ce,
-    svg_element: I,
-    toggle_class: Ee
+    svg_element: P,
+    toggle_class: De
 } = window.__gradio__svelte__internal, {
     onMount: vl
 } = window.__gradio__svelte__internal;
 
 function ql(l) {
-    let t, e, n, i, f, o, _, s, a, u, c, k;
+    let t, e, n, i, f, o, _, s, a, u, d, k;
     return {
         c() {
-            t = wl("div"), e = I("svg"), n = I("g"), i = I("path"), f = I("path"), o = I("path"), _ = I("path"), s = I("g"), a = I("path"), u = I("path"), c = I("path"), k = I("path"), q(i, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), q(i, "fill", "#FF7C00"), q(i, "fill-opacity", "0.4"), q(i, "class", "svelte-43sxxs"), q(f, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), q(f, "fill", "#FF7C00"), q(f, "class", "svelte-43sxxs"), q(o, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), q(o, "fill", "#FF7C00"), q(o, "fill-opacity", "0.4"), q(o, "class", "svelte-43sxxs"), q(_, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), q(_, "fill", "#FF7C00"), q(_, "class", "svelte-43sxxs"), ce(n, "transform", "translate(" + /*$top*/
+            t = wl("div"), e = P("svg"), n = P("g"), i = P("path"), f = P("path"), o = P("path"), _ = P("path"), s = P("g"), a = P("path"), u = P("path"), d = P("path"), k = P("path"), q(i, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), q(i, "fill", "#FF7C00"), q(i, "fill-opacity", "0.4"), q(i, "class", "svelte-43sxxs"), q(f, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), q(f, "fill", "#FF7C00"), q(f, "class", "svelte-43sxxs"), q(o, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), q(o, "fill", "#FF7C00"), q(o, "fill-opacity", "0.4"), q(o, "class", "svelte-43sxxs"), q(_, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), q(_, "fill", "#FF7C00"), q(_, "class", "svelte-43sxxs"), ce(n, "transform", "translate(" + /*$top*/
                 l[1][0] + "px, " + /*$top*/
-                l[1][1] + "px)"), q(a, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), q(a, "fill", "#FF7C00"), q(a, "fill-opacity", "0.4"), q(a, "class", "svelte-43sxxs"), q(u, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), q(u, "fill", "#FF7C00"), q(u, "class", "svelte-43sxxs"), q(c, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), q(c, "fill", "#FF7C00"), q(c, "fill-opacity", "0.4"), q(c, "class", "svelte-43sxxs"), q(k, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), q(k, "fill", "#FF7C00"), q(k, "class", "svelte-43sxxs"), ce(s, "transform", "translate(" + /*$bottom*/
+                l[1][1] + "px)"), q(a, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), q(a, "fill", "#FF7C00"), q(a, "fill-opacity", "0.4"), q(a, "class", "svelte-43sxxs"), q(u, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), q(u, "fill", "#FF7C00"), q(u, "class", "svelte-43sxxs"), q(d, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), q(d, "fill", "#FF7C00"), q(d, "fill-opacity", "0.4"), q(d, "class", "svelte-43sxxs"), q(k, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), q(k, "fill", "#FF7C00"), q(k, "class", "svelte-43sxxs"), ce(s, "transform", "translate(" + /*$bottom*/
                 l[2][0] + "px, " + /*$bottom*/
-                l[2][1] + "px)"), q(e, "viewBox", "-1200 -1200 3000 3000"), q(e, "fill", "none"), q(e, "xmlns", "http://www.w3.org/2000/svg"), q(e, "class", "svelte-43sxxs"), q(t, "class", "svelte-43sxxs"), Ee(
+                l[2][1] + "px)"), q(e, "viewBox", "-1200 -1200 3000 3000"), q(e, "fill", "none"), q(e, "xmlns", "http://www.w3.org/2000/svg"), q(e, "class", "svelte-43sxxs"), q(t, "class", "svelte-43sxxs"), De(
                 t,
                 "margin",
                 /*margin*/
                 l[0]
             );
         },
         m(m, y) {
-            kl(m, t, y), A(t, e), A(e, n), A(n, i), A(n, f), A(n, o), A(n, _), A(e, s), A(s, a), A(s, u), A(s, c), A(s, k);
+            kl(m, t, y), I(t, e), I(e, n), I(n, i), I(n, f), I(n, o), I(n, _), I(e, s), I(s, a), I(s, u), I(s, d), I(s, k);
         },
         p(m, [y]) {
             y & /*$top*/
                 2 && ce(n, "transform", "translate(" + /*$top*/
                     m[1][0] + "px, " + /*$top*/
                     m[1][1] + "px)"), y & /*$bottom*/
                 4 && ce(s, "transform", "translate(" + /*$bottom*/
                     m[2][0] + "px, " + /*$bottom*/
                     m[2][1] + "px)"), y & /*margin*/
-                1 && Ee(
+                1 && De(
                     t,
                     "margin",
                     /*margin*/
                     m[0]
                 );
         },
-        i: De,
-        o: De,
+        i: Ee,
+        o: Ee,
         d(m) {
             m && hl(t);
         }
     };
 }
 
 function Fl(l, t, e) {
     let n, i, {
         margin: f = !0
     } = t;
-    const o = Ze([0, 0]);
-    Be(l, o, (k) => e(1, n = k));
-    const _ = Ze([0, 0]);
-    Be(l, _, (k) => e(2, i = k));
+    const o = Be([0, 0]);
+    Ae(l, o, (k) => e(1, n = k));
+    const _ = Be([0, 0]);
+    Ae(l, _, (k) => e(2, i = k));
     let s;
     async function a() {
         await Promise.all([o.set([125, 140]), _.set([-125, -140])]), await Promise.all([o.set([-125, 140]), _.set([125, -140])]), await Promise.all([o.set([-125, 0]), _.set([125, -0])]), await Promise.all([o.set([125, 0]), _.set([-125, 0])]);
     }
     async function u() {
         await a(), s || u();
     }
-    async function c() {
+    async function d() {
         await Promise.all([o.set([125, 0]), _.set([-125, 0])]), u();
     }
-    return vl(() => (c(), () => s = !0)), l.$$set = (k) => {
+    return vl(() => (d(), () => s = !0)), l.$$set = (k) => {
         "margin" in k && e(0, f = k.margin);
     }, [f, n, i, o, _];
 }
 class Cl extends gl {
     constructor(t) {
         super(), pl(this, t, Fl, ql, yl, {
             margin: 0
         });
     }
 }
 const {
     SvelteComponent: Ll,
-    append: H,
-    attr: D,
-    binding_callbacks: Re,
+    append: J,
+    attr: E,
+    binding_callbacks: Oe,
     check_outros: _t,
     create_component: Sl,
     create_slot: jl,
     destroy_component: Nl,
     destroy_each: at,
     detach: w,
-    element: O,
-    empty: ne,
+    element: U,
+    empty: le,
     ensure_array_like: ke,
     get_all_dirty_from_scope: Vl,
     get_slot_changes: Ml,
     group_outros: rt,
     init: zl,
     insert: p,
-    mount_component: Al,
+    mount_component: Il,
     noop: Fe,
-    safe_not_equal: Il,
+    safe_not_equal: Pl,
     set_data: z,
     set_style: Y,
-    space: E,
+    space: D,
     text: j,
     toggle_class: M,
-    transition_in: te,
-    transition_out: le,
-    update_slot_base: Pl
+    transition_in: ee,
+    transition_out: te,
+    update_slot_base: Tl
 } = window.__gradio__svelte__internal, {
-    tick: Tl
+    tick: Zl
 } = window.__gradio__svelte__internal, {
-    onDestroy: Zl
-} = window.__gradio__svelte__internal, Bl = (l) => ({}), Ue = (l) => ({});
+    onDestroy: Bl
+} = window.__gradio__svelte__internal, Al = (l) => ({}), Re = (l) => ({});
 
-function Oe(l, t, e) {
+function Ue(l, t, e) {
     const n = l.slice();
     return n[38] = t[e], n[40] = e, n;
 }
 
 function Xe(l, t, e) {
     const n = l.slice();
     return n[38] = t[e], n;
 }
 
-function Dl(l) {
+function El(l) {
     let t, e = (
             /*i18n*/
             l[1]("common.error") + ""
         ),
         n, i, f;
     const o = (
             /*#slots*/
             l[29].error
         ),
         _ = jl(
             o,
             l,
             /*$$scope*/
             l[28],
-            Ue
+            Re
         );
     return {
         c() {
-            t = O("span"), n = j(e), i = E(), _ && _.c(), D(t, "class", "error svelte-1yserjw");
+            t = U("span"), n = j(e), i = D(), _ && _.c(), E(t, "class", "error svelte-1yserjw");
         },
         m(s, a) {
-            p(s, t, a), H(t, n), p(s, i, a), _ && _.m(s, a), f = !0;
+            p(s, t, a), J(t, n), p(s, i, a), _ && _.m(s, a), f = !0;
         },
         p(s, a) {
             (!f || a[0] & /*i18n*/
                 2) && e !== (e = /*i18n*/
                 s[1]("common.error") + "") && z(n, e), _ && _.p && (!f || a[0] & /*$$scope*/
-                268435456) && Pl(
+                268435456) && Tl(
                 _,
                 o,
                 s,
                 /*$$scope*/
                 s[28],
                 f ? Ml(
                     o,
                     /*$$scope*/
                     s[28],
                     a,
-                    Bl
+                    Al
                 ) : Vl(
                     /*$$scope*/
                     s[28]
                 ),
-                Ue
+                Re
             );
         },
         i(s) {
-            f || (te(_, s), f = !0);
+            f || (ee(_, s), f = !0);
         },
         o(s) {
-            le(_, s), f = !1;
+            te(_, s), f = !1;
         },
         d(s) {
             s && (w(t), w(i)), _ && _.d(s);
         }
     };
 }
 
-function El(l) {
+function Dl(l) {
     let t, e, n, i, f, o, _, s, a, u = (
         /*variant*/
         l[8] === "default" && /*show_eta_bar*/
         l[18] && /*show_progress*/
         l[6] === "full" && Ye(l)
     );
 
-    function c(r, v) {
+    function d(r, v) {
         if (
             /*progress*/
             r[7]
         )
-            return Ol;
+            return Ul;
         if (
             /*queue_position*/
             r[2] !== null && /*queue_size*/
             r[3] !== void 0 && /*queue_position*/
             r[2] >= 0
         )
-            return Ul;
+            return Rl;
         if (
             /*queue_position*/
             r[2] === 0
         )
-            return Rl;
+            return Ol;
     }
-    let k = c(l),
+    let k = d(l),
         m = k && k(l),
         y = (
             /*timer*/
-            l[5] && He(l)
+            l[5] && Je(l)
         );
-    const S = [Kl, Gl],
+    const S = [Hl, Gl],
         F = [];
 
     function N(r, v) {
         return (
             /*last_progress_level*/
             r[15] != null ? 0 : (
                 /*show_progress*/
                 r[6] === "full" ? 1 : -1
             )
         );
     }
     ~(f = N(l)) && (o = F[f] = S[f](l));
-    let d = ! /*timer*/
+    let c = ! /*timer*/
         l[5] && tt(l);
     return {
         c() {
-            u && u.c(), t = E(), e = O("div"), m && m.c(), n = E(), y && y.c(), i = E(), o && o.c(), _ = E(), d && d.c(), s = ne(), D(e, "class", "progress-text svelte-1yserjw"), M(
+            u && u.c(), t = D(), e = U("div"), m && m.c(), n = D(), y && y.c(), i = D(), o && o.c(), _ = D(), c && c.c(), s = le(), E(e, "class", "progress-text svelte-1yserjw"), M(
                 e,
                 "meta-text-center",
                 /*variant*/
                 l[8] === "center"
             ), M(
                 e,
                 "meta-text",
                 /*variant*/
                 l[8] === "default"
             );
         },
         m(r, v) {
-            u && u.m(r, v), p(r, t, v), p(r, e, v), m && m.m(e, null), H(e, n), y && y.m(e, null), p(r, i, v), ~f && F[f].m(r, v), p(r, _, v), d && d.m(r, v), p(r, s, v), a = !0;
+            u && u.m(r, v), p(r, t, v), p(r, e, v), m && m.m(e, null), J(e, n), y && y.m(e, null), p(r, i, v), ~f && F[f].m(r, v), p(r, _, v), c && c.m(r, v), p(r, s, v), a = !0;
         },
         p(r, v) {
             /*variant*/
             r[8] === "default" && /*show_eta_bar*/
                 r[18] && /*show_progress*/
-                r[6] === "full" ? u ? u.p(r, v) : (u = Ye(r), u.c(), u.m(t.parentNode, t)) : u && (u.d(1), u = null), k === (k = c(r)) && m ? m.p(r, v) : (m && m.d(1), m = k && k(r), m && (m.c(), m.m(e, n))), /*timer*/
-                r[5] ? y ? y.p(r, v) : (y = He(r), y.c(), y.m(e, null)) : y && (y.d(1), y = null), (!a || v[0] & /*variant*/
+                r[6] === "full" ? u ? u.p(r, v) : (u = Ye(r), u.c(), u.m(t.parentNode, t)) : u && (u.d(1), u = null), k === (k = d(r)) && m ? m.p(r, v) : (m && m.d(1), m = k && k(r), m && (m.c(), m.m(e, n))), /*timer*/
+                r[5] ? y ? y.p(r, v) : (y = Je(r), y.c(), y.m(e, null)) : y && (y.d(1), y = null), (!a || v[0] & /*variant*/
                     256) && M(
                     e,
                     "meta-text-center",
                     /*variant*/
                     r[8] === "center"
                 ), (!a || v[0] & /*variant*/
                     256) && M(
                     e,
                     "meta-text",
                     /*variant*/
                     r[8] === "default"
                 );
             let C = f;
-            f = N(r), f === C ? ~f && F[f].p(r, v) : (o && (rt(), le(F[C], 1, 1, () => {
+            f = N(r), f === C ? ~f && F[f].p(r, v) : (o && (rt(), te(F[C], 1, 1, () => {
                     F[C] = null;
-                }), _t()), ~f ? (o = F[f], o ? o.p(r, v) : (o = F[f] = S[f](r), o.c()), te(o, 1), o.m(_.parentNode, _)) : o = null), /*timer*/
-                r[5] ? d && (d.d(1), d = null) : d ? d.p(r, v) : (d = tt(r), d.c(), d.m(s.parentNode, s));
+                }), _t()), ~f ? (o = F[f], o ? o.p(r, v) : (o = F[f] = S[f](r), o.c()), ee(o, 1), o.m(_.parentNode, _)) : o = null), /*timer*/
+                r[5] ? c && (c.d(1), c = null) : c ? c.p(r, v) : (c = tt(r), c.c(), c.m(s.parentNode, s));
         },
         i(r) {
-            a || (te(o), a = !0);
+            a || (ee(o), a = !0);
         },
         o(r) {
-            le(o), a = !1;
+            te(o), a = !1;
         },
         d(r) {
-            r && (w(t), w(e), w(i), w(_), w(s)), u && u.d(r), m && m.d(), y && y.d(), ~f && F[f].d(r), d && d.d(r);
+            r && (w(t), w(e), w(i), w(_), w(s)), u && u.d(r), m && m.d(), y && y.d(), ~f && F[f].d(r), c && c.d(r);
         }
     };
 }
 
 function Ye(l) {
     let t, e = `translateX(${/*eta_level*/
   (l[17] || 0) * 100 - 100}%)`;
     return {
         c() {
-            t = O("div"), D(t, "class", "eta-bar svelte-1yserjw"), Y(t, "transform", e);
+            t = U("div"), E(t, "class", "eta-bar svelte-1yserjw"), Y(t, "transform", e);
         },
         m(n, i) {
             p(n, t, i);
         },
         p(n, i) {
             i[0] & /*eta_level*/
                 131072 && e !== (e = `translateX(${/*eta_level*/
@@ -1423,15 +1423,15 @@
         },
         d(n) {
             n && w(t);
         }
     };
 }
 
-function Rl(l) {
+function Ol(l) {
     let t;
     return {
         c() {
             t = j("processing |");
         },
         m(e, n) {
             p(e, t, n);
@@ -1439,15 +1439,15 @@
         p: Fe,
         d(e) {
             e && w(t);
         }
     };
 }
 
-function Ul(l) {
+function Rl(l) {
     let t, e = (
             /*queue_position*/
             l[2] + 1 + ""
         ),
         n, i, f, o;
     return {
         c() {
@@ -1471,27 +1471,27 @@
         },
         d(_) {
             _ && (w(t), w(n), w(i), w(f), w(o));
         }
     };
 }
 
-function Ol(l) {
+function Ul(l) {
     let t, e = ke(
             /*progress*/
             l[7]
         ),
         n = [];
     for (let i = 0; i < e.length; i += 1)
-        n[i] = Ke(Xe(l, e, i));
+        n[i] = He(Xe(l, e, i));
     return {
         c() {
             for (let i = 0; i < n.length; i += 1)
                 n[i].c();
-            t = ne();
+            t = le();
         },
         m(i, f) {
             for (let o = 0; o < n.length; o += 1)
                 n[o] && n[o].m(i, f);
             p(i, t, f);
         },
         p(i, f) {
@@ -1500,15 +1500,15 @@
                 e = ke(
                     /*progress*/
                     i[7]
                 );
                 let o;
                 for (o = 0; o < e.length; o += 1) {
                     const _ = Xe(i, e, o);
-                    n[o] ? n[o].p(_, f) : (n[o] = Ke(_), n[o].c(), n[o].m(t.parentNode, t));
+                    n[o] ? n[o].p(_, f) : (n[o] = He(_), n[o].c(), n[o].m(t.parentNode, t));
                 }
                 for (; o < n.length; o += 1)
                     n[o].d(1);
                 n.length = e.length;
             }
         },
         d(i) {
@@ -1521,123 +1521,123 @@
     let t, e = (
             /*p*/
             l[38].unit + ""
         ),
         n, i, f = " ",
         o;
 
-    function _(u, c) {
+    function _(u, d) {
         return (
             /*p*/
             u[38].length != null ? Yl : Xl
         );
     }
     let s = _(l),
         a = s(l);
     return {
         c() {
-            a.c(), t = E(), n = j(e), i = j(" | "), o = j(f);
+            a.c(), t = D(), n = j(e), i = j(" | "), o = j(f);
         },
-        m(u, c) {
-            a.m(u, c), p(u, t, c), p(u, n, c), p(u, i, c), p(u, o, c);
+        m(u, d) {
+            a.m(u, d), p(u, t, d), p(u, n, d), p(u, i, d), p(u, o, d);
         },
-        p(u, c) {
-            s === (s = _(u)) && a ? a.p(u, c) : (a.d(1), a = s(u), a && (a.c(), a.m(t.parentNode, t))), c[0] & /*progress*/
+        p(u, d) {
+            s === (s = _(u)) && a ? a.p(u, d) : (a.d(1), a = s(u), a && (a.c(), a.m(t.parentNode, t))), d[0] & /*progress*/
                 128 && e !== (e = /*p*/
                     u[38].unit + "") && z(n, e);
         },
         d(u) {
             u && (w(t), w(n), w(i), w(o)), a.d(u);
         }
     };
 }
 
 function Xl(l) {
-    let t = $(
+    let t = x(
             /*p*/
             l[38].index || 0
         ) + "",
         e;
     return {
         c() {
             e = j(t);
         },
         m(n, i) {
             p(n, e, i);
         },
         p(n, i) {
             i[0] & /*progress*/
-                128 && t !== (t = $(
+                128 && t !== (t = x(
                     /*p*/
                     n[38].index || 0
                 ) + "") && z(e, t);
         },
         d(n) {
             n && w(e);
         }
     };
 }
 
 function Yl(l) {
-    let t = $(
+    let t = x(
             /*p*/
             l[38].index || 0
         ) + "",
-        e, n, i = $(
+        e, n, i = x(
             /*p*/
             l[38].length
         ) + "",
         f;
     return {
         c() {
             e = j(t), n = j("/"), f = j(i);
         },
         m(o, _) {
             p(o, e, _), p(o, n, _), p(o, f, _);
         },
         p(o, _) {
             _[0] & /*progress*/
-                128 && t !== (t = $(
+                128 && t !== (t = x(
                     /*p*/
                     o[38].index || 0
                 ) + "") && z(e, t), _[0] & /*progress*/
-                128 && i !== (i = $(
+                128 && i !== (i = x(
                     /*p*/
                     o[38].length
                 ) + "") && z(f, i);
         },
         d(o) {
             o && (w(e), w(n), w(f));
         }
     };
 }
 
-function Ke(l) {
+function He(l) {
     let t, e = (
         /*p*/
         l[38].index != null && Ge(l)
     );
     return {
         c() {
-            e && e.c(), t = ne();
+            e && e.c(), t = le();
         },
         m(n, i) {
             e && e.m(n, i), p(n, t, i);
         },
         p(n, i) {
             /*p*/
             n[38].index != null ? e ? e.p(n, i) : (e = Ge(n), e.c(), e.m(t.parentNode, t)) : e && (e.d(1), e = null);
         },
         d(n) {
             n && w(t), e && e.d(n);
         }
     };
 }
 
-function He(l) {
+function Je(l) {
     let t, e = (
             /*eta*/
             l[0] ? `/${/*formatted_eta*/
     l[19]}` : ""
         ),
         n, i;
     return {
@@ -1677,75 +1677,75 @@
             )
         }
     }), {
         c() {
             Sl(t.$$.fragment);
         },
         m(n, i) {
-            Al(t, n, i), e = !0;
+            Il(t, n, i), e = !0;
         },
         p(n, i) {
             const f = {};
             i[0] & /*variant*/
                 256 && (f.margin = /*variant*/
                     n[8] === "default"), t.$set(f);
         },
         i(n) {
-            e || (te(t.$$.fragment, n), e = !0);
+            e || (ee(t.$$.fragment, n), e = !0);
         },
         o(n) {
-            le(t.$$.fragment, n), e = !1;
+            te(t.$$.fragment, n), e = !1;
         },
         d(n) {
             Nl(t, n);
         }
     };
 }
 
-function Kl(l) {
+function Hl(l) {
     let t, e, n, i, f, o = `${/*last_progress_level*/
   l[15] * 100}%`,
         _ = (
             /*progress*/
-            l[7] != null && Je(l)
+            l[7] != null && Ke(l)
         );
     return {
         c() {
-            t = O("div"), e = O("div"), _ && _.c(), n = E(), i = O("div"), f = O("div"), D(e, "class", "progress-level-inner svelte-1yserjw"), D(f, "class", "progress-bar svelte-1yserjw"), Y(f, "width", o), D(i, "class", "progress-bar-wrap svelte-1yserjw"), D(t, "class", "progress-level svelte-1yserjw");
+            t = U("div"), e = U("div"), _ && _.c(), n = D(), i = U("div"), f = U("div"), E(e, "class", "progress-level-inner svelte-1yserjw"), E(f, "class", "progress-bar svelte-1yserjw"), Y(f, "width", o), E(i, "class", "progress-bar-wrap svelte-1yserjw"), E(t, "class", "progress-level svelte-1yserjw");
         },
         m(s, a) {
-            p(s, t, a), H(t, e), _ && _.m(e, null), H(t, n), H(t, i), H(i, f), l[30](f);
+            p(s, t, a), J(t, e), _ && _.m(e, null), J(t, n), J(t, i), J(i, f), l[30](f);
         },
         p(s, a) {
             /*progress*/
-            s[7] != null ? _ ? _.p(s, a) : (_ = Je(s), _.c(), _.m(e, null)) : _ && (_.d(1), _ = null), a[0] & /*last_progress_level*/
+            s[7] != null ? _ ? _.p(s, a) : (_ = Ke(s), _.c(), _.m(e, null)) : _ && (_.d(1), _ = null), a[0] & /*last_progress_level*/
                 32768 && o !== (o = `${/*last_progress_level*/
       s[15] * 100}%`) && Y(f, "width", o);
         },
         i: Fe,
         o: Fe,
         d(s) {
             s && w(t), _ && _.d(), l[30](null);
         }
     };
 }
 
-function Je(l) {
+function Ke(l) {
     let t, e = ke(
             /*progress*/
             l[7]
         ),
         n = [];
     for (let i = 0; i < e.length; i += 1)
-        n[i] = et(Oe(l, e, i));
+        n[i] = et(Ue(l, e, i));
     return {
         c() {
             for (let i = 0; i < n.length; i += 1)
                 n[i].c();
-            t = ne();
+            t = le();
         },
         m(i, f) {
             for (let o = 0; o < n.length; o += 1)
                 n[o] && n[o].m(i, f);
             p(i, t, f);
         },
         p(i, f) {
@@ -1753,15 +1753,15 @@
                 16512) {
                 e = ke(
                     /*progress*/
                     i[7]
                 );
                 let o;
                 for (o = 0; o < e.length; o += 1) {
-                    const _ = Oe(i, e, o);
+                    const _ = Ue(i, e, o);
                     n[o] ? n[o].p(_, f) : (n[o] = et(_), n[o].c(), n[o].m(t.parentNode, t));
                 }
                 for (; o < n.length; o += 1)
                     n[o].d(1);
                 n.length = e.length;
             }
         },
@@ -1770,15 +1770,15 @@
         }
     };
 }
 
 function Qe(l) {
     let t, e, n, i, f = (
             /*i*/
-            l[40] !== 0 && Hl()
+            l[40] !== 0 && Jl()
         ),
         o = (
             /*p*/
             l[38].desc != null && We(l)
         ),
         _ = (
             /*p*/
@@ -1791,15 +1791,15 @@
         ),
         s = (
             /*progress_level*/
             l[14] != null && $e(l)
         );
     return {
         c() {
-            f && f.c(), t = E(), o && o.c(), e = E(), _ && _.c(), n = E(), s && s.c(), i = ne();
+            f && f.c(), t = D(), o && o.c(), e = D(), _ && _.c(), n = D(), s && s.c(), i = le();
         },
         m(a, u) {
             f && f.m(a, u), p(a, t, u), o && o.m(a, u), p(a, e, u), _ && _.m(a, u), p(a, n, u), s && s.m(a, u), p(a, i, u);
         },
         p(a, u) {
             /*p*/
             a[38].desc != null ? o ? o.p(a, u) : (o = We(a), o.c(), o.m(e.parentNode, e)) : o && (o.d(1), o = null), /*p*/
@@ -1813,15 +1813,15 @@
         },
         d(a) {
             a && (w(t), w(e), w(n), w(i)), f && f.d(a), o && o.d(a), _ && _.d(a), s && s.d(a);
         }
     };
 }
 
-function Hl(l) {
+function Jl(l) {
     let t;
     return {
         c() {
             t = j(" /");
         },
         m(e, n) {
             p(e, t, n);
@@ -1907,15 +1907,15 @@
             l[14][
                 /*i*/
                 l[40]
             ] != null) && Qe(l)
     );
     return {
         c() {
-            e && e.c(), t = ne();
+            e && e.c(), t = le();
         },
         m(n, i) {
             e && e.m(n, i), p(n, t, i);
         },
         p(n, i) {
             /*p*/
             n[38].desc != null || /*progress_level*/
@@ -1931,21 +1931,21 @@
     };
 }
 
 function tt(l) {
     let t, e;
     return {
         c() {
-            t = O("p"), e = j(
+            t = U("p"), e = j(
                 /*loading_text*/
                 l[9]
-            ), D(t, "class", "loading svelte-1yserjw");
+            ), E(t, "class", "loading svelte-1yserjw");
         },
         m(n, i) {
-            p(n, t, i), H(t, e);
+            p(n, t, i), J(t, e);
         },
         p(n, i) {
             i[0] & /*loading_text*/
                 512 && z(
                     e,
                     /*loading_text*/
                     n[9]
@@ -1953,31 +1953,31 @@
         },
         d(n) {
             n && w(t);
         }
     };
 }
 
-function Jl(l) {
+function Kl(l) {
     let t, e, n, i, f;
-    const o = [El, Dl],
+    const o = [Dl, El],
         _ = [];
 
     function s(a, u) {
         return (
             /*status*/
             a[4] === "pending" ? 0 : (
                 /*status*/
                 a[4] === "error" ? 1 : -1
             )
         );
     }
     return ~(e = s(l)) && (n = _[e] = o[e](l)), {
         c() {
-            t = O("div"), n && n.c(), D(t, "class", i = "wrap " + /*variant*/
+            t = U("div"), n && n.c(), E(t, "class", i = "wrap " + /*variant*/
                 l[8] + " " + /*show_progress*/
                 l[6] + " svelte-1yserjw"), M(t, "hide", ! /*status*/
                 l[4] || /*status*/
                 l[4] === "complete" || /*show_progress*/
                 l[6] === "hidden"), M(
                 t,
                 "translucent",
@@ -2009,21 +2009,21 @@
                 l[10] ? "0" : "var(--size-8) 0"
             );
         },
         m(a, u) {
             p(a, t, u), ~e && _[e].m(t, null), l[31](t), f = !0;
         },
         p(a, u) {
-            let c = e;
-            e = s(a), e === c ? ~e && _[e].p(a, u) : (n && (rt(), le(_[c], 1, 1, () => {
-                    _[c] = null;
-                }), _t()), ~e ? (n = _[e], n ? n.p(a, u) : (n = _[e] = o[e](a), n.c()), te(n, 1), n.m(t, null)) : n = null), (!f || u[0] & /*variant, show_progress*/
+            let d = e;
+            e = s(a), e === d ? ~e && _[e].p(a, u) : (n && (rt(), te(_[d], 1, 1, () => {
+                    _[d] = null;
+                }), _t()), ~e ? (n = _[e], n ? n.p(a, u) : (n = _[e] = o[e](a), n.c()), ee(n, 1), n.m(t, null)) : n = null), (!f || u[0] & /*variant, show_progress*/
                     320 && i !== (i = "wrap " + /*variant*/
                         a[8] + " " + /*show_progress*/
-                        a[6] + " svelte-1yserjw")) && D(t, "class", i), (!f || u[0] & /*variant, show_progress, status, show_progress*/
+                        a[6] + " svelte-1yserjw")) && E(t, "class", i), (!f || u[0] & /*variant, show_progress, status, show_progress*/
                     336) && M(t, "hide", ! /*status*/
                     a[4] || /*status*/
                     a[4] === "complete" || /*show_progress*/
                     a[6] === "hidden"), (!f || u[0] & /*variant, show_progress, variant, status, translucent, show_progress*/
                     2384) && M(
                     t,
                     "translucent",
@@ -2056,33 +2056,33 @@
                     t,
                     "padding",
                     /*absolute*/
                     a[10] ? "0" : "var(--size-8) 0"
                 );
         },
         i(a) {
-            f || (te(n), f = !0);
+            f || (ee(n), f = !0);
         },
         o(a) {
-            le(n), f = !1;
+            te(n), f = !1;
         },
         d(a) {
             a && w(t), ~e && _[e].d(), l[31](null);
         }
     };
 }
 let de = [],
     ye = !1;
 async function Ql(l, t = !0) {
     if (!(window.__gradio_mode__ === "website" || window.__gradio_mode__ !== "app" && t !== !0)) {
         if (de.push(l), !ye)
             ye = !0;
         else
             return;
-        await Tl(), requestAnimationFrame(() => {
+        await Zl(), requestAnimationFrame(() => {
             let e = [0, 0];
             for (let n = 0; n < de.length; n++) {
                 const f = de[n].getBoundingClientRect();
                 (n === 0 || f.top + window.scrollY <= e[0]) && (e[0] = f.top + window.scrollY, e[1] = n);
             }
             window.scrollTo({
                 top: e[0] - 20,
@@ -2109,15 +2109,15 @@
         {
             queue_size: a
         } = t,
         {
             status: u
         } = t,
         {
-            scroll_to_output: c = !1
+            scroll_to_output: d = !1
         } = t,
         {
             timer: k = !0
         } = t,
         {
             show_progress: m = "full"
         } = t,
@@ -2130,123 +2130,123 @@
         {
             variant: F = "default"
         } = t,
         {
             loading_text: N = "Loading..."
         } = t,
         {
-            absolute: d = !0
+            absolute: c = !0
         } = t,
         {
             translucent: r = !1
         } = t,
         {
             border: v = !1
         } = t,
         {
             autoscroll: C
         } = t,
         b, G = !1,
-        J = 0,
-        R = 0,
+        K = 0,
+        O = 0,
         X = null,
-        P = null,
+        T = null,
         _e = 0,
-        U = null,
-        K, T = null,
+        R = null,
+        H, Z = null,
         ae = !0;
     const g = () => {
-        e(0, _ = e(26, X = e(19, ue = null))), e(24, J = performance.now()), e(25, R = 0), G = !0, Z();
+        e(0, _ = e(26, X = e(19, ue = null))), e(24, K = performance.now()), e(25, O = 0), G = !0, B();
     };
 
-    function Z() {
+    function B() {
         requestAnimationFrame(() => {
-            e(25, R = (performance.now() - J) / 1e3), G && Z();
+            e(25, O = (performance.now() - K) / 1e3), G && B();
         });
     }
 
     function re() {
-        e(25, R = 0), e(0, _ = e(26, X = e(19, ue = null))), G && (G = !1);
+        e(25, O = 0), e(0, _ = e(26, X = e(19, ue = null))), G && (G = !1);
     }
-    Zl(() => {
+    Bl(() => {
         G && re();
     });
     let ue = null;
 
     function ut(h) {
-        Re[h ? "unshift" : "push"](() => {
-            T = h, e(16, T), e(7, S), e(14, U), e(15, K);
+        Oe[h ? "unshift" : "push"](() => {
+            Z = h, e(16, Z), e(7, S), e(14, R), e(15, H);
         });
     }
 
     function ct(h) {
-        Re[h ? "unshift" : "push"](() => {
+        Oe[h ? "unshift" : "push"](() => {
             b = h, e(13, b);
         });
     }
     return l.$$set = (h) => {
-        "i18n" in h && e(1, o = h.i18n), "eta" in h && e(0, _ = h.eta), "queue_position" in h && e(2, s = h.queue_position), "queue_size" in h && e(3, a = h.queue_size), "status" in h && e(4, u = h.status), "scroll_to_output" in h && e(21, c = h.scroll_to_output), "timer" in h && e(5, k = h.timer), "show_progress" in h && e(6, m = h.show_progress), "message" in h && e(22, y = h.message), "progress" in h && e(7, S = h.progress), "variant" in h && e(8, F = h.variant), "loading_text" in h && e(9, N = h.loading_text), "absolute" in h && e(10, d = h.absolute), "translucent" in h && e(11, r = h.translucent), "border" in h && e(12, v = h.border), "autoscroll" in h && e(23, C = h.autoscroll), "$$scope" in h && e(28, f = h.$$scope);
+        "i18n" in h && e(1, o = h.i18n), "eta" in h && e(0, _ = h.eta), "queue_position" in h && e(2, s = h.queue_position), "queue_size" in h && e(3, a = h.queue_size), "status" in h && e(4, u = h.status), "scroll_to_output" in h && e(21, d = h.scroll_to_output), "timer" in h && e(5, k = h.timer), "show_progress" in h && e(6, m = h.show_progress), "message" in h && e(22, y = h.message), "progress" in h && e(7, S = h.progress), "variant" in h && e(8, F = h.variant), "loading_text" in h && e(9, N = h.loading_text), "absolute" in h && e(10, c = h.absolute), "translucent" in h && e(11, r = h.translucent), "border" in h && e(12, v = h.border), "autoscroll" in h && e(23, C = h.autoscroll), "$$scope" in h && e(28, f = h.$$scope);
     }, l.$$.update = () => {
         l.$$.dirty[0] & /*eta, old_eta, timer_start, eta_from_start*/
-            218103809 && (_ === null && e(0, _ = X), _ != null && X !== _ && (e(27, P = (performance.now() - J) / 1e3 + _), e(19, ue = P.toFixed(1)), e(26, X = _))), l.$$.dirty[0] & /*eta_from_start, timer_diff*/
-            167772160 && e(17, _e = P === null || P <= 0 || !R ? null : Math.min(R / P, 1)), l.$$.dirty[0] & /*progress*/
+            218103809 && (_ === null && e(0, _ = X), _ != null && X !== _ && (e(27, T = (performance.now() - K) / 1e3 + _), e(19, ue = T.toFixed(1)), e(26, X = _))), l.$$.dirty[0] & /*eta_from_start, timer_diff*/
+            167772160 && e(17, _e = T === null || T <= 0 || !O ? null : Math.min(O / T, 1)), l.$$.dirty[0] & /*progress*/
             128 && S != null && e(18, ae = !1), l.$$.dirty[0] & /*progress, progress_level, progress_bar, last_progress_level*/
-            114816 && (S != null ? e(14, U = S.map((h) => {
+            114816 && (S != null ? e(14, R = S.map((h) => {
                 if (h.index != null && h.length != null)
                     return h.index / h.length;
                 if (h.progress != null)
                     return h.progress;
-            })) : e(14, U = null), U ? (e(15, K = U[U.length - 1]), T && (K === 0 ? e(16, T.style.transition = "0", T) : e(16, T.style.transition = "150ms", T))) : e(15, K = void 0)), l.$$.dirty[0] & /*status*/
+            })) : e(14, R = null), R ? (e(15, H = R[R.length - 1]), Z && (H === 0 ? e(16, Z.style.transition = "0", Z) : e(16, Z.style.transition = "150ms", Z))) : e(15, H = void 0)), l.$$.dirty[0] & /*status*/
             16 && (u === "pending" ? g() : re()), l.$$.dirty[0] & /*el, scroll_to_output, status, autoscroll*/
-            10493968 && b && c && (u === "pending" || u === "complete") && Ql(b, C), l.$$.dirty[0] & /*status, message*/
+            10493968 && b && d && (u === "pending" || u === "complete") && Ql(b, C), l.$$.dirty[0] & /*status, message*/
             4194320, l.$$.dirty[0] & /*timer_diff*/
-            33554432 && e(20, n = R.toFixed(1));
+            33554432 && e(20, n = O.toFixed(1));
     }, [
         _,
         o,
         s,
         a,
         u,
         k,
         m,
         S,
         F,
         N,
-        d,
+        c,
         r,
         v,
         b,
-        U,
-        K,
-        T,
+        R,
+        H,
+        Z,
         _e,
         ae,
         ue,
         n,
-        c,
+        d,
         y,
         C,
-        J,
-        R,
+        K,
+        O,
         X,
-        P,
+        T,
         f,
         i,
         ut,
         ct
     ];
 }
 class xl extends Ll {
     constructor(t) {
         super(), zl(
             this,
             t,
             Wl,
-            Jl,
-            Il, {
+            Kl,
+            Pl, {
                 i18n: 1,
                 eta: 0,
                 queue_position: 2,
                 queue_size: 3,
                 status: 4,
                 scroll_to_output: 21,
                 timer: 5,
@@ -2270,20 +2270,20 @@
     append: me,
     assign: en,
     attr: L,
     binding_callbacks: lt,
     create_component: Ce,
     destroy_component: Le,
     detach: fe,
-    element: ie,
+    element: ne,
     get_spread_object: tn,
     get_spread_update: ln,
     init: nn,
     insert: oe,
-    listen: x,
+    listen: ie,
     mount_component: Se,
     run_all: sn,
     safe_not_equal: fn,
     set_data: on,
     set_input_value: be,
     space: ve,
     text: _n,
@@ -2317,15 +2317,15 @@
         d(e) {
             e && fe(t);
         }
     };
 }
 
 function un(l) {
-    let t, e, n, i, f, o, _, s, a, u, c, k, m, y, S;
+    let t, e, n, i, f, o, _, s, a, u, d, k, m, y, S;
     const F = [{
             autoscroll: (
                 /*gradio*/
                 l[1].autoscroll
             )
         }, {
             i18n: (
@@ -2333,16 +2333,16 @@
                 l[1].i18n
             )
         },
         /*loading_status*/
         l[14]
     ];
     let N = {};
-    for (let d = 0; d < F.length; d += 1)
-        N = en(N, F[d]);
+    for (let c = 0; c < F.length; c += 1)
+        N = en(N, F[c]);
     return t = new xl({
         props: N
     }), o = new ul({
         props: {
             show_label: (
                 /*show_label*/
                 l[13]
@@ -2356,15 +2356,15 @@
             },
             $$scope: {
                 ctx: l
             }
         }
     }), {
         c() {
-            Ce(t.$$.fragment), e = ve(), n = ie("div"), i = ie("div"), f = ie("label"), Ce(o.$$.fragment), _ = ve(), s = ie("input"), u = ve(), c = ie("input"), L(
+            Ce(t.$$.fragment), e = ve(), n = ne("div"), i = ne("div"), f = ne("label"), Ce(o.$$.fragment), _ = ve(), s = ne("input"), u = ve(), d = ne("input"), L(
                     f,
                     "for",
                     /*id*/
                     l[18]
                 ), L(s, "aria-label", a = `number input for ${/*label*/
       l[5]}`), L(s, "data-testid", "number-input"), L(s, "type", "number"), L(
                     s,
@@ -2378,180 +2378,179 @@
                     l[11]
                 ), L(
                     s,
                     "step",
                     /*step*/
                     l[12]
                 ), s.disabled = /*disabled*/
-                l[17], s.readOnly = !0, L(s, "class", "svelte-o2qgeu"), L(i, "class", "head svelte-o2qgeu"), L(n, "class", "wrap svelte-o2qgeu"), L(c, "type", "range"), L(
-                    c,
+                l[17], s.readOnly = !0, L(s, "class", "svelte-o2qgeu"), L(i, "class", "head svelte-o2qgeu"), L(n, "class", "wrap svelte-o2qgeu"), L(d, "type", "range"), L(
+                    d,
                     "id",
                     /*id*/
                     l[18]
-                ), L(c, "name", "cowbell"), L(
-                    c,
+                ), L(d, "name", "cowbell"), L(
+                    d,
                     "min",
                     /*minimum*/
                     l[10]
                 ), L(
-                    c,
+                    d,
                     "max",
                     /*maximum*/
                     l[11]
                 ), L(
-                    c,
+                    d,
                     "step",
                     /*step*/
                     l[12]
-                ), c.disabled = /*disabled*/
-                l[17], L(c, "aria-label", k = `range slider for ${/*label*/
-      l[5]}`), L(c, "class", "svelte-o2qgeu");
+                ), d.disabled = /*disabled*/
+                l[17], L(d, "aria-label", k = `range slider for ${/*label*/
+      l[5]}`), L(d, "class", "svelte-o2qgeu");
         },
-        m(d, r) {
-            Se(t, d, r), oe(d, e, r), oe(d, n, r), me(n, i), me(i, f), Se(o, f, null), me(i, _), me(i, s), be(
+        m(c, r) {
+            Se(t, c, r), oe(c, e, r), oe(c, n, r), me(n, i), me(i, f), Se(o, f, null), me(i, _), me(i, s), be(
                 s,
                 /*value*/
                 l[0]
-            ), l[24](s), oe(d, u, r), oe(d, c, r), be(
-                c,
+            ), l[24](s), oe(c, u, r), oe(c, d, r), be(
+                d,
                 /*value*/
                 l[0]
-            ), l[26](c), m = !0, y || (S = [
-                x(
+            ), l[26](d), m = !0, y || (S = [
+                ie(
                     s,
                     "input",
                     /*input0_input_handler*/
                     l[23]
                 ),
-                x(
+                ie(
                     s,
                     "blur",
                     /*clamp*/
                     l[19]
                 ),
-                x(
-                    c,
+                ie(
+                    d,
                     "change",
                     /*input1_change_input_handler*/
                     l[25]
                 ),
-                x(
-                    c,
+                ie(
+                    d,
                     "input",
                     /*input1_change_input_handler*/
                     l[25]
                 ),
-                x(
-                    c,
+                ie(
+                    d,
                     "input",
                     /*adjustValue*/
                     l[20]
-                ),
-                x(c, "keydown", mn)
+                )
             ], y = !0);
         },
-        p(d, r) {
+        p(c, r) {
             const v = r[0] & /*gradio, loading_status*/
                 16386 ? ln(F, [
                     r[0] & /*gradio*/
                     2 && {
                         autoscroll: (
                             /*gradio*/
-                            d[1].autoscroll
+                            c[1].autoscroll
                         )
                     },
                     r[0] & /*gradio*/
                     2 && {
                         i18n: (
                             /*gradio*/
-                            d[1].i18n
+                            c[1].i18n
                         )
                     },
                     r[0] & /*loading_status*/
                     16384 && tn(
                         /*loading_status*/
-                        d[14]
+                        c[14]
                     )
                 ]) : {};
             t.$set(v);
             const C = {};
             r[0] & /*show_label*/
                 8192 && (C.show_label = /*show_label*/
-                    d[13]), r[0] & /*info*/
+                    c[13]), r[0] & /*info*/
                 64 && (C.info = /*info*/
-                    d[6]), r[0] & /*label*/
+                    c[6]), r[0] & /*label*/
                 32 | r[1] & /*$$scope*/
                 1 && (C.$$scope = {
                     dirty: r,
-                    ctx: d
+                    ctx: c
                 }), o.$set(C), (!m || r[0] & /*label*/
                     32 && a !== (a = `number input for ${/*label*/
-      d[5]}`)) && L(s, "aria-label", a), (!m || r[0] & /*minimum*/
+      c[5]}`)) && L(s, "aria-label", a), (!m || r[0] & /*minimum*/
                     1024) && L(
                     s,
                     "min",
                     /*minimum*/
-                    d[10]
+                    c[10]
                 ), (!m || r[0] & /*maximum*/
                     2048) && L(
                     s,
                     "max",
                     /*maximum*/
-                    d[11]
+                    c[11]
                 ), (!m || r[0] & /*step*/
                     4096) && L(
                     s,
                     "step",
                     /*step*/
-                    d[12]
+                    c[12]
                 ), (!m || r[0] & /*disabled*/
                     131072) && (s.disabled = /*disabled*/
-                    d[17]), r[0] & /*value*/
+                    c[17]), r[0] & /*value*/
                 1 && je(s.value) !== /*value*/
-                d[0] && be(
+                c[0] && be(
                     s,
                     /*value*/
-                    d[0]
+                    c[0]
                 ), (!m || r[0] & /*minimum*/
                     1024) && L(
-                    c,
+                    d,
                     "min",
                     /*minimum*/
-                    d[10]
+                    c[10]
                 ), (!m || r[0] & /*maximum*/
                     2048) && L(
-                    c,
+                    d,
                     "max",
                     /*maximum*/
-                    d[11]
+                    c[11]
                 ), (!m || r[0] & /*step*/
                     4096) && L(
-                    c,
+                    d,
                     "step",
                     /*step*/
-                    d[12]
+                    c[12]
                 ), (!m || r[0] & /*disabled*/
-                    131072) && (c.disabled = /*disabled*/
-                    d[17]), (!m || r[0] & /*label*/
+                    131072) && (d.disabled = /*disabled*/
+                    c[17]), (!m || r[0] & /*label*/
                     32 && k !== (k = `range slider for ${/*label*/
-      d[5]}`)) && L(c, "aria-label", k), r[0] & /*value*/
+      c[5]}`)) && L(d, "aria-label", k), r[0] & /*value*/
                 1 && be(
-                    c,
+                    d,
                     /*value*/
-                    d[0]
+                    c[0]
                 );
         },
-        i(d) {
-            m || (Ne(t.$$.fragment, d), Ne(o.$$.fragment, d), m = !0);
+        i(c) {
+            m || (Ne(t.$$.fragment, c), Ne(o.$$.fragment, c), m = !0);
         },
-        o(d) {
-            Ve(t.$$.fragment, d), Ve(o.$$.fragment, d), m = !1;
+        o(c) {
+            Ve(t.$$.fragment, c), Ve(o.$$.fragment, c), m = !1;
         },
-        d(d) {
-            d && (fe(e), fe(n), fe(u), fe(c)), Le(t, d), Le(o), l[24](null), l[26](null), y = !1, sn(S);
+        d(c) {
+            c && (fe(e), fe(n), fe(u), fe(d)), Le(t, c), Le(o), l[24](null), l[26](null), y = !1, sn(S);
         }
     };
 }
 
 function cn(l) {
     let t, e;
     return t = new jt({
@@ -2624,19 +2623,15 @@
         d(n) {
             Le(t, n);
         }
     };
 }
 let dn = 0;
 
-function mn(l) {
-    (l.key === "ArrowUp" || l.key === "ArrowDown" || l.key === "ArrowLeft" || l.key === "ArrowRight") && l.preventDefault();
-}
-
-function bn(l, t, e) {
+function mn(l, t, e) {
     let n, {
             gradio: i
         } = t,
         {
             elem_id: f = ""
         } = t,
         {
@@ -2651,15 +2646,15 @@
         {
             label: a = i.i18n("slider.slider")
         } = t,
         {
             info: u = void 0
         } = t,
         {
-            container: c = !0
+            container: d = !0
         } = t,
         {
             scale: k = null
         } = t,
         {
             min_width: m = void 0
         } = t,
@@ -2672,113 +2667,113 @@
         {
             step: F
         } = t,
         {
             show_label: N
         } = t,
         {
-            interactive: d
+            interactive: c
         } = t,
         {
             loading_status: r
         } = t,
         {
             value_is_output: v = !1
         } = t,
         C, b;
     const G = `range_id_${dn++}`;
 
-    function J() {
+    function K() {
         i.dispatch("change"), v || i.dispatch("input");
     }
     an(() => {
         e(21, v = !1), X();
     });
 
-    function R() {
+    function O() {
         i.dispatch("release", s), e(0, s = Math.min(Math.max(s, y), S));
     }
 
     function X() {
-        P(), C.addEventListener("input", P), b.addEventListener("input", P);
+        T(), C.addEventListener("input", T), b.addEventListener("input", T);
     }
 
-    function P() {
+    function T() {
         const g = Number(C.value) - Number(C.min),
-            Z = Number(C.max) - Number(C.min),
-            re = Z === 0 ? 0 : g / Z;
+            B = Number(C.max) - Number(C.min),
+            re = B === 0 ? 0 : g / B;
         e(15, C.style.backgroundSize = re * 100 + "% 100%", C);
     }
 
     function _e(g) {
-        let Z = parseFloat(g.target.value);
-        Number.isInteger(Z) && (Z += Z + F <= g.target.max ? 1e-5 : -1e-5, e(0, s = Z));
+        let B = parseFloat(g.target.value);
+        Number.isInteger(B) && (B += B + F <= g.target.max ? 1e-5 : -1e-5, e(0, s = B));
     }
 
-    function U() {
+    function R() {
         s = je(this.value), e(0, s);
     }
 
-    function K(g) {
+    function H(g) {
         lt[g ? "unshift" : "push"](() => {
             b = g, e(16, b);
         });
     }
 
-    function T() {
+    function Z() {
         s = je(this.value), e(0, s);
     }
 
     function ae(g) {
         lt[g ? "unshift" : "push"](() => {
             C = g, e(15, C);
         });
     }
     return l.$$set = (g) => {
-        "gradio" in g && e(1, i = g.gradio), "elem_id" in g && e(2, f = g.elem_id), "elem_classes" in g && e(3, o = g.elem_classes), "visible" in g && e(4, _ = g.visible), "value" in g && e(0, s = g.value), "label" in g && e(5, a = g.label), "info" in g && e(6, u = g.info), "container" in g && e(7, c = g.container), "scale" in g && e(8, k = g.scale), "min_width" in g && e(9, m = g.min_width), "minimum" in g && e(10, y = g.minimum), "maximum" in g && e(11, S = g.maximum), "step" in g && e(12, F = g.step), "show_label" in g && e(13, N = g.show_label), "interactive" in g && e(22, d = g.interactive), "loading_status" in g && e(14, r = g.loading_status), "value_is_output" in g && e(21, v = g.value_is_output);
+        "gradio" in g && e(1, i = g.gradio), "elem_id" in g && e(2, f = g.elem_id), "elem_classes" in g && e(3, o = g.elem_classes), "visible" in g && e(4, _ = g.visible), "value" in g && e(0, s = g.value), "label" in g && e(5, a = g.label), "info" in g && e(6, u = g.info), "container" in g && e(7, d = g.container), "scale" in g && e(8, k = g.scale), "min_width" in g && e(9, m = g.min_width), "minimum" in g && e(10, y = g.minimum), "maximum" in g && e(11, S = g.maximum), "step" in g && e(12, F = g.step), "show_label" in g && e(13, N = g.show_label), "interactive" in g && e(22, c = g.interactive), "loading_status" in g && e(14, r = g.loading_status), "value_is_output" in g && e(21, v = g.value_is_output);
     }, l.$$.update = () => {
         l.$$.dirty[0] & /*interactive*/
-            4194304 && e(17, n = !d), l.$$.dirty[0] & /*value*/
-            1 && J();
+            4194304 && e(17, n = !c), l.$$.dirty[0] & /*value*/
+            1 && K();
     }, [
         s,
         i,
         f,
         o,
         _,
         a,
         u,
-        c,
+        d,
         k,
         m,
         y,
         S,
         F,
         N,
         r,
         C,
         b,
         n,
         G,
-        R,
+        O,
         _e,
         v,
-        d,
-        U,
-        K,
-        T,
+        c,
+        R,
+        H,
+        Z,
         ae
     ];
 }
-class gn extends $l {
+class bn extends $l {
     constructor(t) {
         super(), nn(
             this,
             t,
-            bn,
+            mn,
             cn,
             fn, {
                 gradio: 1,
                 elem_id: 2,
                 elem_classes: 3,
                 visible: 4,
                 value: 0,
@@ -2797,10 +2792,10 @@
             },
             null,
             [-1, -1]
         );
     }
 }
 export {
-    gn as
+    bn as
     default
 };
```

### Comparing `gradio_variableslider-0.0.3/backend/gradio_variableslider/templates/component/style.css` & `gradio_variableslider-0.0.4/backend/gradio_variableslider/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `gradio_variableslider-0.0.3/backend/gradio_variableslider/templates/example/index.js` & `gradio_variableslider-0.0.4/backend/gradio_variableslider/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `gradio_variableslider-0.0.3/demo/app.py` & `gradio_variableslider-0.0.4/demo/app.py`

 * *Files identical despite different names*

### Comparing `gradio_variableslider-0.0.3/demo/css.css` & `gradio_variableslider-0.0.4/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_variableslider-0.0.3/demo/space.py` & `gradio_variableslider-0.0.4/demo/space.py`

 * *Files identical despite different names*

### Comparing `gradio_variableslider-0.0.3/frontend/Index.svelte` & `gradio_variableslider-0.0.4/frontend/Index.svelte`

 * *Files 5% similar despite different names*

```diff
@@ -71,21 +71,14 @@
 		let sliderValue = parseFloat(event.target.value);
 		if (Number.isInteger(sliderValue)) {
 			sliderValue += sliderValue + step <= event.target.max ? 0.00001: -0.00001;
 			value = sliderValue
 		}
 	}
 
-	function disableArrowKeyInput(event: KeyboardEvent): void {
-        // Prevent default action if the key pressed is an arrow key
-        if (event.key === 'ArrowUp' || event.key === 'ArrowDown' || event.key === 'ArrowLeft' || event.key === 'ArrowRight') {
-            event.preventDefault();
-        }
-    }
-
 
 	$: disabled = !interactive;
 
 	// When the value changes, dispatch the change event via handle_change()
 	// See the docs for an explanation: https://svelte.dev/docs/svelte-components#script-3-$-marks-a-statement-as-reactive
 	$: value, handle_change();
 </script>
@@ -127,15 +120,14 @@
 		bind:value
 		bind:this={rangeInput}
 		min={minimum}
 		max={maximum}
 		{step}
 		{disabled}
 		on:input={adjustValue}
-		on:keydown={disableArrowKeyInput}
 		aria-label={`range slider for ${label}`}
 	/>
 	<!--Shows the slider value -->
 	<!-- <p>Value: {value}</p> -->
 </Block>
 
 <style>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 visible} {elem_id} {elem_classes} {container} {scale} {min_width}>
 ...loading_status} />
 show_label} {info}>{label}
 {label}`} data-testid="number-input" type="number" bind:value bind:this=
 {numberInput} min={minimum} max={maximum} on:blur={clamp} {step} {disabled}
 readonly />
 id} name="cowbell" bind:value bind:this={rangeInput} min={minimum} max=
-{maximum} {step} {disabled} on:input={adjustValue} on:keydown=
-{disableArrowKeyInput} aria-label={`range slider for ${label}`} />
+{maximum} {step} {disabled} on:input={adjustValue} aria-label={`range slider
+for ${label}`} />
```

### Comparing `gradio_variableslider-0.0.3/frontend/package-lock.json` & `gradio_variableslider-0.0.4/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_variableslider-0.0.3/README.md` & `gradio_variableslider-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gradio_variableslider-0.0.3/pyproject.toml` & `gradio_variableslider-0.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_variableslider"
-version = "0.0.3"
+version = "0.0.4"
 description = "Python library for easily interacting with trained machine learning models"
 readme = "README.md"
 license = "Apache-2.0"
 requires-python = ">=3.8"
 authors = [{ name = "Keiane Balicanta", email = "balica15@students.rowan.edu" }]
 keywords = [
   "gradio-custom-component",
@@ -37,11 +37,11 @@
   'Topic :: Scientific/Engineering :: Visualization',
 ]
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
 [tool.hatch.build]
-artifacts = ["/backend/gradio_variableslider/templates", "*.pyi", "backend/gradio_variableslider/templates", "backend/gradio_variableslider/templates", "backend/gradio_variableslider/templates", "backend/gradio_variableslider/templates"]
+artifacts = ["/backend/gradio_variableslider/templates", "*.pyi", "backend/gradio_variableslider/templates", "backend/gradio_variableslider/templates", "backend/gradio_variableslider/templates", "backend/gradio_variableslider/templates", "backend/gradio_variableslider/templates"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["/backend/gradio_variableslider"]
```

### Comparing `gradio_variableslider-0.0.3/PKG-INFO` & `gradio_variableslider-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gradio_variableslider
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python library for easily interacting with trained machine learning models
 Author-email: Keiane Balicanta <balica15@students.rowan.edu>
 License-Expression: Apache-2.0
 Keywords: gradio-custom-component,gradio-custom-slider,gradio-float-values,gradio-template-Slider
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

