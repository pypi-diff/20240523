# Comparing `tmp/gradio_clickabletextbox-0.0.1.tar.gz` & `tmp/gradio_clickabletextbox-0.0.2.tar.gz`

## Comparing `gradio_clickabletextbox-0.0.1.tar` & `gradio_clickabletextbox-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.1/backend/gradio_clickabletextbox/__init__.py
--rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.1/backend/gradio_clickabletextbox/clickabletextbox.py
--rw-r--r--   0        0        0    37699 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.1/backend/gradio_clickabletextbox/clickabletextbox.pyi
--rw-r--r--   0        0        0    92012 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.1/backend/gradio_clickabletextbox/templates/component/index.js
--rw-r--r--   0        0        0    16141 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.1/backend/gradio_clickabletextbox/templates/component/style.css
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.1/backend/gradio_clickabletextbox/templates/example/index.js
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.1/backend/gradio_clickabletextbox/templates/example/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.1/demo/__init__.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.1/demo/app.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.1/demo/css.css
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.1/demo/requirements.txt
--rw-r--r--   0        0        0    10231 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.1/demo/space.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.1/frontend/Example.svelte
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.1/frontend/Index.svelte
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.1/frontend/gradio.config.js
--rw-r--r--   0        0        0   150164 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.1/frontend/package-lock.json
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.1/frontend/package.json
--rw-r--r--   0        0        0    14366 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.1/frontend/shared/Textbox.svelte
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.1/.gitignore
--rw-r--r--   0        0        0    10608 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.1/README.md
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    11658 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/__init__.py
+-rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/clickabletextbox.py
+-rw-r--r--   0        0        0    37561 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/clickabletextbox.pyi
+-rw-r--r--   0        0        0    97610 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/templates/component/index.js
+-rw-r--r--   0        0        0    16404 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/templates/component/style.css
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/templates/example/index.js
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/templates/example/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/demo/__init__.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/demo/app.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/demo/css.css
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/demo/requirements.txt
+-rw-r--r--   0        0        0    10461 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/demo/space.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/frontend/Example.svelte
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/frontend/Index.svelte
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/frontend/gradio.config.js
+-rw-r--r--   0        0        0   150164 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/frontend/package-lock.json
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/frontend/package.json
+-rw-r--r--   0        0        0    15711 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/frontend/shared/Textbox.svelte
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/frontend/shared/transitions.js
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/.gitignore
+-rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/README.md
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.2/PKG-INFO
```

### Comparing `gradio_clickabletextbox-0.0.1/backend/gradio_clickabletextbox/clickabletextbox.py` & `gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/clickabletextbox.py`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.1/backend/gradio_clickabletextbox/clickabletextbox.pyi` & `gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/clickabletextbox.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
             postprocess: If False, will not run postprocessing of component data before returning 'fn' output to the browser.
             cancels: A list of other events to cancel when this listener is triggered. For example, setting cancels=[click_event] will cancel the click_event, where click_event is the return value of another components .click method. Functions that have not yet run (or generators that are iterating) will be cancelled, but functions that are currently running will be allowed to finish.
             every: Run this event 'every' number of seconds while the client connection is open. Interpreted in seconds.
             trigger_mode: If "once" (default for all events except `.change()`) would not allow any submissions while an event is pending. If set to "multiple", unlimited submissions are allowed while pending, and "always_last" (default for `.change()` and `.key_up()` events) would allow a second submission after the pending event is complete.
             js: Optional frontend js method to run before running 'fn'. Input arguments for js method are values of 'inputs' and 'outputs', return should be a list of values for output components.
             concurrency_limit: If set, this is the maximum number of this event that can be running simultaneously. Can be set to None to mean no concurrency_limit (any number of this event can be running simultaneously). Set to "default" to use the default concurrency limit (defined by the `default_concurrency_limit` parameter in `Blocks.queue()`, which itself is 1 by default).
             concurrency_id: If set, this is the id of the concurrency group. Events with the same concurrency_id will be limited by the lowest set concurrency_limit.
-            show_api: whether to show this event in the "view API" page of the Gradio app, or in the ".view_api()" method of the Gradio clients. Unlike setting api_name to False, setting show_api to False will still allow downstream apps as well as the Clients to use this event. If fn is None, show_api will automatically be set to False.
+            show_api: whether to show this event in the "view API" page of the Gradio app, or in the ".view_api()" method of the Gradio clients. Unlike setting api_name to False, setting show_api to False will still allow downstream apps to use this event. If fn is None, show_api will automatically be set to False.
         """
         ...
     
     def input(self,
         fn: Callable | None,
         inputs: Component | Sequence[Component] | set[Component] | None = None,
         outputs: Component | Sequence[Component] | None = None,
@@ -217,15 +217,15 @@
             postprocess: If False, will not run postprocessing of component data before returning 'fn' output to the browser.
             cancels: A list of other events to cancel when this listener is triggered. For example, setting cancels=[click_event] will cancel the click_event, where click_event is the return value of another components .click method. Functions that have not yet run (or generators that are iterating) will be cancelled, but functions that are currently running will be allowed to finish.
             every: Run this event 'every' number of seconds while the client connection is open. Interpreted in seconds.
             trigger_mode: If "once" (default for all events except `.change()`) would not allow any submissions while an event is pending. If set to "multiple", unlimited submissions are allowed while pending, and "always_last" (default for `.change()` and `.key_up()` events) would allow a second submission after the pending event is complete.
             js: Optional frontend js method to run before running 'fn'. Input arguments for js method are values of 'inputs' and 'outputs', return should be a list of values for output components.
             concurrency_limit: If set, this is the maximum number of this event that can be running simultaneously. Can be set to None to mean no concurrency_limit (any number of this event can be running simultaneously). Set to "default" to use the default concurrency limit (defined by the `default_concurrency_limit` parameter in `Blocks.queue()`, which itself is 1 by default).
             concurrency_id: If set, this is the id of the concurrency group. Events with the same concurrency_id will be limited by the lowest set concurrency_limit.
-            show_api: whether to show this event in the "view API" page of the Gradio app, or in the ".view_api()" method of the Gradio clients. Unlike setting api_name to False, setting show_api to False will still allow downstream apps as well as the Clients to use this event. If fn is None, show_api will automatically be set to False.
+            show_api: whether to show this event in the "view API" page of the Gradio app, or in the ".view_api()" method of the Gradio clients. Unlike setting api_name to False, setting show_api to False will still allow downstream apps to use this event. If fn is None, show_api will automatically be set to False.
         """
         ...
     
     def select(self,
         fn: Callable | None,
         inputs: Component | Sequence[Component] | set[Component] | None = None,
         outputs: Component | Sequence[Component] | None = None,
@@ -259,15 +259,15 @@
             postprocess: If False, will not run postprocessing of component data before returning 'fn' output to the browser.
             cancels: A list of other events to cancel when this listener is triggered. For example, setting cancels=[click_event] will cancel the click_event, where click_event is the return value of another components .click method. Functions that have not yet run (or generators that are iterating) will be cancelled, but functions that are currently running will be allowed to finish.
             every: Run this event 'every' number of seconds while the client connection is open. Interpreted in seconds.
             trigger_mode: If "once" (default for all events except `.change()`) would not allow any submissions while an event is pending. If set to "multiple", unlimited submissions are allowed while pending, and "always_last" (default for `.change()` and `.key_up()` events) would allow a second submission after the pending event is complete.
             js: Optional frontend js method to run before running 'fn'. Input arguments for js method are values of 'inputs' and 'outputs', return should be a list of values for output components.
             concurrency_limit: If set, this is the maximum number of this event that can be running simultaneously. Can be set to None to mean no concurrency_limit (any number of this event can be running simultaneously). Set to "default" to use the default concurrency limit (defined by the `default_concurrency_limit` parameter in `Blocks.queue()`, which itself is 1 by default).
             concurrency_id: If set, this is the id of the concurrency group. Events with the same concurrency_id will be limited by the lowest set concurrency_limit.
-            show_api: whether to show this event in the "view API" page of the Gradio app, or in the ".view_api()" method of the Gradio clients. Unlike setting api_name to False, setting show_api to False will still allow downstream apps as well as the Clients to use this event. If fn is None, show_api will automatically be set to False.
+            show_api: whether to show this event in the "view API" page of the Gradio app, or in the ".view_api()" method of the Gradio clients. Unlike setting api_name to False, setting show_api to False will still allow downstream apps to use this event. If fn is None, show_api will automatically be set to False.
         """
         ...
     
     def submit(self,
         fn: Callable | None,
         inputs: Component | Sequence[Component] | set[Component] | None = None,
         outputs: Component | Sequence[Component] | None = None,
@@ -301,15 +301,15 @@
             postprocess: If False, will not run postprocessing of component data before returning 'fn' output to the browser.
             cancels: A list of other events to cancel when this listener is triggered. For example, setting cancels=[click_event] will cancel the click_event, where click_event is the return value of another components .click method. Functions that have not yet run (or generators that are iterating) will be cancelled, but functions that are currently running will be allowed to finish.
             every: Run this event 'every' number of seconds while the client connection is open. Interpreted in seconds.
             trigger_mode: If "once" (default for all events except `.change()`) would not allow any submissions while an event is pending. If set to "multiple", unlimited submissions are allowed while pending, and "always_last" (default for `.change()` and `.key_up()` events) would allow a second submission after the pending event is complete.
             js: Optional frontend js method to run before running 'fn'. Input arguments for js method are values of 'inputs' and 'outputs', return should be a list of values for output components.
             concurrency_limit: If set, this is the maximum number of this event that can be running simultaneously. Can be set to None to mean no concurrency_limit (any number of this event can be running simultaneously). Set to "default" to use the default concurrency limit (defined by the `default_concurrency_limit` parameter in `Blocks.queue()`, which itself is 1 by default).
             concurrency_id: If set, this is the id of the concurrency group. Events with the same concurrency_id will be limited by the lowest set concurrency_limit.
-            show_api: whether to show this event in the "view API" page of the Gradio app, or in the ".view_api()" method of the Gradio clients. Unlike setting api_name to False, setting show_api to False will still allow downstream apps as well as the Clients to use this event. If fn is None, show_api will automatically be set to False.
+            show_api: whether to show this event in the "view API" page of the Gradio app, or in the ".view_api()" method of the Gradio clients. Unlike setting api_name to False, setting show_api to False will still allow downstream apps to use this event. If fn is None, show_api will automatically be set to False.
         """
         ...
     
     def focus(self,
         fn: Callable | None,
         inputs: Component | Sequence[Component] | set[Component] | None = None,
         outputs: Component | Sequence[Component] | None = None,
@@ -343,15 +343,15 @@
             postprocess: If False, will not run postprocessing of component data before returning 'fn' output to the browser.
             cancels: A list of other events to cancel when this listener is triggered. For example, setting cancels=[click_event] will cancel the click_event, where click_event is the return value of another components .click method. Functions that have not yet run (or generators that are iterating) will be cancelled, but functions that are currently running will be allowed to finish.
             every: Run this event 'every' number of seconds while the client connection is open. Interpreted in seconds.
             trigger_mode: If "once" (default for all events except `.change()`) would not allow any submissions while an event is pending. If set to "multiple", unlimited submissions are allowed while pending, and "always_last" (default for `.change()` and `.key_up()` events) would allow a second submission after the pending event is complete.
             js: Optional frontend js method to run before running 'fn'. Input arguments for js method are values of 'inputs' and 'outputs', return should be a list of values for output components.
             concurrency_limit: If set, this is the maximum number of this event that can be running simultaneously. Can be set to None to mean no concurrency_limit (any number of this event can be running simultaneously). Set to "default" to use the default concurrency limit (defined by the `default_concurrency_limit` parameter in `Blocks.queue()`, which itself is 1 by default).
             concurrency_id: If set, this is the id of the concurrency group. Events with the same concurrency_id will be limited by the lowest set concurrency_limit.
-            show_api: whether to show this event in the "view API" page of the Gradio app, or in the ".view_api()" method of the Gradio clients. Unlike setting api_name to False, setting show_api to False will still allow downstream apps as well as the Clients to use this event. If fn is None, show_api will automatically be set to False.
+            show_api: whether to show this event in the "view API" page of the Gradio app, or in the ".view_api()" method of the Gradio clients. Unlike setting api_name to False, setting show_api to False will still allow downstream apps to use this event. If fn is None, show_api will automatically be set to False.
         """
         ...
     
     def blur(self,
         fn: Callable | None,
         inputs: Component | Sequence[Component] | set[Component] | None = None,
         outputs: Component | Sequence[Component] | None = None,
@@ -385,10 +385,10 @@
             postprocess: If False, will not run postprocessing of component data before returning 'fn' output to the browser.
             cancels: A list of other events to cancel when this listener is triggered. For example, setting cancels=[click_event] will cancel the click_event, where click_event is the return value of another components .click method. Functions that have not yet run (or generators that are iterating) will be cancelled, but functions that are currently running will be allowed to finish.
             every: Run this event 'every' number of seconds while the client connection is open. Interpreted in seconds.
             trigger_mode: If "once" (default for all events except `.change()`) would not allow any submissions while an event is pending. If set to "multiple", unlimited submissions are allowed while pending, and "always_last" (default for `.change()` and `.key_up()` events) would allow a second submission after the pending event is complete.
             js: Optional frontend js method to run before running 'fn'. Input arguments for js method are values of 'inputs' and 'outputs', return should be a list of values for output components.
             concurrency_limit: If set, this is the maximum number of this event that can be running simultaneously. Can be set to None to mean no concurrency_limit (any number of this event can be running simultaneously). Set to "default" to use the default concurrency limit (defined by the `default_concurrency_limit` parameter in `Blocks.queue()`, which itself is 1 by default).
             concurrency_id: If set, this is the id of the concurrency group. Events with the same concurrency_id will be limited by the lowest set concurrency_limit.
-            show_api: whether to show this event in the "view API" page of the Gradio app, or in the ".view_api()" method of the Gradio clients. Unlike setting api_name to False, setting show_api to False will still allow downstream apps as well as the Clients to use this event. If fn is None, show_api will automatically be set to False.
+            show_api: whether to show this event in the "view API" page of the Gradio app, or in the ".view_api()" method of the Gradio clients. Unlike setting api_name to False, setting show_api to False will still allow downstream apps to use this event. If fn is None, show_api will automatically be set to False.
         """
         ...
```

### Comparing `gradio_clickabletextbox-0.0.1/backend/gradio_clickabletextbox/templates/component/index.js` & `gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/templates/component/index.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,86 +1,86 @@
 const {
-    SvelteComponent: wl,
-    assign: vl,
-    create_slot: kl,
-    detach: pl,
-    element: Cl,
-    get_all_dirty_from_scope: yl,
-    get_slot_changes: Ll,
-    get_spread_update: Ml,
-    init: Vl,
-    insert: ql,
-    safe_not_equal: Hl,
-    set_dynamic_element_data: ct,
+    SvelteComponent: Sl,
+    assign: zl,
+    create_slot: El,
+    detach: Tl,
+    element: Bl,
+    get_all_dirty_from_scope: Nl,
+    get_slot_changes: Dl,
+    get_spread_update: Il,
+    init: jl,
+    insert: Al,
+    safe_not_equal: Pl,
+    set_dynamic_element_data: Mt,
     set_style: K,
-    toggle_class: se,
-    transition_in: ll,
-    transition_out: nl,
-    update_slot_base: Zl
+    toggle_class: ie,
+    transition_in: dl,
+    transition_out: ml,
+    update_slot_base: Yl
 } = window.__gradio__svelte__internal;
 
-function Fl(l) {
+function Kl(l) {
     let e, t, n;
     const s = (
             /*#slots*/
             l[18].default
         ),
-        i = kl(
+        o = El(
             s,
             l,
             /*$$scope*/
             l[17],
             null
         );
-    let f = [{
+    let i = [{
             "data-testid": (
                 /*test_id*/
                 l[7]
             )
         }, {
             id: (
                 /*elem_id*/
                 l[2]
             )
         }, {
             class: t = "block " + /*elem_classes*/
                 l[3].join(" ") + " svelte-nl1om8"
         }],
-        a = {};
-    for (let r = 0; r < f.length; r += 1)
-        a = vl(a, f[r]);
+        f = {};
+    for (let r = 0; r < i.length; r += 1)
+        f = zl(f, i[r]);
     return {
         c() {
-            e = Cl(
+            e = Bl(
                 /*tag*/
                 l[14]
-            ), i && i.c(), ct(
+            ), o && o.c(), Mt(
                 /*tag*/
                 l[14]
-            )(e, a), se(
+            )(e, f), ie(
                 e,
                 "hidden",
                 /*visible*/
                 l[10] === !1
-            ), se(
+            ), ie(
                 e,
                 "padded",
                 /*padding*/
                 l[6]
-            ), se(
+            ), ie(
                 e,
                 "border_focus",
                 /*border_mode*/
                 l[5] === "focus"
-            ), se(
+            ), ie(
                 e,
                 "border_contrast",
                 /*border_mode*/
                 l[5] === "contrast"
-            ), se(e, "hide-container", ! /*explicit_call*/
+            ), ie(e, "hide-container", ! /*explicit_call*/
                 l[8] && ! /*container*/
                 l[9]), K(
                 e,
                 "height",
                 /*get_dimension*/
                 l[15](
                     /*height*/
@@ -107,230 +107,230 @@
                 e,
                 "flex-grow",
                 /*scale*/
                 l[12]
             ), K(e, "min-width", `calc(min(${/*min_width*/
       l[13]}px, 100%))`), K(e, "border-width", "var(--block-border-width)");
         },
-        m(r, o) {
-            ql(r, e, o), i && i.m(e, null), n = !0;
+        m(r, a) {
+            Al(r, e, a), o && o.m(e, null), n = !0;
         },
-        p(r, o) {
-            i && i.p && (!n || o & /*$$scope*/
-                    131072) && Zl(
-                    i,
+        p(r, a) {
+            o && o.p && (!n || a & /*$$scope*/
+                    131072) && Yl(
+                    o,
                     s,
                     r,
                     /*$$scope*/
                     r[17],
-                    n ? Ll(
+                    n ? Dl(
                         s,
                         /*$$scope*/
                         r[17],
-                        o,
+                        a,
                         null
-                    ) : yl(
+                    ) : Nl(
                         /*$$scope*/
                         r[17]
                     ),
                     null
-                ), ct(
+                ), Mt(
                     /*tag*/
                     r[14]
-                )(e, a = Ml(f, [
-                    (!n || o & /*test_id*/
+                )(e, f = Il(i, [
+                    (!n || a & /*test_id*/
                         128) && {
                         "data-testid": (
                             /*test_id*/
                             r[7]
                         )
                     },
-                    (!n || o & /*elem_id*/
+                    (!n || a & /*elem_id*/
                         4) && {
                         id: (
                             /*elem_id*/
                             r[2]
                         )
                     },
-                    (!n || o & /*elem_classes*/
+                    (!n || a & /*elem_classes*/
                         8 && t !== (t = "block " + /*elem_classes*/
                             r[3].join(" ") + " svelte-nl1om8")) && {
                         class: t
                     }
-                ])), se(
+                ])), ie(
                     e,
                     "hidden",
                     /*visible*/
                     r[10] === !1
-                ), se(
+                ), ie(
                     e,
                     "padded",
                     /*padding*/
                     r[6]
-                ), se(
+                ), ie(
                     e,
                     "border_focus",
                     /*border_mode*/
                     r[5] === "focus"
-                ), se(
+                ), ie(
                     e,
                     "border_contrast",
                     /*border_mode*/
                     r[5] === "contrast"
-                ), se(e, "hide-container", ! /*explicit_call*/
+                ), ie(e, "hide-container", ! /*explicit_call*/
                     r[8] && ! /*container*/
-                    r[9]), o & /*height*/
+                    r[9]), a & /*height*/
                 1 && K(
                     e,
                     "height",
                     /*get_dimension*/
                     r[15](
                         /*height*/
                         r[0]
                     )
-                ), o & /*width*/
+                ), a & /*width*/
                 2 && K(e, "width", typeof /*width*/ r[1] == "number" ? `calc(min(${/*width*/
       r[1]}px, 100%))` : (
                     /*get_dimension*/
                     r[15](
                         /*width*/
                         r[1]
                     )
-                )), o & /*variant*/
+                )), a & /*variant*/
                 16 && K(
                     e,
                     "border-style",
                     /*variant*/
                     r[4]
-                ), o & /*allow_overflow*/
+                ), a & /*allow_overflow*/
                 2048 && K(
                     e,
                     "overflow",
                     /*allow_overflow*/
                     r[11] ? "visible" : "hidden"
-                ), o & /*scale*/
+                ), a & /*scale*/
                 4096 && K(
                     e,
                     "flex-grow",
                     /*scale*/
                     r[12]
-                ), o & /*min_width*/
+                ), a & /*min_width*/
                 8192 && K(e, "min-width", `calc(min(${/*min_width*/
       r[13]}px, 100%))`);
         },
         i(r) {
-            n || (ll(i, r), n = !0);
+            n || (dl(o, r), n = !0);
         },
         o(r) {
-            nl(i, r), n = !1;
+            ml(o, r), n = !1;
         },
         d(r) {
-            r && pl(e), i && i.d(r);
+            r && Tl(e), o && o.d(r);
         }
     };
 }
 
-function Sl(l) {
+function Ol(l) {
     let e, t = (
         /*tag*/
-        l[14] && Fl(l)
+        l[14] && Kl(l)
     );
     return {
         c() {
             t && t.c();
         },
         m(n, s) {
             t && t.m(n, s), e = !0;
         },
         p(n, [s]) {
             /*tag*/
             n[14] && t.p(n, s);
         },
         i(n) {
-            e || (ll(t, n), e = !0);
+            e || (dl(t, n), e = !0);
         },
         o(n) {
-            nl(t, n), e = !1;
+            ml(t, n), e = !1;
         },
         d(n) {
             t && t.d(n);
         }
     };
 }
 
-function zl(l, e, t) {
+function Ul(l, e, t) {
     let {
         $$slots: n = {},
         $$scope: s
     } = e, {
-        height: i = void 0
+        height: o = void 0
     } = e, {
-        width: f = void 0
+        width: i = void 0
     } = e, {
-        elem_id: a = ""
+        elem_id: f = ""
     } = e, {
         elem_classes: r = []
     } = e, {
-        variant: o = "solid"
+        variant: a = "solid"
     } = e, {
         border_mode: u = "base"
     } = e, {
         padding: _ = !0
     } = e, {
-        type: d = "normal"
+        type: c = "normal"
     } = e, {
         test_id: h = void 0
     } = e, {
-        explicit_call: M = !1
+        explicit_call: L = !1
     } = e, {
         container: H = !0
     } = e, {
-        visible: k = !0
+        visible: p = !0
     } = e, {
-        allow_overflow: Z = !0
+        allow_overflow: v = !0
     } = e, {
-        scale: c = null
+        scale: m = null
     } = e, {
-        min_width: m = 0
-    } = e, p = d === "fieldset" ? "fieldset" : "div";
-    const V = (w) => {
-        if (w !== void 0) {
-            if (typeof w == "number")
-                return w + "px";
-            if (typeof w == "string")
-                return w;
+        min_width: b = 0
+    } = e, C = c === "fieldset" ? "fieldset" : "div";
+    const T = (k) => {
+        if (k !== void 0) {
+            if (typeof k == "number")
+                return k + "px";
+            if (typeof k == "string")
+                return k;
         }
     };
-    return l.$$set = (w) => {
-        "height" in w && t(0, i = w.height), "width" in w && t(1, f = w.width), "elem_id" in w && t(2, a = w.elem_id), "elem_classes" in w && t(3, r = w.elem_classes), "variant" in w && t(4, o = w.variant), "border_mode" in w && t(5, u = w.border_mode), "padding" in w && t(6, _ = w.padding), "type" in w && t(16, d = w.type), "test_id" in w && t(7, h = w.test_id), "explicit_call" in w && t(8, M = w.explicit_call), "container" in w && t(9, H = w.container), "visible" in w && t(10, k = w.visible), "allow_overflow" in w && t(11, Z = w.allow_overflow), "scale" in w && t(12, c = w.scale), "min_width" in w && t(13, m = w.min_width), "$$scope" in w && t(17, s = w.$$scope);
+    return l.$$set = (k) => {
+        "height" in k && t(0, o = k.height), "width" in k && t(1, i = k.width), "elem_id" in k && t(2, f = k.elem_id), "elem_classes" in k && t(3, r = k.elem_classes), "variant" in k && t(4, a = k.variant), "border_mode" in k && t(5, u = k.border_mode), "padding" in k && t(6, _ = k.padding), "type" in k && t(16, c = k.type), "test_id" in k && t(7, h = k.test_id), "explicit_call" in k && t(8, L = k.explicit_call), "container" in k && t(9, H = k.container), "visible" in k && t(10, p = k.visible), "allow_overflow" in k && t(11, v = k.allow_overflow), "scale" in k && t(12, m = k.scale), "min_width" in k && t(13, b = k.min_width), "$$scope" in k && t(17, s = k.$$scope);
     }, [
+        o,
         i,
         f,
-        a,
         r,
-        o,
+        a,
         u,
         _,
         h,
-        M,
+        L,
         H,
-        k,
-        Z,
-        c,
-        m,
         p,
-        V,
-        d,
+        v,
+        m,
+        b,
+        C,
+        T,
+        c,
         s,
         n
     ];
 }
-class El extends wl {
+class Xl extends Sl {
     constructor(e) {
-        super(), Vl(this, e, zl, Sl, Hl, {
+        super(), jl(this, e, Ul, Ol, Pl, {
             height: 0,
             width: 1,
             elem_id: 2,
             elem_classes: 3,
             variant: 4,
             border_mode: 5,
             padding: 6,
@@ -342,582 +342,582 @@
             allow_overflow: 11,
             scale: 12,
             min_width: 13
         });
     }
 }
 const {
-    SvelteComponent: Tl,
-    attr: Bl,
-    create_slot: Nl,
-    detach: Dl,
-    element: Il,
-    get_all_dirty_from_scope: jl,
-    get_slot_changes: Al,
-    init: Pl,
-    insert: Yl,
-    safe_not_equal: Kl,
-    transition_in: Ul,
-    transition_out: Xl,
-    update_slot_base: Gl
+    SvelteComponent: Gl,
+    attr: Rl,
+    create_slot: Wl,
+    detach: Jl,
+    element: Ql,
+    get_all_dirty_from_scope: xl,
+    get_slot_changes: $l,
+    init: en,
+    insert: tn,
+    safe_not_equal: ln,
+    transition_in: nn,
+    transition_out: sn,
+    update_slot_base: on
 } = window.__gradio__svelte__internal;
 
-function Ol(l) {
+function fn(l) {
     let e, t;
     const n = (
             /*#slots*/
             l[1].default
         ),
-        s = Nl(
+        s = Wl(
             n,
             l,
             /*$$scope*/
             l[0],
             null
         );
     return {
         c() {
-            e = Il("div"), s && s.c(), Bl(e, "class", "svelte-1hnfib2");
+            e = Ql("div"), s && s.c(), Rl(e, "class", "svelte-1hnfib2");
         },
-        m(i, f) {
-            Yl(i, e, f), s && s.m(e, null), t = !0;
+        m(o, i) {
+            tn(o, e, i), s && s.m(e, null), t = !0;
         },
-        p(i, [f]) {
-            s && s.p && (!t || f & /*$$scope*/
-                1) && Gl(
+        p(o, [i]) {
+            s && s.p && (!t || i & /*$$scope*/
+                1) && on(
                 s,
                 n,
-                i,
+                o,
                 /*$$scope*/
-                i[0],
-                t ? Al(
+                o[0],
+                t ? $l(
                     n,
                     /*$$scope*/
-                    i[0],
-                    f,
+                    o[0],
+                    i,
                     null
-                ) : jl(
+                ) : xl(
                     /*$$scope*/
-                    i[0]
+                    o[0]
                 ),
                 null
             );
         },
-        i(i) {
-            t || (Ul(s, i), t = !0);
+        i(o) {
+            t || (nn(s, o), t = !0);
         },
-        o(i) {
-            Xl(s, i), t = !1;
+        o(o) {
+            sn(s, o), t = !1;
         },
-        d(i) {
-            i && Dl(e), s && s.d(i);
+        d(o) {
+            o && Jl(e), s && s.d(o);
         }
     };
 }
 
-function Rl(l, e, t) {
+function an(l, e, t) {
     let {
         $$slots: n = {},
         $$scope: s
     } = e;
-    return l.$$set = (i) => {
-        "$$scope" in i && t(0, s = i.$$scope);
+    return l.$$set = (o) => {
+        "$$scope" in o && t(0, s = o.$$scope);
     }, [s, n];
 }
-class Wl extends Tl {
+class rn extends Gl {
     constructor(e) {
-        super(), Pl(this, e, Rl, Ol, Kl, {});
+        super(), en(this, e, an, fn, ln, {});
     }
 }
 const {
-    SvelteComponent: Jl,
-    attr: dt,
-    check_outros: Ql,
-    create_component: xl,
-    create_slot: $l,
-    destroy_component: en,
-    detach: De,
-    element: tn,
-    empty: ln,
-    get_all_dirty_from_scope: nn,
-    get_slot_changes: sn,
-    group_outros: fn,
-    init: on,
-    insert: Ie,
-    mount_component: an,
-    safe_not_equal: rn,
-    set_data: un,
-    space: _n,
-    text: cn,
-    toggle_class: ye,
-    transition_in: ze,
-    transition_out: je,
-    update_slot_base: dn
+    SvelteComponent: un,
+    attr: Vt,
+    check_outros: _n,
+    create_component: cn,
+    create_slot: dn,
+    destroy_component: mn,
+    detach: Pe,
+    element: hn,
+    empty: bn,
+    get_all_dirty_from_scope: gn,
+    get_slot_changes: wn,
+    group_outros: vn,
+    init: kn,
+    insert: Ye,
+    mount_component: pn,
+    safe_not_equal: Cn,
+    set_data: yn,
+    space: Ln,
+    text: Mn,
+    toggle_class: Le,
+    transition_in: Be,
+    transition_out: Ke,
+    update_slot_base: Vn
 } = window.__gradio__svelte__internal;
 
-function mt(l) {
+function Ht(l) {
     let e, t;
-    return e = new Wl({
+    return e = new rn({
         props: {
             $$slots: {
-                default: [mn]
+                default: [Hn]
             },
             $$scope: {
                 ctx: l
             }
         }
     }), {
         c() {
-            xl(e.$$.fragment);
+            cn(e.$$.fragment);
         },
         m(n, s) {
-            an(e, n, s), t = !0;
+            pn(e, n, s), t = !0;
         },
         p(n, s) {
-            const i = {};
+            const o = {};
             s & /*$$scope, info*/
-                10 && (i.$$scope = {
+                10 && (o.$$scope = {
                     dirty: s,
                     ctx: n
-                }), e.$set(i);
+                }), e.$set(o);
         },
         i(n) {
-            t || (ze(e.$$.fragment, n), t = !0);
+            t || (Be(e.$$.fragment, n), t = !0);
         },
         o(n) {
-            je(e.$$.fragment, n), t = !1;
+            Ke(e.$$.fragment, n), t = !1;
         },
         d(n) {
-            en(e, n);
+            mn(e, n);
         }
     };
 }
 
-function mn(l) {
+function Hn(l) {
     let e;
     return {
         c() {
-            e = cn(
+            e = Mn(
                 /*info*/
                 l[1]
             );
         },
         m(t, n) {
-            Ie(t, e, n);
+            Ye(t, e, n);
         },
         p(t, n) {
             n & /*info*/
-                2 && un(
+                2 && yn(
                     e,
                     /*info*/
                     t[1]
                 );
         },
         d(t) {
-            t && De(e);
+            t && Pe(e);
         }
     };
 }
 
-function hn(l) {
+function qn(l) {
     let e, t, n, s;
-    const i = (
+    const o = (
             /*#slots*/
             l[2].default
         ),
-        f = $l(
-            i,
+        i = dn(
+            o,
             l,
             /*$$scope*/
             l[3],
             null
         );
-    let a = (
+    let f = (
         /*info*/
-        l[1] && mt(l)
+        l[1] && Ht(l)
     );
     return {
         c() {
-            e = tn("span"), f && f.c(), t = _n(), a && a.c(), n = ln(), dt(e, "data-testid", "block-info"), dt(e, "class", "svelte-22c38v"), ye(e, "sr-only", ! /*show_label*/
-                l[0]), ye(e, "hide", ! /*show_label*/
-                l[0]), ye(
+            e = hn("span"), i && i.c(), t = Ln(), f && f.c(), n = bn(), Vt(e, "data-testid", "block-info"), Vt(e, "class", "svelte-22c38v"), Le(e, "sr-only", ! /*show_label*/
+                l[0]), Le(e, "hide", ! /*show_label*/
+                l[0]), Le(
                 e,
                 "has-info",
                 /*info*/
                 l[1] != null
             );
         },
-        m(r, o) {
-            Ie(r, e, o), f && f.m(e, null), Ie(r, t, o), a && a.m(r, o), Ie(r, n, o), s = !0;
+        m(r, a) {
+            Ye(r, e, a), i && i.m(e, null), Ye(r, t, a), f && f.m(r, a), Ye(r, n, a), s = !0;
         },
-        p(r, [o]) {
-            f && f.p && (!s || o & /*$$scope*/
-                    8) && dn(
-                    f,
+        p(r, [a]) {
+            i && i.p && (!s || a & /*$$scope*/
+                    8) && Vn(
                     i,
+                    o,
                     r,
                     /*$$scope*/
                     r[3],
-                    s ? sn(
-                        i,
+                    s ? wn(
+                        o,
                         /*$$scope*/
                         r[3],
-                        o,
+                        a,
                         null
-                    ) : nn(
+                    ) : gn(
                         /*$$scope*/
                         r[3]
                     ),
                     null
-                ), (!s || o & /*show_label*/
-                    1) && ye(e, "sr-only", ! /*show_label*/
-                    r[0]), (!s || o & /*show_label*/
-                    1) && ye(e, "hide", ! /*show_label*/
-                    r[0]), (!s || o & /*info*/
-                    2) && ye(
+                ), (!s || a & /*show_label*/
+                    1) && Le(e, "sr-only", ! /*show_label*/
+                    r[0]), (!s || a & /*show_label*/
+                    1) && Le(e, "hide", ! /*show_label*/
+                    r[0]), (!s || a & /*info*/
+                    2) && Le(
                     e,
                     "has-info",
                     /*info*/
                     r[1] != null
                 ), /*info*/
-                r[1] ? a ? (a.p(r, o), o & /*info*/
-                    2 && ze(a, 1)) : (a = mt(r), a.c(), ze(a, 1), a.m(n.parentNode, n)) : a && (fn(), je(a, 1, 1, () => {
-                    a = null;
-                }), Ql());
+                r[1] ? f ? (f.p(r, a), a & /*info*/
+                    2 && Be(f, 1)) : (f = Ht(r), f.c(), Be(f, 1), f.m(n.parentNode, n)) : f && (vn(), Ke(f, 1, 1, () => {
+                    f = null;
+                }), _n());
         },
         i(r) {
-            s || (ze(f, r), ze(a), s = !0);
+            s || (Be(i, r), Be(f), s = !0);
         },
         o(r) {
-            je(f, r), je(a), s = !1;
+            Ke(i, r), Ke(f), s = !1;
         },
         d(r) {
-            r && (De(e), De(t), De(n)), f && f.d(r), a && a.d(r);
+            r && (Pe(e), Pe(t), Pe(n)), i && i.d(r), f && f.d(r);
         }
     };
 }
 
-function bn(l, e, t) {
+function Fn(l, e, t) {
     let {
         $$slots: n = {},
         $$scope: s
     } = e, {
-        show_label: i = !0
+        show_label: o = !0
     } = e, {
-        info: f = void 0
+        info: i = void 0
     } = e;
-    return l.$$set = (a) => {
-        "show_label" in a && t(0, i = a.show_label), "info" in a && t(1, f = a.info), "$$scope" in a && t(3, s = a.$$scope);
-    }, [i, f, n, s];
+    return l.$$set = (f) => {
+        "show_label" in f && t(0, o = f.show_label), "info" in f && t(1, i = f.info), "$$scope" in f && t(3, s = f.$$scope);
+    }, [o, i, n, s];
 }
-class gn extends Jl {
+class Zn extends un {
     constructor(e) {
-        super(), on(this, e, bn, hn, rn, {
+        super(), kn(this, e, Fn, qn, Cn, {
             show_label: 0,
             info: 1
         });
     }
 }
 const {
-    SvelteComponent: wn,
-    append: tt,
-    attr: me,
-    bubble: vn,
-    create_component: kn,
-    destroy_component: pn,
-    detach: il,
-    element: lt,
-    init: Cn,
-    insert: sl,
-    listen: yn,
-    mount_component: Ln,
-    safe_not_equal: Mn,
-    set_data: Vn,
-    set_style: Le,
-    space: qn,
-    text: Hn,
-    toggle_class: A,
-    transition_in: Zn,
-    transition_out: Fn
+    SvelteComponent: Sn,
+    append: ut,
+    attr: ue,
+    bubble: zn,
+    create_component: En,
+    destroy_component: Tn,
+    detach: hl,
+    element: _t,
+    init: Bn,
+    insert: bl,
+    listen: Nn,
+    mount_component: Dn,
+    safe_not_equal: In,
+    set_data: jn,
+    set_style: Me,
+    space: An,
+    text: Pn,
+    toggle_class: P,
+    transition_in: Yn,
+    transition_out: Kn
 } = window.__gradio__svelte__internal;
 
-function ht(l) {
+function qt(l) {
     let e, t;
     return {
         c() {
-            e = lt("span"), t = Hn(
+            e = _t("span"), t = Pn(
                 /*label*/
                 l[1]
-            ), me(e, "class", "svelte-1lrphxw");
+            ), ue(e, "class", "svelte-1lrphxw");
         },
         m(n, s) {
-            sl(n, e, s), tt(e, t);
+            bl(n, e, s), ut(e, t);
         },
         p(n, s) {
             s & /*label*/
-                2 && Vn(
+                2 && jn(
                     t,
                     /*label*/
                     n[1]
                 );
         },
         d(n) {
-            n && il(e);
+            n && hl(e);
         }
     };
 }
 
-function Sn(l) {
-    let e, t, n, s, i, f, a, r = (
+function On(l) {
+    let e, t, n, s, o, i, f, r = (
         /*show_label*/
-        l[2] && ht(l)
+        l[2] && qt(l)
     );
     return s = new /*Icon*/
     l[0]({}), {
         c() {
-            e = lt("button"), r && r.c(), t = qn(), n = lt("div"), kn(s.$$.fragment), me(n, "class", "svelte-1lrphxw"), A(
+            e = _t("button"), r && r.c(), t = An(), n = _t("div"), En(s.$$.fragment), ue(n, "class", "svelte-1lrphxw"), P(
                     n,
                     "small",
                     /*size*/
                     l[4] === "small"
-                ), A(
+                ), P(
                     n,
                     "large",
                     /*size*/
                     l[4] === "large"
-                ), A(
+                ), P(
                     n,
                     "medium",
                     /*size*/
                     l[4] === "medium"
                 ), e.disabled = /*disabled*/
-                l[7], me(
+                l[7], ue(
                     e,
                     "aria-label",
                     /*label*/
                     l[1]
-                ), me(
+                ), ue(
                     e,
                     "aria-haspopup",
                     /*hasPopup*/
                     l[8]
-                ), me(
+                ), ue(
                     e,
                     "title",
                     /*label*/
                     l[1]
-                ), me(e, "class", "svelte-1lrphxw"), A(
+                ), ue(e, "class", "svelte-1lrphxw"), P(
                     e,
                     "pending",
                     /*pending*/
                     l[3]
-                ), A(
+                ), P(
                     e,
                     "padded",
                     /*padded*/
                     l[5]
-                ), A(
+                ), P(
                     e,
                     "highlight",
                     /*highlight*/
                     l[6]
-                ), A(
+                ), P(
                     e,
                     "transparent",
                     /*transparent*/
                     l[9]
-                ), Le(e, "color", ! /*disabled*/
+                ), Me(e, "color", ! /*disabled*/
                     l[7] && /*_color*/
                     l[12] ? (
                         /*_color*/
                         l[12]
-                    ) : "var(--block-label-text-color)"), Le(e, "--bg-color", /*disabled*/
+                    ) : "var(--block-label-text-color)"), Me(e, "--bg-color", /*disabled*/
                     l[7] ? "auto" : (
                         /*background*/
                         l[10]
-                    )), Le(
+                    )), Me(
                     e,
                     "margin-left",
                     /*offset*/
                     l[11] + "px"
                 );
         },
-        m(o, u) {
-            sl(o, e, u), r && r.m(e, null), tt(e, t), tt(e, n), Ln(s, n, null), i = !0, f || (a = yn(
+        m(a, u) {
+            bl(a, e, u), r && r.m(e, null), ut(e, t), ut(e, n), Dn(s, n, null), o = !0, i || (f = Nn(
                 e,
                 "click",
                 /*click_handler*/
                 l[14]
-            ), f = !0);
+            ), i = !0);
         },
-        p(o, [u]) {
+        p(a, [u]) {
             /*show_label*/
-            o[2] ? r ? r.p(o, u) : (r = ht(o), r.c(), r.m(e, t)) : r && (r.d(1), r = null), (!i || u & /*size*/
-                    16) && A(
+            a[2] ? r ? r.p(a, u) : (r = qt(a), r.c(), r.m(e, t)) : r && (r.d(1), r = null), (!o || u & /*size*/
+                    16) && P(
                     n,
                     "small",
                     /*size*/
-                    o[4] === "small"
-                ), (!i || u & /*size*/
-                    16) && A(
+                    a[4] === "small"
+                ), (!o || u & /*size*/
+                    16) && P(
                     n,
                     "large",
                     /*size*/
-                    o[4] === "large"
-                ), (!i || u & /*size*/
-                    16) && A(
+                    a[4] === "large"
+                ), (!o || u & /*size*/
+                    16) && P(
                     n,
                     "medium",
                     /*size*/
-                    o[4] === "medium"
-                ), (!i || u & /*disabled*/
+                    a[4] === "medium"
+                ), (!o || u & /*disabled*/
                     128) && (e.disabled = /*disabled*/
-                    o[7]), (!i || u & /*label*/
-                    2) && me(
+                    a[7]), (!o || u & /*label*/
+                    2) && ue(
                     e,
                     "aria-label",
                     /*label*/
-                    o[1]
-                ), (!i || u & /*hasPopup*/
-                    256) && me(
+                    a[1]
+                ), (!o || u & /*hasPopup*/
+                    256) && ue(
                     e,
                     "aria-haspopup",
                     /*hasPopup*/
-                    o[8]
-                ), (!i || u & /*label*/
-                    2) && me(
+                    a[8]
+                ), (!o || u & /*label*/
+                    2) && ue(
                     e,
                     "title",
                     /*label*/
-                    o[1]
-                ), (!i || u & /*pending*/
-                    8) && A(
+                    a[1]
+                ), (!o || u & /*pending*/
+                    8) && P(
                     e,
                     "pending",
                     /*pending*/
-                    o[3]
-                ), (!i || u & /*padded*/
-                    32) && A(
+                    a[3]
+                ), (!o || u & /*padded*/
+                    32) && P(
                     e,
                     "padded",
                     /*padded*/
-                    o[5]
-                ), (!i || u & /*highlight*/
-                    64) && A(
+                    a[5]
+                ), (!o || u & /*highlight*/
+                    64) && P(
                     e,
                     "highlight",
                     /*highlight*/
-                    o[6]
-                ), (!i || u & /*transparent*/
-                    512) && A(
+                    a[6]
+                ), (!o || u & /*transparent*/
+                    512) && P(
                     e,
                     "transparent",
                     /*transparent*/
-                    o[9]
+                    a[9]
                 ), u & /*disabled, _color*/
-                4224 && Le(e, "color", ! /*disabled*/
-                    o[7] && /*_color*/
-                    o[12] ? (
+                4224 && Me(e, "color", ! /*disabled*/
+                    a[7] && /*_color*/
+                    a[12] ? (
                         /*_color*/
-                        o[12]
+                        a[12]
                     ) : "var(--block-label-text-color)"), u & /*disabled, background*/
-                1152 && Le(e, "--bg-color", /*disabled*/
-                    o[7] ? "auto" : (
+                1152 && Me(e, "--bg-color", /*disabled*/
+                    a[7] ? "auto" : (
                         /*background*/
-                        o[10]
+                        a[10]
                     )), u & /*offset*/
-                2048 && Le(
+                2048 && Me(
                     e,
                     "margin-left",
                     /*offset*/
-                    o[11] + "px"
+                    a[11] + "px"
                 );
         },
-        i(o) {
-            i || (Zn(s.$$.fragment, o), i = !0);
+        i(a) {
+            o || (Yn(s.$$.fragment, a), o = !0);
         },
-        o(o) {
-            Fn(s.$$.fragment, o), i = !1;
+        o(a) {
+            Kn(s.$$.fragment, a), o = !1;
         },
-        d(o) {
-            o && il(e), r && r.d(), pn(s), f = !1, a();
+        d(a) {
+            a && hl(e), r && r.d(), Tn(s), i = !1, f();
         }
     };
 }
 
-function zn(l, e, t) {
+function Un(l, e, t) {
     let n, {
             Icon: s
         } = e,
         {
-            label: i = ""
+            label: o = ""
         } = e,
         {
-            show_label: f = !1
+            show_label: i = !1
         } = e,
         {
-            pending: a = !1
+            pending: f = !1
         } = e,
         {
             size: r = "small"
         } = e,
         {
-            padded: o = !0
+            padded: a = !0
         } = e,
         {
             highlight: u = !1
         } = e,
         {
             disabled: _ = !1
         } = e,
         {
-            hasPopup: d = !1
+            hasPopup: c = !1
         } = e,
         {
             color: h = "var(--block-label-text-color)"
         } = e,
         {
-            transparent: M = !1
+            transparent: L = !1
         } = e,
         {
             background: H = "var(--background-fill-primary)"
         } = e,
         {
-            offset: k = 0
+            offset: p = 0
         } = e;
 
-    function Z(c) {
-        vn.call(this, l, c);
+    function v(m) {
+        zn.call(this, l, m);
     }
-    return l.$$set = (c) => {
-        "Icon" in c && t(0, s = c.Icon), "label" in c && t(1, i = c.label), "show_label" in c && t(2, f = c.show_label), "pending" in c && t(3, a = c.pending), "size" in c && t(4, r = c.size), "padded" in c && t(5, o = c.padded), "highlight" in c && t(6, u = c.highlight), "disabled" in c && t(7, _ = c.disabled), "hasPopup" in c && t(8, d = c.hasPopup), "color" in c && t(13, h = c.color), "transparent" in c && t(9, M = c.transparent), "background" in c && t(10, H = c.background), "offset" in c && t(11, k = c.offset);
+    return l.$$set = (m) => {
+        "Icon" in m && t(0, s = m.Icon), "label" in m && t(1, o = m.label), "show_label" in m && t(2, i = m.show_label), "pending" in m && t(3, f = m.pending), "size" in m && t(4, r = m.size), "padded" in m && t(5, a = m.padded), "highlight" in m && t(6, u = m.highlight), "disabled" in m && t(7, _ = m.disabled), "hasPopup" in m && t(8, c = m.hasPopup), "color" in m && t(13, h = m.color), "transparent" in m && t(9, L = m.transparent), "background" in m && t(10, H = m.background), "offset" in m && t(11, p = m.offset);
     }, l.$$.update = () => {
         l.$$.dirty & /*highlight, color*/
             8256 && t(12, n = u ? "var(--color-accent)" : h);
     }, [
         s,
+        o,
         i,
         f,
-        a,
         r,
-        o,
+        a,
         u,
         _,
-        d,
-        M,
+        c,
+        L,
         H,
-        k,
+        p,
         n,
         h,
-        Z
+        v
     ];
 }
-class En extends wn {
+class Xn extends Sn {
     constructor(e) {
-        super(), Cn(this, e, zn, Sn, Mn, {
+        super(), Bn(this, e, Un, On, In, {
             Icon: 0,
             label: 1,
             show_label: 2,
             pending: 3,
             size: 4,
             padded: 5,
             highlight: 6,
@@ -927,49 +927,49 @@
             transparent: 9,
             background: 10,
             offset: 11
         });
     }
 }
 const {
-    SvelteComponent: Tn,
-    append: We,
-    attr: Q,
-    detach: Bn,
-    init: Nn,
-    insert: Dn,
-    noop: Je,
-    safe_not_equal: In,
-    set_style: fe,
-    svg_element: Te
+    SvelteComponent: Gn,
+    append: it,
+    attr: R,
+    detach: Rn,
+    init: Wn,
+    insert: Jn,
+    noop: st,
+    safe_not_equal: Qn,
+    set_style: se,
+    svg_element: Ie
 } = window.__gradio__svelte__internal;
 
-function jn(l) {
+function xn(l) {
     let e, t, n, s;
     return {
         c() {
-            e = Te("svg"), t = Te("g"), n = Te("path"), s = Te("path"), Q(n, "d", "M18,6L6.087,17.913"), fe(n, "fill", "none"), fe(n, "fill-rule", "nonzero"), fe(n, "stroke-width", "2px"), Q(t, "transform", "matrix(1.14096,-0.140958,-0.140958,1.14096,-0.0559523,0.0559523)"), Q(s, "d", "M4.364,4.364L19.636,19.636"), fe(s, "fill", "none"), fe(s, "fill-rule", "nonzero"), fe(s, "stroke-width", "2px"), Q(e, "width", "100%"), Q(e, "height", "100%"), Q(e, "viewBox", "0 0 24 24"), Q(e, "version", "1.1"), Q(e, "xmlns", "http://www.w3.org/2000/svg"), Q(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), Q(e, "xml:space", "preserve"), Q(e, "stroke", "currentColor"), fe(e, "fill-rule", "evenodd"), fe(e, "clip-rule", "evenodd"), fe(e, "stroke-linecap", "round"), fe(e, "stroke-linejoin", "round");
+            e = Ie("svg"), t = Ie("g"), n = Ie("path"), s = Ie("path"), R(n, "d", "M18,6L6.087,17.913"), se(n, "fill", "none"), se(n, "fill-rule", "nonzero"), se(n, "stroke-width", "2px"), R(t, "transform", "matrix(1.14096,-0.140958,-0.140958,1.14096,-0.0559523,0.0559523)"), R(s, "d", "M4.364,4.364L19.636,19.636"), se(s, "fill", "none"), se(s, "fill-rule", "nonzero"), se(s, "stroke-width", "2px"), R(e, "width", "100%"), R(e, "height", "100%"), R(e, "viewBox", "0 0 24 24"), R(e, "version", "1.1"), R(e, "xmlns", "http://www.w3.org/2000/svg"), R(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), R(e, "xml:space", "preserve"), R(e, "stroke", "currentColor"), se(e, "fill-rule", "evenodd"), se(e, "clip-rule", "evenodd"), se(e, "stroke-linecap", "round"), se(e, "stroke-linejoin", "round");
         },
-        m(i, f) {
-            Dn(i, e, f), We(e, t), We(t, n), We(e, s);
+        m(o, i) {
+            Jn(o, e, i), it(e, t), it(t, n), it(e, s);
         },
-        p: Je,
-        i: Je,
-        o: Je,
-        d(i) {
-            i && Bn(e);
+        p: st,
+        i: st,
+        o: st,
+        d(o) {
+            o && Rn(e);
         }
     };
 }
-class An extends Tn {
+class $n extends Gn {
     constructor(e) {
-        super(), Nn(this, e, null, jn, In, {});
+        super(), Wn(this, e, null, xn, Qn, {});
     }
 }
-const Pn = [{
+const ei = [{
         color: "red",
         primary: 600,
         secondary: 100
     }, {
         color: "green",
         primary: 600,
         secondary: 100
@@ -1002,15 +1002,15 @@
         primary: 500,
         secondary: 100
     }, {
         color: "pink",
         primary: 600,
         secondary: 100
     }],
-    bt = {
+    Ft = {
         inherit: "inherit",
         current: "currentColor",
         transparent: "transparent",
         black: "#000",
         white: "#fff",
         slate: {
             50: "#f8fafc",
@@ -1295,2131 +1295,2406 @@
             600: "#e11d48",
             700: "#be123c",
             800: "#9f1239",
             900: "#881337",
             950: "#4c0519"
         }
     };
-Pn.reduce(
+ei.reduce(
     (l, {
         color: e,
         primary: t,
         secondary: n
     }) => ({
         ...l,
         [e]: {
-            primary: bt[e][t],
-            secondary: bt[e][n]
+            primary: Ft[e][t],
+            secondary: Ft[e][n]
         }
     }), {}
 );
 
-function Ae() {}
-const Yn = (l) => l;
+function Oe() {}
 
-function Kn(l, e) {
+function ti(l, e) {
     return l != l ? e == e : l !== e || l && typeof l == "object" || typeof l == "function";
 }
-const fl = typeof window < "u";
-let gt = fl ? () => window.performance.now() : () => Date.now(),
-    ol = fl ? (l) => requestAnimationFrame(l) : Ae;
-const Ze = /* @__PURE__ */ new Set();
-
-function al(l) {
-    Ze.forEach((e) => {
-        e.c(l) || (Ze.delete(e), e.f());
-    }), Ze.size !== 0 && ol(al);
+const gl = typeof window < "u";
+let Zt = gl ? () => window.performance.now() : () => Date.now(),
+    wl = gl ? (l) => requestAnimationFrame(l) : Oe;
+const Se = /* @__PURE__ */ new Set();
+
+function vl(l) {
+    Se.forEach((e) => {
+        e.c(l) || (Se.delete(e), e.f());
+    }), Se.size !== 0 && wl(vl);
 }
 
-function Un(l) {
+function li(l) {
     let e;
-    return Ze.size === 0 && ol(al), {
+    return Se.size === 0 && wl(vl), {
         promise: new Promise((t) => {
-            Ze.add(e = {
+            Se.add(e = {
                 c: l,
                 f: t
             });
         }),
         abort() {
-            Ze.delete(e);
+            Se.delete(e);
         }
     };
 }
 
-function wt(l, {
-    delay: e = 0,
-    duration: t = 400,
-    easing: n = Yn
-} = {}) {
-    const s = +getComputedStyle(l).opacity;
-    return {
-        delay: e,
-        duration: t,
-        easing: n,
-        css: (i) => `opacity: ${i * s}`
-    };
+function ni(l) {
+    const e = l - 1;
+    return e * e * e + 1;
 }
-const Me = [];
+const Ve = [];
 
-function Xn(l, e = Ae) {
+function ii(l, e = Oe) {
     let t;
     const n = /* @__PURE__ */ new Set();
 
-    function s(a) {
-        if (Kn(l, a) && (l = a, t)) {
-            const r = !Me.length;
-            for (const o of n)
-                o[1](), Me.push(o, l);
+    function s(f) {
+        if (ti(l, f) && (l = f, t)) {
+            const r = !Ve.length;
+            for (const a of n)
+                a[1](), Ve.push(a, l);
             if (r) {
-                for (let o = 0; o < Me.length; o += 2)
-                    Me[o][0](Me[o + 1]);
-                Me.length = 0;
+                for (let a = 0; a < Ve.length; a += 2)
+                    Ve[a][0](Ve[a + 1]);
+                Ve.length = 0;
             }
         }
     }
 
-    function i(a) {
-        s(a(l));
+    function o(f) {
+        s(f(l));
     }
 
-    function f(a, r = Ae) {
-        const o = [a, r];
-        return n.add(o), n.size === 1 && (t = e(s, i) || Ae), a(l), () => {
-            n.delete(o), n.size === 0 && t && (t(), t = null);
+    function i(f, r = Oe) {
+        const a = [f, r];
+        return n.add(a), n.size === 1 && (t = e(s, o) || Oe), f(l), () => {
+            n.delete(a), n.size === 0 && t && (t(), t = null);
         };
     }
     return {
         set: s,
-        update: i,
-        subscribe: f
+        update: o,
+        subscribe: i
     };
 }
 
-function vt(l) {
+function St(l) {
     return Object.prototype.toString.call(l) === "[object Date]";
 }
 
-function nt(l, e, t, n) {
-    if (typeof t == "number" || vt(t)) {
+function ct(l, e, t, n) {
+    if (typeof t == "number" || St(t)) {
         const s = n - t,
-            i = (t - e) / (l.dt || 1 / 60),
-            f = l.opts.stiffness * s,
-            a = l.opts.damping * i,
-            r = (f - a) * l.inv_mass,
-            o = (i + r) * l.dt;
-        return Math.abs(o) < l.opts.precision && Math.abs(s) < l.opts.precision ? n : (l.settled = !1, vt(t) ? new Date(t.getTime() + o) : t + o);
+            o = (t - e) / (l.dt || 1 / 60),
+            i = l.opts.stiffness * s,
+            f = l.opts.damping * o,
+            r = (i - f) * l.inv_mass,
+            a = (o + r) * l.dt;
+        return Math.abs(a) < l.opts.precision && Math.abs(s) < l.opts.precision ? n : (l.settled = !1, St(t) ? new Date(t.getTime() + a) : t + a);
     } else {
         if (Array.isArray(t))
             return t.map(
-                (s, i) => nt(l, e[i], t[i], n[i])
+                (s, o) => ct(l, e[o], t[o], n[o])
             );
         if (typeof t == "object") {
             const s = {};
-            for (const i in t)
-                s[i] = nt(l, e[i], t[i], n[i]);
+            for (const o in t)
+                s[o] = ct(l, e[o], t[o], n[o]);
             return s;
         } else
             throw new Error(`Cannot spring ${typeof t} values`);
     }
 }
 
-function kt(l, e = {}) {
-    const t = Xn(l),
+function zt(l, e = {}) {
+    const t = ii(l),
         {
             stiffness: n = 0.15,
             damping: s = 0.8,
-            precision: i = 0.01
+            precision: o = 0.01
         } = e;
-    let f, a, r, o = l,
+    let i, f, r, a = l,
         u = l,
         _ = 1,
-        d = 0,
+        c = 0,
         h = !1;
 
-    function M(k, Z = {}) {
-        u = k;
-        const c = r = {};
-        return l == null || Z.hard || H.stiffness >= 1 && H.damping >= 1 ? (h = !0, f = gt(), o = k, t.set(l = u), Promise.resolve()) : (Z.soft && (d = 1 / ((Z.soft === !0 ? 0.5 : +Z.soft) * 60), _ = 0), a || (f = gt(), h = !1, a = Un((m) => {
+    function L(p, v = {}) {
+        u = p;
+        const m = r = {};
+        return l == null || v.hard || H.stiffness >= 1 && H.damping >= 1 ? (h = !0, i = Zt(), a = p, t.set(l = u), Promise.resolve()) : (v.soft && (c = 1 / ((v.soft === !0 ? 0.5 : +v.soft) * 60), _ = 0), f || (i = Zt(), h = !1, f = li((b) => {
             if (h)
-                return h = !1, a = null, !1;
-            _ = Math.min(_ + d, 1);
-            const p = {
+                return h = !1, f = null, !1;
+            _ = Math.min(_ + c, 1);
+            const C = {
                     inv_mass: _,
                     opts: H,
                     settled: !0,
-                    dt: (m - f) * 60 / 1e3
+                    dt: (b - i) * 60 / 1e3
                 },
-                V = nt(p, o, l, u);
-            return f = m, o = l, t.set(l = V), p.settled && (a = null), !p.settled;
-        })), new Promise((m) => {
-            a.promise.then(() => {
-                c === r && m();
+                T = ct(C, a, l, u);
+            return i = b, a = l, t.set(l = T), C.settled && (f = null), !C.settled;
+        })), new Promise((b) => {
+            f.promise.then(() => {
+                m === r && b();
             });
         }));
     }
     const H = {
-        set: M,
-        update: (k, Z) => M(k(u, l), Z),
+        set: L,
+        update: (p, v) => L(p(u, l), v),
         subscribe: t.subscribe,
         stiffness: n,
         damping: s,
-        precision: i
+        precision: o
     };
     return H;
 }
+
+function Et(l, {
+    delay: e = 0,
+    duration: t = 500,
+    easing: n = ni
+} = {}) {
+    const s = parseFloat(getComputedStyle(l).height);
+    return {
+        delay: e,
+        duration: t,
+        easing: n,
+        css: (o) => {
+            const i = o,
+                f = `translateY(${(1 - o) * -10}px)`,
+                r = o * s;
+            return `
+                opacity: ${i};
+                transform: ${f};
+                height: ${r}px;
+            `;
+        }
+    };
+}
 const {
-    SvelteComponent: Gn,
-    action_destroyer: On,
-    add_render_callback: Rn,
-    append: S,
-    attr: C,
-    binding_callbacks: Wn,
-    bubble: pt,
-    check_outros: Jn,
-    create_bidirectional_transition: Ct,
-    create_component: Qn,
-    destroy_component: xn,
-    destroy_each: rl,
-    detach: ue,
-    element: I,
-    ensure_array_like: Pe,
-    group_outros: $n,
-    init: ei,
-    insert: _e,
-    is_function: ti,
-    listen: oe,
-    mount_component: li,
-    noop: Qe,
-    run_all: ni,
-    safe_not_equal: ii,
-    set_data: ot,
-    set_input_value: yt,
-    space: ce,
-    svg_element: Ye,
-    text: at,
-    toggle_class: Lt,
-    transition_in: xe,
-    transition_out: $e
+    SvelteComponent: si,
+    action_destroyer: bt,
+    add_render_callback: oi,
+    append: F,
+    attr: g,
+    binding_callbacks: ot,
+    bubble: He,
+    check_outros: fi,
+    create_bidirectional_transition: Tt,
+    create_component: ai,
+    destroy_component: ri,
+    destroy_each: kl,
+    detach: $,
+    element: B,
+    ensure_array_like: Ue,
+    group_outros: ui,
+    init: _i,
+    insert: ee,
+    is_function: gt,
+    listen: E,
+    mount_component: ci,
+    noop: Xe,
+    null_to_empty: wt,
+    run_all: vt,
+    safe_not_equal: di,
+    set_data: kt,
+    set_input_value: ze,
+    space: te,
+    svg_element: Ge,
+    text: pt,
+    toggle_class: Bt,
+    transition_in: ft,
+    transition_out: at
 } = window.__gradio__svelte__internal, {
-    beforeUpdate: si,
-    afterUpdate: fi,
-    createEventDispatcher: oi,
-    tick: Mt
+    beforeUpdate: mi,
+    afterUpdate: hi,
+    createEventDispatcher: bi,
+    tick: Nt
 } = window.__gradio__svelte__internal;
 
-function Vt(l, e, t) {
+function Dt(l, e, t) {
     const n = l.slice();
-    return n[39] = e[t], n;
+    return n[47] = e[t], n;
 }
 
-function qt(l, e, t) {
+function It(l, e, t) {
     const n = l.slice();
-    return n[39] = e[t], n;
+    return n[47] = e[t], n;
 }
 
-function ai(l) {
+function gi(l) {
     let e;
     return {
         c() {
-            e = at(
+            e = pt(
                 /*label*/
                 l[3]
             );
         },
         m(t, n) {
-            _e(t, e, n);
+            ee(t, e, n);
         },
         p(t, n) {
             n[0] & /*label*/
-                8 && ot(
+                8 && kt(
                     e,
                     /*label*/
                     t[3]
                 );
         },
         d(t) {
-            t && ue(e);
+            t && $(e);
         }
     };
 }
 
-function ri(l) {
-    let e, t, n;
+function wi(l) {
+    let e, t, n, s, o, i;
     return {
         c() {
-            e = I("button"), e.innerHTML = '<svg width="26" height="26" viewBox="0 0 26 26" fill="none" xmlns="http://www.w3.org/2000/svg" class="svelte-n6pmag"><path d="M23.0978 15.6987L23.5777 15.2188L21.7538 13.3952L21.2739 13.8751L23.0978 15.6987ZM11.1253 2.74873L10.6454 3.22809L12.4035 4.98733L12.8834 4.50769L11.1253 2.74873ZM25.5996 9.23801H22.885V9.91673H25.5996V9.23801ZM10.6692 9.23801H7.95457V9.91673H10.6692V9.23801ZM21.8008 5.01533L23.5982 3.21773L23.118 2.73781L21.3206 4.53541L21.8008 5.01533ZM17.2391 7.29845L18.6858 8.74521C18.7489 8.80822 18.7989 8.88303 18.8331 8.96538C18.8672 9.04773 18.8847 9.13599 18.8847 9.22513C18.8847 9.31427 18.8672 9.40254 18.8331 9.48488C18.7989 9.56723 18.7489 9.64205 18.6858 9.70505L3.00501 25.3859C2.74013 25.6511 2.31061 25.6511 2.04517 25.3859L0.598406 23.9391C0.535351 23.8761 0.485329 23.8013 0.4512 23.719C0.417072 23.6366 0.399506 23.5483 0.399506 23.4592C0.399506 23.3701 0.417072 23.2818 0.4512 23.1995C0.485329 23.1171 0.535351 23.0423 0.598406 22.9793L16.2792 7.29845C16.3422 7.23533 16.417 7.18525 16.4994 7.15108C16.5817 7.11691 16.67 7.09932 16.7592 7.09932C16.8483 7.09932 16.9366 7.11691 17.019 7.15108C17.1013 7.18525 17.1761 7.23533 17.2391 7.29845ZM14.4231 13.2042L18.3792 9.24893L16.746 7.61541L12.7899 11.5713L14.4231 13.2042ZM17.4555 0.415771H16.7768V3.13037H17.4555V0.415771ZM17.4555 15.3462H16.7768V18.0608H17.4555V15.3462Z" fill="#CCCCCC" class="svelte-n6pmag"></path></svg>', C(e, "class", "extend_button svelte-n6pmag"), C(e, "aria-label", "Extend"), C(e, "aria-roledescription", "Extend text");
+            e = B("textarea"), g(e, "data-testid", "textbox"), g(e, "class", wt(
+                    /*show_magic*/
+                    l[15] ? "scroll_hide_magic" : "scroll-hide"
+                ) + " svelte-82ixrs"), g(e, "dir", t = /*rtl*/
+                    l[10] ? "rtl" : "ltr"), g(
+                    e,
+                    "placeholder",
+                    /*placeholder*/
+                    l[2]
+                ), g(
+                    e,
+                    "rows",
+                    /*lines*/
+                    l[1]
+                ), e.disabled = /*disabled*/
+                l[5], e.autofocus = /*autofocus*/
+                l[11], g(e, "style", n = /*text_align*/
+                    l[12] ? "text-align: " + /*text_align*/
+                    l[12] : "");
         },
-        m(s, i) {
-            _e(s, e, i), t || (n = oe(
-                e,
-                "click",
-                /*handle_extension*/
-                l[15]
-            ), t = !0);
+        m(f, r) {
+            ee(f, e, r), ze(
+                    e,
+                    /*value*/
+                    l[0]
+                ), l[38](e), /*autofocus*/
+                l[11] && e.focus(), o || (i = [
+                    bt(s = /*text_area_resize*/
+                        l[21].call(
+                            null,
+                            e,
+                            /*value*/
+                            l[0]
+                        )),
+                    E(
+                        e,
+                        "input",
+                        /*textarea_input_handler_2*/
+                        l[37]
+                    ),
+                    E(
+                        e,
+                        "keypress",
+                        /*handle_keypress*/
+                        l[19]
+                    ),
+                    E(
+                        e,
+                        "blur",
+                        /*blur_handler_2*/
+                        l[29]
+                    ),
+                    E(
+                        e,
+                        "select",
+                        /*handle_select*/
+                        l[18]
+                    ),
+                    E(
+                        e,
+                        "focus",
+                        /*focus_handler_2*/
+                        l[30]
+                    ),
+                    E(
+                        e,
+                        "scroll",
+                        /*handle_scroll*/
+                        l[20]
+                    )
+                ], o = !0);
         },
-        p: Qe,
-        i: Qe,
-        o: Qe,
-        d(s) {
-            s && ue(e), t = !1, n();
+        p(f, r) {
+            r[0] & /*rtl*/
+                1024 && t !== (t = /*rtl*/
+                    f[10] ? "rtl" : "ltr") && g(e, "dir", t), r[0] & /*placeholder*/
+                4 && g(
+                    e,
+                    "placeholder",
+                    /*placeholder*/
+                    f[2]
+                ), r[0] & /*lines*/
+                2 && g(
+                    e,
+                    "rows",
+                    /*lines*/
+                    f[1]
+                ), r[0] & /*disabled*/
+                32 && (e.disabled = /*disabled*/
+                    f[5]), r[0] & /*autofocus*/
+                2048 && (e.autofocus = /*autofocus*/
+                    f[11]), r[0] & /*text_align*/
+                4096 && n !== (n = /*text_align*/
+                    f[12] ? "text-align: " + /*text_align*/
+                    f[12] : "") && g(e, "style", n), s && gt(s.update) && r[0] & /*value*/
+                1 && s.update.call(
+                    null,
+                    /*value*/
+                    f[0]
+                ), r[0] & /*value*/
+                1 && ze(
+                    e,
+                    /*value*/
+                    f[0]
+                );
+        },
+        i: Xe,
+        o: Xe,
+        d(f) {
+            f && $(e), l[38](null), o = !1, vt(i);
         }
     };
 }
 
-function ui(l) {
-    let e, t, n, s, i, f, a, r, o = (
+function vi(l) {
+    let e, t, n, s, o, i, f, r, a;
+    return {
+        c() {
+            e = B("div"), t = B("textarea"), i = te(), f = B("button"), f.innerHTML = '<svg width="26" height="26" viewBox="0 0 26 26" fill="none" xmlns="http://www.w3.org/2000/svg" class="svelte-82ixrs"><path d="M23.0978 15.6987L23.5777 15.2188L21.7538 13.3952L21.2739 13.8751L23.0978 15.6987ZM11.1253 2.74873L10.6454 3.22809L12.4035 4.98733L12.8834 4.50769L11.1253 2.74873ZM25.5996 9.23801H22.885V9.91673H25.5996V9.23801ZM10.6692 9.23801H7.95457V9.91673H10.6692V9.23801ZM21.8008 5.01533L23.5982 3.21773L23.118 2.73781L21.3206 4.53541L21.8008 5.01533ZM17.2391 7.29845L18.6858 8.74521C18.7489 8.80822 18.7989 8.88303 18.8331 8.96538C18.8672 9.04773 18.8847 9.13599 18.8847 9.22513C18.8847 9.31427 18.8672 9.40254 18.8331 9.48488C18.7989 9.56723 18.7489 9.64205 18.6858 9.70505L3.00501 25.3859C2.74013 25.6511 2.31061 25.6511 2.04517 25.3859L0.598406 23.9391C0.535351 23.8761 0.485329 23.8013 0.4512 23.719C0.417072 23.6366 0.399506 23.5483 0.399506 23.4592C0.399506 23.3701 0.417072 23.2818 0.4512 23.1995C0.485329 23.1171 0.535351 23.0423 0.598406 22.9793L16.2792 7.29845C16.3422 7.23533 16.417 7.18525 16.4994 7.15108C16.5817 7.11691 16.67 7.09932 16.7592 7.09932C16.8483 7.09932 16.9366 7.11691 17.019 7.15108C17.1013 7.18525 17.1761 7.23533 17.2391 7.29845ZM14.4231 13.2042L18.3792 9.24893L16.746 7.61541L12.7899 11.5713L14.4231 13.2042ZM17.4555 0.415771H16.7768V3.13037H17.4555V0.415771ZM17.4555 15.3462H16.7768V18.0608H17.4555V15.3462Z" fill="#CCCCCC" class="svelte-82ixrs"></path></svg>', g(t, "data-testid", "textbox"), g(t, "class", wt(
+                    /*show_magic*/
+                    l[15] ? "scroll_hide_magic" : "scroll-hide"
+                ) + " svelte-82ixrs"), g(t, "dir", n = /*rtl*/
+                    l[10] ? "rtl" : "ltr"), g(
+                    t,
+                    "placeholder",
+                    /*placeholder*/
+                    l[2]
+                ), g(
+                    t,
+                    "rows",
+                    /*lines*/
+                    l[1]
+                ), t.disabled = /*disabled*/
+                l[5], t.autofocus = /*autofocus*/
+                l[11], g(t, "style", s = /*text_align*/
+                    l[12] ? "text-align: " + /*text_align*/
+                    l[12] : ""), g(f, "class", "extend_button svelte-82ixrs"), g(f, "aria-label", "Extend"), g(f, "aria-roledescription", "Extend text"), g(e, "class", "magic_container svelte-82ixrs");
+        },
+        m(u, _) {
+            ee(u, e, _), F(e, t), ze(
+                    t,
+                    /*value*/
+                    l[0]
+                ), l[36](t), F(e, i), F(e, f), /*autofocus*/
+                l[11] && t.focus(), r || (a = [
+                    bt(o = /*text_area_resize*/
+                        l[21].call(
+                            null,
+                            t,
+                            /*value*/
+                            l[0]
+                        )),
+                    E(
+                        t,
+                        "input",
+                        /*textarea_input_handler_1*/
+                        l[35]
+                    ),
+                    E(
+                        t,
+                        "keypress",
+                        /*handle_keypress*/
+                        l[19]
+                    ),
+                    E(
+                        t,
+                        "blur",
+                        /*blur_handler_1*/
+                        l[27]
+                    ),
+                    E(
+                        t,
+                        "select",
+                        /*handle_select*/
+                        l[18]
+                    ),
+                    E(
+                        t,
+                        "focus",
+                        /*focus_handler_1*/
+                        l[28]
+                    ),
+                    E(
+                        t,
+                        "scroll",
+                        /*handle_scroll*/
+                        l[20]
+                    ),
+                    E(
+                        f,
+                        "click",
+                        /*handle_extension*/
+                        l[16]
+                    )
+                ], r = !0);
+        },
+        p(u, _) {
+            _[0] & /*rtl*/
+                1024 && n !== (n = /*rtl*/
+                    u[10] ? "rtl" : "ltr") && g(t, "dir", n), _[0] & /*placeholder*/
+                4 && g(
+                    t,
+                    "placeholder",
+                    /*placeholder*/
+                    u[2]
+                ), _[0] & /*lines*/
+                2 && g(
+                    t,
+                    "rows",
+                    /*lines*/
+                    u[1]
+                ), _[0] & /*disabled*/
+                32 && (t.disabled = /*disabled*/
+                    u[5]), _[0] & /*autofocus*/
+                2048 && (t.autofocus = /*autofocus*/
+                    u[11]), _[0] & /*text_align*/
+                4096 && s !== (s = /*text_align*/
+                    u[12] ? "text-align: " + /*text_align*/
+                    u[12] : "") && g(t, "style", s), o && gt(o.update) && _[0] & /*value*/
+                1 && o.update.call(
+                    null,
+                    /*value*/
+                    u[0]
+                ), _[0] & /*value*/
+                1 && ze(
+                    t,
+                    /*value*/
+                    u[0]
+                );
+        },
+        i: Xe,
+        o: Xe,
+        d(u) {
+            u && $(e), l[36](null), r = !1, vt(a);
+        }
+    };
+}
+
+function ki(l) {
+    let e, t, n, s, o, i, f, r, a, u, _, c, h, L, H = (
             /*prompts*/
-            l[8].length > 0 && Ht(l)
+            l[8].length > 0 && jt(l)
         ),
-        u = (
+        p = (
             /*suffixes*/
-            l[9].length > 0 && Ft(l)
+            l[9].length > 0 && Pt(l)
         );
     return {
         c() {
-            e = I("button"), e.innerHTML = '<svg width="26" height="26" viewBox="0 0 26 26" fill="none" xmlns="http://www.w3.org/2000/svg" class="svelte-n6pmag"><path d="M23.0978 15.6987L23.5777 15.2188L21.7538 13.3952L21.2739 13.8751L23.0978 15.6987ZM11.1253 2.74873L10.6454 3.22809L12.4035 4.98733L12.8834 4.50769L11.1253 2.74873ZM25.5996 9.23801H22.885V9.91673H25.5996V9.23801ZM10.6692 9.23801H7.95457V9.91673H10.6692V9.23801ZM21.8008 5.01533L23.5982 3.21773L23.118 2.73781L21.3206 4.53541L21.8008 5.01533ZM17.2391 7.29845L18.6858 8.74521C18.7489 8.80822 18.7989 8.88303 18.8331 8.96538C18.8672 9.04773 18.8847 9.13599 18.8847 9.22513C18.8847 9.31427 18.8672 9.40254 18.8331 9.48488C18.7989 9.56723 18.7489 9.64205 18.6858 9.70505L3.00501 25.3859C2.74013 25.6511 2.31061 25.6511 2.04517 25.3859L0.598406 23.9391C0.535351 23.8761 0.485329 23.8013 0.4512 23.719C0.417072 23.6366 0.399506 23.5483 0.399506 23.4592C0.399506 23.3701 0.417072 23.2818 0.4512 23.1995C0.485329 23.1171 0.535351 23.0423 0.598406 22.9793L16.2792 7.29845C16.3422 7.23533 16.417 7.18525 16.4994 7.15108C16.5817 7.11691 16.67 7.09932 16.7592 7.09932C16.8483 7.09932 16.9366 7.11691 17.019 7.15108C17.1013 7.18525 17.1761 7.23533 17.2391 7.29845ZM14.4231 13.2042L18.3792 9.24893L16.746 7.61541L12.7899 11.5713L14.4231 13.2042ZM17.4555 0.415771H16.7768V3.13037H17.4555V0.415771ZM17.4555 15.3462H16.7768V18.0608H17.4555V15.3462Z" fill="#ff6700" class="svelte-n6pmag"></path></svg>', t = ce(), n = I("div"), o && o.c(), s = ce(), u && u.c(), C(e, "class", "extend_button svelte-n6pmag"), C(e, "aria-label", "Extend"), C(e, "aria-roledescription", "Extend text"), C(n, "class", "menu svelte-n6pmag");
+            e = B("div"), t = B("textarea"), i = te(), f = B("button"), f.innerHTML = '<svg width="26" height="26" viewBox="0 0 26 26" fill="none" xmlns="http://www.w3.org/2000/svg" class="svelte-82ixrs"><path d="M23.0978 15.6987L23.5777 15.2188L21.7538 13.3952L21.2739 13.8751L23.0978 15.6987ZM11.1253 2.74873L10.6454 3.22809L12.4035 4.98733L12.8834 4.50769L11.1253 2.74873ZM25.5996 9.23801H22.885V9.91673H25.5996V9.23801ZM10.6692 9.23801H7.95457V9.91673H10.6692V9.23801ZM21.8008 5.01533L23.5982 3.21773L23.118 2.73781L21.3206 4.53541L21.8008 5.01533ZM17.2391 7.29845L18.6858 8.74521C18.7489 8.80822 18.7989 8.88303 18.8331 8.96538C18.8672 9.04773 18.8847 9.13599 18.8847 9.22513C18.8847 9.31427 18.8672 9.40254 18.8331 9.48488C18.7989 9.56723 18.7489 9.64205 18.6858 9.70505L3.00501 25.3859C2.74013 25.6511 2.31061 25.6511 2.04517 25.3859L0.598406 23.9391C0.535351 23.8761 0.485329 23.8013 0.4512 23.719C0.417072 23.6366 0.399506 23.5483 0.399506 23.4592C0.399506 23.3701 0.417072 23.2818 0.4512 23.1995C0.485329 23.1171 0.535351 23.0423 0.598406 22.9793L16.2792 7.29845C16.3422 7.23533 16.417 7.18525 16.4994 7.15108C16.5817 7.11691 16.67 7.09932 16.7592 7.09932C16.8483 7.09932 16.9366 7.11691 17.019 7.15108C17.1013 7.18525 17.1761 7.23533 17.2391 7.29845ZM14.4231 13.2042L18.3792 9.24893L16.746 7.61541L12.7899 11.5713L14.4231 13.2042ZM17.4555 0.415771H16.7768V3.13037H17.4555V0.415771ZM17.4555 15.3462H16.7768V18.0608H17.4555V15.3462Z" fill="#ff6700" class="svelte-82ixrs"></path></svg>', r = te(), a = B("div"), H && H.c(), u = te(), p && p.c(), g(t, "data-testid", "textbox"), g(t, "class", wt(
+                    /*show_magic*/
+                    l[15] ? "scroll_hide_magic" : "scroll-hide"
+                ) + " svelte-82ixrs"), g(t, "dir", n = /*rtl*/
+                    l[10] ? "rtl" : "ltr"), g(
+                    t,
+                    "placeholder",
+                    /*placeholder*/
+                    l[2]
+                ), g(
+                    t,
+                    "rows",
+                    /*lines*/
+                    l[1]
+                ), t.disabled = /*disabled*/
+                l[5], t.autofocus = /*autofocus*/
+                l[11], g(t, "style", s = /*text_align*/
+                    l[12] ? "text-align: " + /*text_align*/
+                    l[12] : ""), g(f, "class", "extend_button svelte-82ixrs"), g(f, "aria-label", "Extend"), g(f, "aria-roledescription", "Extend text"), g(e, "class", "magic_container svelte-82ixrs"), g(a, "class", "menu svelte-82ixrs");
         },
-        m(_, d) {
-            _e(_, e, d), _e(_, t, d), _e(_, n, d), o && o.m(n, null), S(n, s), u && u.m(n, null), f = !0, a || (r = oe(
-                e,
-                "click",
-                /*handle_extension*/
-                l[15]
-            ), a = !0);
+        m(v, m) {
+            ee(v, e, m), F(e, t), ze(
+                    t,
+                    /*value*/
+                    l[0]
+                ), l[32](t), F(e, i), F(e, f), ee(v, r, m), ee(v, a, m), H && H.m(a, null), F(a, u), p && p.m(a, null), c = !0, /*autofocus*/
+                l[11] && t.focus(), h || (L = [
+                    bt(o = /*text_area_resize*/
+                        l[21].call(
+                            null,
+                            t,
+                            /*value*/
+                            l[0]
+                        )),
+                    E(
+                        t,
+                        "input",
+                        /*textarea_input_handler*/
+                        l[31]
+                    ),
+                    E(
+                        t,
+                        "keypress",
+                        /*handle_keypress*/
+                        l[19]
+                    ),
+                    E(
+                        t,
+                        "blur",
+                        /*blur_handler*/
+                        l[25]
+                    ),
+                    E(
+                        t,
+                        "select",
+                        /*handle_select*/
+                        l[18]
+                    ),
+                    E(
+                        t,
+                        "focus",
+                        /*focus_handler*/
+                        l[26]
+                    ),
+                    E(
+                        t,
+                        "scroll",
+                        /*handle_scroll*/
+                        l[20]
+                    ),
+                    E(
+                        f,
+                        "click",
+                        /*handle_extension*/
+                        l[16]
+                    )
+                ], h = !0);
         },
-        p(_, d) {
-            /*prompts*/
-            _[8].length > 0 ? o ? o.p(_, d) : (o = Ht(_), o.c(), o.m(n, s)) : o && (o.d(1), o = null), /*suffixes*/
-                _[9].length > 0 ? u ? u.p(_, d) : (u = Ft(_), u.c(), u.m(n, null)) : u && (u.d(1), u = null);
+        p(v, m) {
+            (!c || m[0] & /*rtl*/
+                1024 && n !== (n = /*rtl*/
+                    v[10] ? "rtl" : "ltr")) && g(t, "dir", n), (!c || m[0] & /*placeholder*/
+                    4) && g(
+                    t,
+                    "placeholder",
+                    /*placeholder*/
+                    v[2]
+                ), (!c || m[0] & /*lines*/
+                    2) && g(
+                    t,
+                    "rows",
+                    /*lines*/
+                    v[1]
+                ), (!c || m[0] & /*disabled*/
+                    32) && (t.disabled = /*disabled*/
+                    v[5]), (!c || m[0] & /*autofocus*/
+                    2048) && (t.autofocus = /*autofocus*/
+                    v[11]), (!c || m[0] & /*text_align*/
+                    4096 && s !== (s = /*text_align*/
+                        v[12] ? "text-align: " + /*text_align*/
+                        v[12] : "")) && g(t, "style", s), o && gt(o.update) && m[0] & /*value*/
+                1 && o.update.call(
+                    null,
+                    /*value*/
+                    v[0]
+                ), m[0] & /*value*/
+                1 && ze(
+                    t,
+                    /*value*/
+                    v[0]
+                ), /*prompts*/
+                v[8].length > 0 ? H ? H.p(v, m) : (H = jt(v), H.c(), H.m(a, u)) : H && (H.d(1), H = null), /*suffixes*/
+                v[9].length > 0 ? p ? p.p(v, m) : (p = Pt(v), p.c(), p.m(a, null)) : p && (p.d(1), p = null);
         },
-        i(_) {
-            f || (_ && Rn(() => {
-                f && (i || (i = Ct(n, wt, {}, !0)), i.run(1));
-            }), f = !0);
+        i(v) {
+            c || (v && oi(() => {
+                c && (_ || (_ = Tt(a, Et, {}, !0)), _.run(1));
+            }), c = !0);
         },
-        o(_) {
-            _ && (i || (i = Ct(n, wt, {}, !1)), i.run(0)), f = !1;
+        o(v) {
+            v && (_ || (_ = Tt(a, Et, {}, !1)), _.run(0)), c = !1;
         },
-        d(_) {
-            _ && (ue(e), ue(t), ue(n)), o && o.d(), u && u.d(), _ && i && i.end(), a = !1, r();
+        d(v) {
+            v && ($(e), $(r), $(a)), l[32](null), H && H.d(), p && p.d(), v && _ && _.end(), h = !1, vt(L);
         }
     };
 }
 
-function Ht(l) {
-    let e, t, n, s, i = Pe(
+function jt(l) {
+    let e, t, n, s, o = Ue(
             /*prompts*/
             l[8]
         ),
-        f = [];
-    for (let a = 0; a < i.length; a += 1)
-        f[a] = Zt(qt(l, i, a));
+        i = [];
+    for (let f = 0; f < o.length; f += 1)
+        i[f] = At(It(l, o, f));
     return {
         c() {
-            e = I("div"), t = I("span"), t.textContent = "Best prompt structures", n = ce(), s = I("ul");
-            for (let a = 0; a < f.length; a += 1)
-                f[a].c();
-            C(s, "class", "svelte-n6pmag"), C(e, "class", "menu_section svelte-n6pmag");
-        },
-        m(a, r) {
-            _e(a, e, r), S(e, t), S(e, n), S(e, s);
-            for (let o = 0; o < f.length; o += 1)
-                f[o] && f[o].m(s, null);
+            e = B("div"), t = B("span"), t.textContent = "Best prompt structures", n = te(), s = B("ul");
+            for (let f = 0; f < i.length; f += 1)
+                i[f].c();
+            g(s, "class", "svelte-82ixrs"), g(e, "class", "menu_section svelte-82ixrs");
+        },
+        m(f, r) {
+            ee(f, e, r), F(e, t), F(e, n), F(e, s);
+            for (let a = 0; a < i.length; a += 1)
+                i[a] && i[a].m(s, null);
         },
-        p(a, r) {
+        p(f, r) {
             if (r[0] & /*addToTextbox, prompts*/
-                65792) {
-                i = Pe(
+                131328) {
+                o = Ue(
                     /*prompts*/
-                    a[8]
+                    f[8]
                 );
-                let o;
-                for (o = 0; o < i.length; o += 1) {
-                    const u = qt(a, i, o);
-                    f[o] ? f[o].p(u, r) : (f[o] = Zt(u), f[o].c(), f[o].m(s, null));
+                let a;
+                for (a = 0; a < o.length; a += 1) {
+                    const u = It(f, o, a);
+                    i[a] ? i[a].p(u, r) : (i[a] = At(u), i[a].c(), i[a].m(s, null));
                 }
-                for (; o < f.length; o += 1)
-                    f[o].d(1);
-                f.length = i.length;
+                for (; a < i.length; a += 1)
+                    i[a].d(1);
+                i.length = o.length;
             }
         },
-        d(a) {
-            a && ue(e), rl(f, a);
+        d(f) {
+            f && $(e), kl(i, f);
         }
     };
 }
 
-function Zt(l) {
+function At(l) {
     let e, t, n = (
             /*word*/
-            l[39] + ""
+            l[47] + ""
         ),
-        s, i, f, a, r, o, u;
+        s, o, i, f, r, a, u;
 
     function _() {
         return (
             /*click_handler*/
-            l[29](
+            l[33](
                 /*word*/
-                l[39]
+                l[47]
             )
         );
     }
     return {
         c() {
-            e = I("li"), t = I("button"), s = at(n), i = ce(), f = Ye("svg"), a = Ye("path"), r = ce(), C(a, "d", "M8.70801 5.51112H5.95801V2.57779C5.95801 2.44813 5.90972 2.32377 5.82376 2.23209C5.73781 2.14041 5.62123 2.0889 5.49967 2.0889C5.37812 2.0889 5.26154 2.14041 5.17558 2.23209C5.08963 2.32377 5.04134 2.44813 5.04134 2.57779V5.51112H2.29134C2.16978 5.51112 2.0532 5.56263 1.96725 5.65431C1.8813 5.746 1.83301 5.87035 1.83301 6.00001C1.83301 6.12967 1.8813 6.25402 1.96725 6.34571C2.0532 6.43739 2.16978 6.4889 2.29134 6.4889H5.04134V9.42223C5.04134 9.55189 5.08963 9.67624 5.17558 9.76793C5.26154 9.85961 5.37812 9.91112 5.49967 9.91112C5.62123 9.91112 5.73781 9.85961 5.82376 9.76793C5.90972 9.67624 5.95801 9.55189 5.95801 9.42223V6.4889H8.70801C8.82956 6.4889 8.94614 6.43739 9.0321 6.34571C9.11805 6.25402 9.16634 6.12967 9.16634 6.00001C9.16634 5.87035 9.11805 5.746 9.0321 5.65431C8.94614 5.56263 8.82956 5.51112 8.70801 5.51112Z"), C(a, "fill", "#FF9A57"), C(a, "class", "svelte-n6pmag"), C(f, "xmlns", "http://www.w3.org/2000/svg"), C(f, "width", "11"), C(f, "height", "12"), C(f, "viewBox", "0 0 11 12"), C(f, "fill", "none"), C(f, "class", "svelte-n6pmag"), C(t, "class", "text_extension_button_prompt svelte-n6pmag"), C(e, "class", "svelte-n6pmag");
+            e = B("li"), t = B("button"), s = pt(n), o = te(), i = Ge("svg"), f = Ge("path"), r = te(), g(f, "d", "M8.70801 5.51112H5.95801V2.57779C5.95801 2.44813 5.90972 2.32377 5.82376 2.23209C5.73781 2.14041 5.62123 2.0889 5.49967 2.0889C5.37812 2.0889 5.26154 2.14041 5.17558 2.23209C5.08963 2.32377 5.04134 2.44813 5.04134 2.57779V5.51112H2.29134C2.16978 5.51112 2.0532 5.56263 1.96725 5.65431C1.8813 5.746 1.83301 5.87035 1.83301 6.00001C1.83301 6.12967 1.8813 6.25402 1.96725 6.34571C2.0532 6.43739 2.16978 6.4889 2.29134 6.4889H5.04134V9.42223C5.04134 9.55189 5.08963 9.67624 5.17558 9.76793C5.26154 9.85961 5.37812 9.91112 5.49967 9.91112C5.62123 9.91112 5.73781 9.85961 5.82376 9.76793C5.90972 9.67624 5.95801 9.55189 5.95801 9.42223V6.4889H8.70801C8.82956 6.4889 8.94614 6.43739 9.0321 6.34571C9.11805 6.25402 9.16634 6.12967 9.16634 6.00001C9.16634 5.87035 9.11805 5.746 9.0321 5.65431C8.94614 5.56263 8.82956 5.51112 8.70801 5.51112Z"), g(f, "fill", "#FF9A57"), g(f, "class", "svelte-82ixrs"), g(i, "xmlns", "http://www.w3.org/2000/svg"), g(i, "width", "11"), g(i, "height", "12"), g(i, "viewBox", "0 0 11 12"), g(i, "fill", "none"), g(i, "class", "svelte-82ixrs"), g(t, "class", "text_extension_button_prompt svelte-82ixrs"), g(e, "class", "svelte-82ixrs");
         },
-        m(d, h) {
-            _e(d, e, h), S(e, t), S(t, s), S(t, i), S(t, f), S(f, a), S(e, r), o || (u = oe(t, "click", _), o = !0);
+        m(c, h) {
+            ee(c, e, h), F(e, t), F(t, s), F(t, o), F(t, i), F(i, f), F(e, r), a || (u = E(t, "click", _), a = !0);
         },
-        p(d, h) {
-            l = d, h[0] & /*prompts*/
+        p(c, h) {
+            l = c, h[0] & /*prompts*/
                 256 && n !== (n = /*word*/
-                    l[39] + "") && ot(s, n);
+                    l[47] + "") && kt(s, n);
         },
-        d(d) {
-            d && ue(e), o = !1, u();
+        d(c) {
+            c && $(e), a = !1, u();
         }
     };
 }
 
-function Ft(l) {
-    let e, t, n, s, i = Pe(
+function Pt(l) {
+    let e, t, n, s, o = Ue(
             /*suffixes*/
             l[9]
         ),
-        f = [];
-    for (let a = 0; a < i.length; a += 1)
-        f[a] = St(Vt(l, i, a));
+        i = [];
+    for (let f = 0; f < o.length; f += 1)
+        i[f] = Yt(Dt(l, o, f));
     return {
         c() {
-            e = I("div"), t = I("span"), t.textContent = "Best style keywords", n = ce(), s = I("ul");
-            for (let a = 0; a < f.length; a += 1)
-                f[a].c();
-            C(s, "class", "svelte-n6pmag"), C(e, "class", "menu_section svelte-n6pmag");
-        },
-        m(a, r) {
-            _e(a, e, r), S(e, t), S(e, n), S(e, s);
-            for (let o = 0; o < f.length; o += 1)
-                f[o] && f[o].m(s, null);
+            e = B("div"), t = B("span"), t.textContent = "Best style keywords", n = te(), s = B("ul");
+            for (let f = 0; f < i.length; f += 1)
+                i[f].c();
+            g(s, "class", "svelte-82ixrs"), g(e, "class", "menu_section svelte-82ixrs");
+        },
+        m(f, r) {
+            ee(f, e, r), F(e, t), F(e, n), F(e, s);
+            for (let a = 0; a < i.length; a += 1)
+                i[a] && i[a].m(s, null);
         },
-        p(a, r) {
+        p(f, r) {
             if (r[0] & /*addToTextbox, suffixes*/
-                66048) {
-                i = Pe(
+                131584) {
+                o = Ue(
                     /*suffixes*/
-                    a[9]
+                    f[9]
                 );
-                let o;
-                for (o = 0; o < i.length; o += 1) {
-                    const u = Vt(a, i, o);
-                    f[o] ? f[o].p(u, r) : (f[o] = St(u), f[o].c(), f[o].m(s, null));
+                let a;
+                for (a = 0; a < o.length; a += 1) {
+                    const u = Dt(f, o, a);
+                    i[a] ? i[a].p(u, r) : (i[a] = Yt(u), i[a].c(), i[a].m(s, null));
                 }
-                for (; o < f.length; o += 1)
-                    f[o].d(1);
-                f.length = i.length;
+                for (; a < i.length; a += 1)
+                    i[a].d(1);
+                i.length = o.length;
             }
         },
-        d(a) {
-            a && ue(e), rl(f, a);
+        d(f) {
+            f && $(e), kl(i, f);
         }
     };
 }
 
-function St(l) {
+function Yt(l) {
     let e, t, n = (
             /*word*/
-            l[39] + ""
+            l[47] + ""
         ),
-        s, i, f, a, r, o, u;
+        s, o, i, f, r, a, u;
 
     function _() {
         return (
             /*click_handler_1*/
-            l[30](
+            l[34](
                 /*word*/
-                l[39]
+                l[47]
             )
         );
     }
     return {
         c() {
-            e = I("li"), t = I("button"), s = at(n), i = ce(), f = Ye("svg"), a = Ye("path"), r = ce(), C(a, "d", "M8.70801 5.51112H5.95801V2.57779C5.95801 2.44813 5.90972 2.32377 5.82376 2.23209C5.73781 2.14041 5.62123 2.0889 5.49967 2.0889C5.37812 2.0889 5.26154 2.14041 5.17558 2.23209C5.08963 2.32377 5.04134 2.44813 5.04134 2.57779V5.51112H2.29134C2.16978 5.51112 2.0532 5.56263 1.96725 5.65431C1.8813 5.746 1.83301 5.87035 1.83301 6.00001C1.83301 6.12967 1.8813 6.25402 1.96725 6.34571C2.0532 6.43739 2.16978 6.4889 2.29134 6.4889H5.04134V9.42223C5.04134 9.55189 5.08963 9.67624 5.17558 9.76793C5.26154 9.85961 5.37812 9.91112 5.49967 9.91112C5.62123 9.91112 5.73781 9.85961 5.82376 9.76793C5.90972 9.67624 5.95801 9.55189 5.95801 9.42223V6.4889H8.70801C8.82956 6.4889 8.94614 6.43739 9.0321 6.34571C9.11805 6.25402 9.16634 6.12967 9.16634 6.00001C9.16634 5.87035 9.11805 5.746 9.0321 5.65431C8.94614 5.56263 8.82956 5.51112 8.70801 5.51112Z"), C(a, "fill", "#FF9A57"), C(a, "class", "svelte-n6pmag"), C(f, "xmlns", "http://www.w3.org/2000/svg"), C(f, "width", "11"), C(f, "height", "12"), C(f, "viewBox", "0 0 11 12"), C(f, "fill", "none"), C(f, "class", "svelte-n6pmag"), C(t, "class", "text_extension_button svelte-n6pmag"), C(e, "class", "svelte-n6pmag");
+            e = B("li"), t = B("button"), s = pt(n), o = te(), i = Ge("svg"), f = Ge("path"), r = te(), g(f, "d", "M8.70801 5.51112H5.95801V2.57779C5.95801 2.44813 5.90972 2.32377 5.82376 2.23209C5.73781 2.14041 5.62123 2.0889 5.49967 2.0889C5.37812 2.0889 5.26154 2.14041 5.17558 2.23209C5.08963 2.32377 5.04134 2.44813 5.04134 2.57779V5.51112H2.29134C2.16978 5.51112 2.0532 5.56263 1.96725 5.65431C1.8813 5.746 1.83301 5.87035 1.83301 6.00001C1.83301 6.12967 1.8813 6.25402 1.96725 6.34571C2.0532 6.43739 2.16978 6.4889 2.29134 6.4889H5.04134V9.42223C5.04134 9.55189 5.08963 9.67624 5.17558 9.76793C5.26154 9.85961 5.37812 9.91112 5.49967 9.91112C5.62123 9.91112 5.73781 9.85961 5.82376 9.76793C5.90972 9.67624 5.95801 9.55189 5.95801 9.42223V6.4889H8.70801C8.82956 6.4889 8.94614 6.43739 9.0321 6.34571C9.11805 6.25402 9.16634 6.12967 9.16634 6.00001C9.16634 5.87035 9.11805 5.746 9.0321 5.65431C8.94614 5.56263 8.82956 5.51112 8.70801 5.51112Z"), g(f, "fill", "#FF9A57"), g(f, "class", "svelte-82ixrs"), g(i, "xmlns", "http://www.w3.org/2000/svg"), g(i, "width", "11"), g(i, "height", "12"), g(i, "viewBox", "0 0 11 12"), g(i, "fill", "none"), g(i, "class", "svelte-82ixrs"), g(t, "class", "text_extension_button svelte-82ixrs"), g(e, "class", "svelte-82ixrs");
         },
-        m(d, h) {
-            _e(d, e, h), S(e, t), S(t, s), S(t, i), S(t, f), S(f, a), S(e, r), o || (u = oe(t, "click", _), o = !0);
+        m(c, h) {
+            ee(c, e, h), F(e, t), F(t, s), F(t, o), F(t, i), F(i, f), F(e, r), a || (u = E(t, "click", _), a = !0);
         },
-        p(d, h) {
-            l = d, h[0] & /*suffixes*/
+        p(c, h) {
+            l = c, h[0] & /*suffixes*/
                 512 && n !== (n = /*word*/
-                    l[39] + "") && ot(s, n);
+                    l[47] + "") && kt(s, n);
         },
-        d(d) {
-            d && ue(e), o = !1, u();
+        d(c) {
+            c && $(e), a = !1, u();
         }
     };
 }
 
-function _i(l) {
-    let e, t, n, s, i, f, a, r, o, u, _, d, h, M;
-    t = new gn({
+function pi(l) {
+    let e, t, n, s, o, i, f;
+    t = new Zn({
         props: {
             show_label: (
                 /*show_label*/
                 l[6]
             ),
             info: (
                 /*info*/
                 l[4]
             ),
             $$slots: {
-                default: [ai]
+                default: [gi]
             },
             $$scope: {
                 ctx: l
             }
         }
     });
-    const H = [ui, ri],
-        k = [];
+    const r = [ki, vi, wi],
+        a = [];
 
-    function Z(c, m) {
+    function u(_, c) {
         return (
             /*show_menu*/
-            c[14] && /*prompts*/
-            (c[8].length > 0 || /*suffixes*/
-                c[9].length > 0) ? 0 : (
-                /*prompts*/
-                c[8].length > 0 || /*suffixes*/
-                c[9].length > 0 ? 1 : -1
-            )
+            _[14] && /*show_magic*/
+            _[15] ? 0 : ! /*show_menu*/
+            _[14] && /*show_magic*/
+            _[15] ? 1 : 2
         );
     }
-    return ~(u = Z(l)) && (_ = k[u] = H[u](l)), {
+    return o = u(l), i = a[o] = r[o](l), {
         c() {
-            e = I("label"), Qn(t.$$.fragment), n = ce(), s = I("div"), i = I("textarea"), o = ce(), _ && _.c(), C(i, "data-testid", "textbox"), C(i, "class", "scroll-hide svelte-n6pmag"), C(i, "dir", f = /*rtl*/
-                    l[10] ? "rtl" : "ltr"), C(
-                    i,
-                    "placeholder",
-                    /*placeholder*/
-                    l[2]
-                ), C(
-                    i,
-                    "rows",
-                    /*lines*/
-                    l[1]
-                ), i.disabled = /*disabled*/
-                l[5], i.autofocus = /*autofocus*/
-                l[11], C(i, "style", a = /*text_align*/
-                    l[12] ? "text-align: " + /*text_align*/
-                    l[12] : ""), C(s, "class", "input-container"), C(e, "class", "svelte-n6pmag"), Lt(
-                    e,
-                    "container",
-                    /*container*/
-                    l[7]
-                );
+            e = B("label"), ai(t.$$.fragment), n = te(), s = B("div"), i.c(), g(s, "class", "input-container"), g(e, "class", "svelte-82ixrs"), Bt(
+                e,
+                "container",
+                /*container*/
+                l[7]
+            );
         },
-        m(c, m) {
-            _e(c, e, m), li(t, e, null), S(e, n), S(e, s), S(s, i), yt(
-                    i,
-                    /*value*/
-                    l[0]
-                ), l[28](i), S(s, o), ~u && k[u].m(s, null), d = !0, /*autofocus*/
-                l[11] && i.focus(), h || (M = [
-                    On(r = /*text_area_resize*/
-                        l[20].call(
-                            null,
-                            i,
-                            /*value*/
-                            l[0]
-                        )),
-                    oe(
-                        i,
-                        "input",
-                        /*textarea_input_handler*/
-                        l[27]
-                    ),
-                    oe(
-                        i,
-                        "keypress",
-                        /*handle_keypress*/
-                        l[18]
-                    ),
-                    oe(
-                        i,
-                        "blur",
-                        /*blur_handler*/
-                        l[25]
-                    ),
-                    oe(
-                        i,
-                        "select",
-                        /*handle_select*/
-                        l[17]
-                    ),
-                    oe(
-                        i,
-                        "focus",
-                        /*focus_handler*/
-                        l[26]
-                    ),
-                    oe(
-                        i,
-                        "scroll",
-                        /*handle_scroll*/
-                        l[19]
-                    )
-                ], h = !0);
+        m(_, c) {
+            ee(_, e, c), ci(t, e, null), F(e, n), F(e, s), a[o].m(s, null), f = !0;
         },
-        p(c, m) {
-            const p = {};
-            m[0] & /*show_label*/
-                64 && (p.show_label = /*show_label*/
-                    c[6]), m[0] & /*info*/
-                16 && (p.info = /*info*/
-                    c[4]), m[0] & /*label*/
-                8 | m[1] & /*$$scope*/
-                8192 && (p.$$scope = {
-                    dirty: m,
-                    ctx: c
-                }), t.$set(p), (!d || m[0] & /*rtl*/
-                    1024 && f !== (f = /*rtl*/
-                        c[10] ? "rtl" : "ltr")) && C(i, "dir", f), (!d || m[0] & /*placeholder*/
-                    4) && C(
-                    i,
-                    "placeholder",
-                    /*placeholder*/
-                    c[2]
-                ), (!d || m[0] & /*lines*/
-                    2) && C(
-                    i,
-                    "rows",
-                    /*lines*/
-                    c[1]
-                ), (!d || m[0] & /*disabled*/
-                    32) && (i.disabled = /*disabled*/
-                    c[5]), (!d || m[0] & /*autofocus*/
-                    2048) && (i.autofocus = /*autofocus*/
-                    c[11]), (!d || m[0] & /*text_align*/
-                    4096 && a !== (a = /*text_align*/
-                        c[12] ? "text-align: " + /*text_align*/
-                        c[12] : "")) && C(i, "style", a), r && ti(r.update) && m[0] & /*value*/
-                1 && r.update.call(
-                    null,
-                    /*value*/
-                    c[0]
-                ), m[0] & /*value*/
-                1 && yt(
-                    i,
-                    /*value*/
-                    c[0]
-                );
-            let V = u;
-            u = Z(c), u === V ? ~u && k[u].p(c, m) : (_ && ($n(), $e(k[V], 1, 1, () => {
-                k[V] = null;
-            }), Jn()), ~u ? (_ = k[u], _ ? _.p(c, m) : (_ = k[u] = H[u](c), _.c()), xe(_, 1), _.m(s, null)) : _ = null), (!d || m[0] & /*container*/
-                128) && Lt(
+        p(_, c) {
+            const h = {};
+            c[0] & /*show_label*/
+                64 && (h.show_label = /*show_label*/
+                    _[6]), c[0] & /*info*/
+                16 && (h.info = /*info*/
+                    _[4]), c[0] & /*label*/
+                8 | c[1] & /*$$scope*/
+                2097152 && (h.$$scope = {
+                    dirty: c,
+                    ctx: _
+                }), t.$set(h);
+            let L = o;
+            o = u(_), o === L ? a[o].p(_, c) : (ui(), at(a[L], 1, 1, () => {
+                a[L] = null;
+            }), fi(), i = a[o], i ? i.p(_, c) : (i = a[o] = r[o](_), i.c()), ft(i, 1), i.m(s, null)), (!f || c[0] & /*container*/
+                128) && Bt(
                 e,
                 "container",
                 /*container*/
-                c[7]
+                _[7]
             );
         },
-        i(c) {
-            d || (xe(t.$$.fragment, c), xe(_), d = !0);
+        i(_) {
+            f || (ft(t.$$.fragment, _), ft(i), f = !0);
         },
-        o(c) {
-            $e(t.$$.fragment, c), $e(_), d = !1;
+        o(_) {
+            at(t.$$.fragment, _), at(i), f = !1;
         },
-        d(c) {
-            c && ue(e), xn(t), l[28](null), ~u && k[u].d(), h = !1, ni(M);
+        d(_) {
+            _ && $(e), ri(t), a[o].d();
         }
     };
 }
 
-function ci(l, e, t) {
-    var n = this && this.__awaiter || function(b, T, B, N) {
-        function Y(ie) {
-            return ie instanceof B ? ie : new B(function(Ce) {
-                Ce(ie);
+function Ci(l, e, t) {
+    var n = this && this.__awaiter || function(d, S, D, A) {
+        function me(Te) {
+            return Te instanceof D ? Te : new D(function(De) {
+                De(Te);
             });
         }
-        return new(B || (B = Promise))(function(ie, Ce) {
-            function Oe(J) {
+        return new(D || (D = Promise))(function(Te, De) {
+            function Fl(he) {
                 try {
-                    W(N.next(J));
-                } catch (Re) {
-                    Ce(Re);
+                    lt(A.next(he));
+                } catch (nt) {
+                    De(nt);
                 }
             }
 
-            function Se(J) {
+            function Zl(he) {
                 try {
-                    W(N.throw(J));
-                } catch (Re) {
-                    Ce(Re);
+                    lt(A.throw(he));
+                } catch (nt) {
+                    De(nt);
                 }
             }
 
-            function W(J) {
-                J.done ? ie(J.value) : Y(J.value).then(Oe, Se);
+            function lt(he) {
+                he.done ? Te(he.value) : me(he.value).then(Fl, Zl);
             }
-            W((N = N.apply(b, T || [])).next());
+            lt((A = A.apply(d, S || [])).next());
         });
     };
     let {
         value: s = ""
     } = e, {
-        value_is_output: i = !1
+        value_is_output: o = !1
     } = e, {
-        lines: f = 1
+        lines: i = 1
     } = e, {
-        placeholder: a = "Type here..."
+        placeholder: f = "Type here..."
     } = e, {
         label: r
     } = e, {
-        info: o = void 0
+        info: a = void 0
     } = e, {
         disabled: u = !1
     } = e, {
         show_label: _ = !0
     } = e, {
-        container: d = !0
+        container: c = !0
     } = e, {
         max_lines: h
     } = e, {
-        prompts: M = []
+        prompts: L = []
     } = e, {
         suffixes: H = []
     } = e, {
-        type: k = "text"
+        rtl: p = !1
     } = e, {
-        rtl: Z = !1
-    } = e, {
-        autofocus: c = !1
+        autofocus: v = !1
     } = e, {
         text_align: m = void 0
     } = e, {
-        autoscroll: p = !0
-    } = e, V, w = !1, E, j = 0, R = !1;
-    const D = oi();
-    si(() => {
-        E = V && V.offsetHeight + V.scrollTop > V.scrollHeight - 100;
+        autoscroll: b = !0
+    } = e, C, T = !1, k, N = 0, I = !1, ae = L.length > 0 || H.length > 0;
+    const j = bi();
+    mi(() => {
+        k = C && C.offsetHeight + C.scrollTop > C.scrollHeight - 100;
     });
     const le = () => {
-        E && p && !R && V.scrollTo(0, V.scrollHeight);
+        k && b && !I && C.scrollTo(0, C.scrollHeight);
     };
 
     function ne() {
-        D("change", s), i || D("input");
+        j("change", s), o || j("input");
     }
-    fi(() => {
-        c && V.focus(), E && p && le(), t(21, i = !1);
+    hi(() => {
+        v && C.focus(), k && b && le(), t(22, o = !1);
     });
 
-    function we() {
+    function ge() {
         return n(this, void 0, void 0, function*() {
-            t(14, w = !w);
+            t(14, T = !T);
         });
     }
 
-    function P(b) {
-        t(0, s += `${b} `);
+    function Y(d) {
+        t(0, s += `${d} `);
     }
 
-    function de(b) {
-        const T = b.target,
-            B = T.value,
-            N = [T.selectionStart, T.selectionEnd];
-        D("select", {
-            value: B.substring(...N),
-            index: N
+    function re(d) {
+        const S = d.target,
+            D = S.value,
+            A = [S.selectionStart, S.selectionEnd];
+        j("select", {
+            value: D.substring(...A),
+            index: A
         });
     }
 
-    function U(b) {
+    function O(d) {
         return n(this, void 0, void 0, function*() {
-            yield Mt(), (b.key === "Enter" && b.shiftKey && f > 1 || b.key === "Enter" && !b.shiftKey && f === 1 && h >= 1) && (b.preventDefault(), D("submit"));
+            yield Nt(), (d.key === "Enter" && d.shiftKey && i > 1 || d.key === "Enter" && !d.shiftKey && i === 1 && h >= 1) && (d.preventDefault(), j("submit"));
         });
     }
 
-    function ve(b) {
-        const T = b.target,
-            B = T.scrollTop;
-        B < j && (R = !0), j = B;
-        const N = T.scrollHeight - T.clientHeight;
-        B >= N && (R = !1);
+    function we(d) {
+        const S = d.target,
+            D = S.scrollTop;
+        D < N && (I = !0), N = D;
+        const A = S.scrollHeight - S.clientHeight;
+        D >= A && (I = !1);
     }
 
-    function he(b) {
+    function _e(d) {
         return n(this, void 0, void 0, function*() {
-            if (yield Mt(), f === h)
+            if (yield Nt(), i === h)
                 return;
-            let T = h === void 0 ? !1 : h === void 0 ? 21 * 11 : 21 * (h + 1),
-                B = 21 * (f + 1);
-            const N = b.target;
-            N.style.height = "1px";
-            let Y;
-            T && N.scrollHeight > T ? Y = T : N.scrollHeight < B ? Y = B : Y = N.scrollHeight, N.style.height = `${Y}px`;
+            let S = h === void 0 ? !1 : h === void 0 ? 21 * 11 : 21 * (h + 1),
+                D = 21 * (i + 1);
+            const A = d.target;
+            A.style.height = "1px";
+            let me;
+            S && A.scrollHeight > S ? me = S : A.scrollHeight < D ? me = D : me = A.scrollHeight, A.style.height = `${me}px`;
         });
     }
 
-    function ke(b, T) {
-        if (f !== h && (b.style.overflowY = "scroll", b.addEventListener("input", he), !!T.trim()))
-            return he({
-                target: b
+    function ve(d, S) {
+        if (i !== h && (d.style.overflowY = "scroll", d.addEventListener("input", _e), !!S.trim()))
+            return _e({
+                target: d
             }), {
-                destroy: () => b.removeEventListener("input", he)
+                destroy: () => d.removeEventListener("input", _e)
             };
     }
 
-    function g(b) {
-        pt.call(this, l, b);
+    function w(d) {
+        He.call(this, l, d);
+    }
+
+    function ke(d) {
+        He.call(this, l, d);
     }
 
-    function pe(b) {
-        pt.call(this, l, b);
+    function We(d) {
+        He.call(this, l, d);
     }
 
-    function Ue() {
+    function Je(d) {
+        He.call(this, l, d);
+    }
+
+    function Qe(d) {
+        He.call(this, l, d);
+    }
+
+    function y(d) {
+        He.call(this, l, d);
+    }
+
+    function xe() {
         s = this.value, t(0, s);
     }
 
-    function Xe(b) {
-        Wn[b ? "unshift" : "push"](() => {
-            V = b, t(13, V);
+    function pe(d) {
+        ot[d ? "unshift" : "push"](() => {
+            C = d, t(13, C);
         });
     }
-    const Ge = (b) => P(b),
-        v = (b) => P(b);
-    return l.$$set = (b) => {
-        "value" in b && t(0, s = b.value), "value_is_output" in b && t(21, i = b.value_is_output), "lines" in b && t(1, f = b.lines), "placeholder" in b && t(2, a = b.placeholder), "label" in b && t(3, r = b.label), "info" in b && t(4, o = b.info), "disabled" in b && t(5, u = b.disabled), "show_label" in b && t(6, _ = b.show_label), "container" in b && t(7, d = b.container), "max_lines" in b && t(22, h = b.max_lines), "prompts" in b && t(8, M = b.prompts), "suffixes" in b && t(9, H = b.suffixes), "type" in b && t(23, k = b.type), "rtl" in b && t(10, Z = b.rtl), "autofocus" in b && t(11, c = b.autofocus), "text_align" in b && t(12, m = b.text_align), "autoscroll" in b && t(24, p = b.autoscroll);
+    const Ce = (d) => Y(d),
+        $e = (d) => Y(d);
+
+    function de() {
+        s = this.value, t(0, s);
+    }
+
+    function ye(d) {
+        ot[d ? "unshift" : "push"](() => {
+            C = d, t(13, C);
+        });
+    }
+
+    function et() {
+        s = this.value, t(0, s);
+    }
+
+    function tt(d) {
+        ot[d ? "unshift" : "push"](() => {
+            C = d, t(13, C);
+        });
+    }
+    return l.$$set = (d) => {
+        "value" in d && t(0, s = d.value), "value_is_output" in d && t(22, o = d.value_is_output), "lines" in d && t(1, i = d.lines), "placeholder" in d && t(2, f = d.placeholder), "label" in d && t(3, r = d.label), "info" in d && t(4, a = d.info), "disabled" in d && t(5, u = d.disabled), "show_label" in d && t(6, _ = d.show_label), "container" in d && t(7, c = d.container), "max_lines" in d && t(23, h = d.max_lines), "prompts" in d && t(8, L = d.prompts), "suffixes" in d && t(9, H = d.suffixes), "rtl" in d && t(10, p = d.rtl), "autofocus" in d && t(11, v = d.autofocus), "text_align" in d && t(12, m = d.text_align), "autoscroll" in d && t(24, b = d.autoscroll);
     }, l.$$.update = () => {
         l.$$.dirty[0] & /*value*/
             1 && s === null && t(0, s = ""), l.$$.dirty[0] & /*value, el, lines, max_lines*/
-            4202499 && V && f !== h && he({
-                target: V
+            8396803 && C && i !== h && _e({
+                target: C
             }), l.$$.dirty[0] & /*value*/
             1 && ne();
     }, [
         s,
+        i,
         f,
-        a,
         r,
-        o,
+        a,
         u,
         _,
-        d,
-        M,
-        H,
-        Z,
         c,
+        L,
+        H,
+        p,
+        v,
         m,
-        V,
-        w,
+        C,
+        T,
+        ae,
+        ge,
+        Y,
+        re,
+        O,
         we,
-        P,
-        de,
-        U,
         ve,
-        ke,
-        i,
+        o,
         h,
-        k,
-        p,
-        g,
+        b,
+        w,
+        ke,
+        We,
+        Je,
+        Qe,
+        y,
+        xe,
         pe,
-        Ue,
-        Xe,
-        Ge,
-        v
+        Ce,
+        $e,
+        de,
+        ye,
+        et,
+        tt
     ];
 }
-class di extends Gn {
+class yi extends si {
     constructor(e) {
-        super(), ei(
+        super(), _i(
             this,
             e,
-            ci,
-            _i,
-            ii, {
+            Ci,
+            pi,
+            di, {
                 value: 0,
-                value_is_output: 21,
+                value_is_output: 22,
                 lines: 1,
                 placeholder: 2,
                 label: 3,
                 info: 4,
                 disabled: 5,
                 show_label: 6,
                 container: 7,
-                max_lines: 22,
+                max_lines: 23,
                 prompts: 8,
                 suffixes: 9,
-                type: 23,
                 rtl: 10,
                 autofocus: 11,
                 text_align: 12,
                 autoscroll: 24
             },
             null,
             [-1, -1]
         );
     }
 }
 
-function qe(l) {
+function Fe(l) {
     let e = ["", "k", "M", "G", "T", "P", "E", "Z"],
         t = 0;
     for (; l > 1e3 && t < e.length - 1;)
         l /= 1e3, t++;
     let n = e[t];
     return (Number.isInteger(l) ? l : l.toFixed(1)) + n;
 }
 const {
-    SvelteComponent: mi,
-    append: x,
+    SvelteComponent: Li,
+    append: W,
     attr: q,
-    component_subscribe: zt,
-    detach: hi,
-    element: bi,
-    init: gi,
-    insert: wi,
-    noop: Et,
-    safe_not_equal: vi,
-    set_style: Be,
-    svg_element: $,
-    toggle_class: Tt
+    component_subscribe: Kt,
+    detach: Mi,
+    element: Vi,
+    init: Hi,
+    insert: qi,
+    noop: Ot,
+    safe_not_equal: Fi,
+    set_style: je,
+    svg_element: J,
+    toggle_class: Ut
 } = window.__gradio__svelte__internal, {
-    onMount: ki
+    onMount: Zi
 } = window.__gradio__svelte__internal;
 
-function pi(l) {
-    let e, t, n, s, i, f, a, r, o, u, _, d;
+function Si(l) {
+    let e, t, n, s, o, i, f, r, a, u, _, c;
     return {
         c() {
-            e = bi("div"), t = $("svg"), n = $("g"), s = $("path"), i = $("path"), f = $("path"), a = $("path"), r = $("g"), o = $("path"), u = $("path"), _ = $("path"), d = $("path"), q(s, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), q(s, "fill", "#FF7C00"), q(s, "fill-opacity", "0.4"), q(s, "class", "svelte-43sxxs"), q(i, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), q(i, "fill", "#FF7C00"), q(i, "class", "svelte-43sxxs"), q(f, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), q(f, "fill", "#FF7C00"), q(f, "fill-opacity", "0.4"), q(f, "class", "svelte-43sxxs"), q(a, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), q(a, "fill", "#FF7C00"), q(a, "class", "svelte-43sxxs"), Be(n, "transform", "translate(" + /*$top*/
+            e = Vi("div"), t = J("svg"), n = J("g"), s = J("path"), o = J("path"), i = J("path"), f = J("path"), r = J("g"), a = J("path"), u = J("path"), _ = J("path"), c = J("path"), q(s, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), q(s, "fill", "#FF7C00"), q(s, "fill-opacity", "0.4"), q(s, "class", "svelte-43sxxs"), q(o, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), q(o, "fill", "#FF7C00"), q(o, "class", "svelte-43sxxs"), q(i, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), q(i, "fill", "#FF7C00"), q(i, "fill-opacity", "0.4"), q(i, "class", "svelte-43sxxs"), q(f, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), q(f, "fill", "#FF7C00"), q(f, "class", "svelte-43sxxs"), je(n, "transform", "translate(" + /*$top*/
                 l[1][0] + "px, " + /*$top*/
-                l[1][1] + "px)"), q(o, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), q(o, "fill", "#FF7C00"), q(o, "fill-opacity", "0.4"), q(o, "class", "svelte-43sxxs"), q(u, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), q(u, "fill", "#FF7C00"), q(u, "class", "svelte-43sxxs"), q(_, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), q(_, "fill", "#FF7C00"), q(_, "fill-opacity", "0.4"), q(_, "class", "svelte-43sxxs"), q(d, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), q(d, "fill", "#FF7C00"), q(d, "class", "svelte-43sxxs"), Be(r, "transform", "translate(" + /*$bottom*/
+                l[1][1] + "px)"), q(a, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), q(a, "fill", "#FF7C00"), q(a, "fill-opacity", "0.4"), q(a, "class", "svelte-43sxxs"), q(u, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), q(u, "fill", "#FF7C00"), q(u, "class", "svelte-43sxxs"), q(_, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), q(_, "fill", "#FF7C00"), q(_, "fill-opacity", "0.4"), q(_, "class", "svelte-43sxxs"), q(c, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), q(c, "fill", "#FF7C00"), q(c, "class", "svelte-43sxxs"), je(r, "transform", "translate(" + /*$bottom*/
                 l[2][0] + "px, " + /*$bottom*/
-                l[2][1] + "px)"), q(t, "viewBox", "-1200 -1200 3000 3000"), q(t, "fill", "none"), q(t, "xmlns", "http://www.w3.org/2000/svg"), q(t, "class", "svelte-43sxxs"), q(e, "class", "svelte-43sxxs"), Tt(
+                l[2][1] + "px)"), q(t, "viewBox", "-1200 -1200 3000 3000"), q(t, "fill", "none"), q(t, "xmlns", "http://www.w3.org/2000/svg"), q(t, "class", "svelte-43sxxs"), q(e, "class", "svelte-43sxxs"), Ut(
                 e,
                 "margin",
                 /*margin*/
                 l[0]
             );
         },
-        m(h, M) {
-            wi(h, e, M), x(e, t), x(t, n), x(n, s), x(n, i), x(n, f), x(n, a), x(t, r), x(r, o), x(r, u), x(r, _), x(r, d);
+        m(h, L) {
+            qi(h, e, L), W(e, t), W(t, n), W(n, s), W(n, o), W(n, i), W(n, f), W(t, r), W(r, a), W(r, u), W(r, _), W(r, c);
         },
-        p(h, [M]) {
-            M & /*$top*/
-                2 && Be(n, "transform", "translate(" + /*$top*/
+        p(h, [L]) {
+            L & /*$top*/
+                2 && je(n, "transform", "translate(" + /*$top*/
                     h[1][0] + "px, " + /*$top*/
-                    h[1][1] + "px)"), M & /*$bottom*/
-                4 && Be(r, "transform", "translate(" + /*$bottom*/
+                    h[1][1] + "px)"), L & /*$bottom*/
+                4 && je(r, "transform", "translate(" + /*$bottom*/
                     h[2][0] + "px, " + /*$bottom*/
-                    h[2][1] + "px)"), M & /*margin*/
-                1 && Tt(
+                    h[2][1] + "px)"), L & /*margin*/
+                1 && Ut(
                     e,
                     "margin",
                     /*margin*/
                     h[0]
                 );
         },
-        i: Et,
-        o: Et,
+        i: Ot,
+        o: Ot,
         d(h) {
-            h && hi(e);
+            h && Mi(e);
         }
     };
 }
 
-function Ci(l, e, t) {
+function zi(l, e, t) {
     let n, s;
-    var i = this && this.__awaiter || function(h, M, H, k) {
-        function Z(c) {
-            return c instanceof H ? c : new H(function(m) {
-                m(c);
+    var o = this && this.__awaiter || function(h, L, H, p) {
+        function v(m) {
+            return m instanceof H ? m : new H(function(b) {
+                b(m);
             });
         }
-        return new(H || (H = Promise))(function(c, m) {
-            function p(E) {
+        return new(H || (H = Promise))(function(m, b) {
+            function C(N) {
                 try {
-                    w(k.next(E));
-                } catch (j) {
-                    m(j);
+                    k(p.next(N));
+                } catch (I) {
+                    b(I);
                 }
             }
 
-            function V(E) {
+            function T(N) {
                 try {
-                    w(k.throw(E));
-                } catch (j) {
-                    m(j);
+                    k(p.throw(N));
+                } catch (I) {
+                    b(I);
                 }
             }
 
-            function w(E) {
-                E.done ? c(E.value) : Z(E.value).then(p, V);
+            function k(N) {
+                N.done ? m(N.value) : v(N.value).then(C, T);
             }
-            w((k = k.apply(h, M || [])).next());
+            k((p = p.apply(h, L || [])).next());
         });
     };
     let {
-        margin: f = !0
+        margin: i = !0
     } = e;
-    const a = kt([0, 0]);
-    zt(l, a, (h) => t(1, n = h));
-    const r = kt([0, 0]);
-    zt(l, r, (h) => t(2, s = h));
-    let o;
+    const f = zt([0, 0]);
+    Kt(l, f, (h) => t(1, n = h));
+    const r = zt([0, 0]);
+    Kt(l, r, (h) => t(2, s = h));
+    let a;
 
     function u() {
-        return i(this, void 0, void 0, function*() {
-            yield Promise.all([a.set([125, 140]), r.set([-125, -140])]), yield Promise.all([a.set([-125, 140]), r.set([125, -140])]), yield Promise.all([a.set([-125, 0]), r.set([125, -0])]), yield Promise.all([a.set([125, 0]), r.set([-125, 0])]);
+        return o(this, void 0, void 0, function*() {
+            yield Promise.all([f.set([125, 140]), r.set([-125, -140])]), yield Promise.all([f.set([-125, 140]), r.set([125, -140])]), yield Promise.all([f.set([-125, 0]), r.set([125, -0])]), yield Promise.all([f.set([125, 0]), r.set([-125, 0])]);
         });
     }
 
     function _() {
-        return i(this, void 0, void 0, function*() {
-            yield u(), o || _();
+        return o(this, void 0, void 0, function*() {
+            yield u(), a || _();
         });
     }
 
-    function d() {
-        return i(this, void 0, void 0, function*() {
-            yield Promise.all([a.set([125, 0]), r.set([-125, 0])]), _();
+    function c() {
+        return o(this, void 0, void 0, function*() {
+            yield Promise.all([f.set([125, 0]), r.set([-125, 0])]), _();
         });
     }
-    return ki(() => (d(), () => o = !0)), l.$$set = (h) => {
-        "margin" in h && t(0, f = h.margin);
-    }, [f, n, s, a, r];
+    return Zi(() => (c(), () => a = !0)), l.$$set = (h) => {
+        "margin" in h && t(0, i = h.margin);
+    }, [i, n, s, f, r];
 }
-class yi extends mi {
+class Ei extends Li {
     constructor(e) {
-        super(), gi(this, e, Ci, pi, vi, {
+        super(), Hi(this, e, zi, Si, Fi, {
             margin: 0
         });
     }
 }
 const {
-    SvelteComponent: Li,
-    append: ge,
-    attr: te,
-    binding_callbacks: Bt,
-    check_outros: it,
-    create_component: ul,
-    create_slot: _l,
-    destroy_component: cl,
-    destroy_each: dl,
-    detach: y,
-    element: ae,
-    empty: Fe,
-    ensure_array_like: Ke,
-    get_all_dirty_from_scope: ml,
-    get_slot_changes: hl,
-    group_outros: st,
-    init: Mi,
-    insert: L,
-    mount_component: bl,
-    noop: ft,
-    safe_not_equal: Vi,
-    set_data: O,
-    set_style: be,
-    space: G,
+    SvelteComponent: Ti,
+    append: be,
+    attr: x,
+    binding_callbacks: Xt,
+    check_outros: dt,
+    create_component: pl,
+    create_slot: Cl,
+    destroy_component: yl,
+    destroy_each: Ll,
+    detach: M,
+    element: oe,
+    empty: Ee,
+    ensure_array_like: Re,
+    get_all_dirty_from_scope: Ml,
+    get_slot_changes: Vl,
+    group_outros: mt,
+    init: Bi,
+    insert: V,
+    mount_component: Hl,
+    noop: ht,
+    safe_not_equal: Ni,
+    set_data: G,
+    set_style: ce,
+    space: X,
     text: z,
-    toggle_class: X,
-    transition_in: ee,
-    transition_out: re,
-    update_slot_base: gl
+    toggle_class: U,
+    transition_in: Q,
+    transition_out: fe,
+    update_slot_base: ql
 } = window.__gradio__svelte__internal, {
-    tick: qi
+    tick: Di
 } = window.__gradio__svelte__internal, {
-    onDestroy: Hi
+    onDestroy: Ii
 } = window.__gradio__svelte__internal, {
-    createEventDispatcher: Zi
-} = window.__gradio__svelte__internal, Fi = (l) => ({}), Nt = (l) => ({}), Si = (l) => ({}), Dt = (l) => ({});
+    createEventDispatcher: ji
+} = window.__gradio__svelte__internal, Ai = (l) => ({}), Gt = (l) => ({}), Pi = (l) => ({}), Rt = (l) => ({});
 
-function It(l, e, t) {
+function Wt(l, e, t) {
     const n = l.slice();
     return n[41] = e[t], n[43] = t, n;
 }
 
-function jt(l, e, t) {
+function Jt(l, e, t) {
     const n = l.slice();
     return n[41] = e[t], n;
 }
 
-function zi(l) {
-    let e, t, n, s, i = (
+function Yi(l) {
+    let e, t, n, s, o = (
             /*i18n*/
             l[1]("common.error") + ""
         ),
-        f, a, r;
-    t = new En({
+        i, f, r;
+    t = new Xn({
         props: {
-            Icon: An,
+            Icon: $n,
             label: (
                 /*i18n*/
                 l[1]("common.clear")
             ),
             disabled: !1
         }
     }), t.$on(
         "click",
         /*click_handler*/
         l[32]
     );
-    const o = (
+    const a = (
             /*#slots*/
             l[30].error
         ),
-        u = _l(
-            o,
+        u = Cl(
+            a,
             l,
             /*$$scope*/
             l[29],
-            Nt
+            Gt
         );
     return {
         c() {
-            e = ae("div"), ul(t.$$.fragment), n = G(), s = ae("span"), f = z(i), a = G(), u && u.c(), te(e, "class", "clear-status svelte-vopvsi"), te(s, "class", "error svelte-vopvsi");
+            e = oe("div"), pl(t.$$.fragment), n = X(), s = oe("span"), i = z(o), f = X(), u && u.c(), x(e, "class", "clear-status svelte-vopvsi"), x(s, "class", "error svelte-vopvsi");
         },
-        m(_, d) {
-            L(_, e, d), bl(t, e, null), L(_, n, d), L(_, s, d), ge(s, f), L(_, a, d), u && u.m(_, d), r = !0;
+        m(_, c) {
+            V(_, e, c), Hl(t, e, null), V(_, n, c), V(_, s, c), be(s, i), V(_, f, c), u && u.m(_, c), r = !0;
         },
-        p(_, d) {
+        p(_, c) {
             const h = {};
-            d[0] & /*i18n*/
+            c[0] & /*i18n*/
                 2 && (h.label = /*i18n*/
-                    _[1]("common.clear")), t.$set(h), (!r || d[0] & /*i18n*/
-                    2) && i !== (i = /*i18n*/
-                    _[1]("common.error") + "") && O(f, i), u && u.p && (!r || d[0] & /*$$scope*/
-                    536870912) && gl(
+                    _[1]("common.clear")), t.$set(h), (!r || c[0] & /*i18n*/
+                    2) && o !== (o = /*i18n*/
+                    _[1]("common.error") + "") && G(i, o), u && u.p && (!r || c[0] & /*$$scope*/
+                    536870912) && ql(
                     u,
-                    o,
+                    a,
                     _,
                     /*$$scope*/
                     _[29],
-                    r ? hl(
-                        o,
+                    r ? Vl(
+                        a,
                         /*$$scope*/
                         _[29],
-                        d,
-                        Fi
-                    ) : ml(
+                        c,
+                        Ai
+                    ) : Ml(
                         /*$$scope*/
                         _[29]
                     ),
-                    Nt
+                    Gt
                 );
         },
         i(_) {
-            r || (ee(t.$$.fragment, _), ee(u, _), r = !0);
+            r || (Q(t.$$.fragment, _), Q(u, _), r = !0);
         },
         o(_) {
-            re(t.$$.fragment, _), re(u, _), r = !1;
+            fe(t.$$.fragment, _), fe(u, _), r = !1;
         },
         d(_) {
-            _ && (y(e), y(n), y(s), y(a)), cl(t), u && u.d(_);
+            _ && (M(e), M(n), M(s), M(f)), yl(t), u && u.d(_);
         }
     };
 }
 
-function Ei(l) {
-    let e, t, n, s, i, f, a, r, o, u = (
+function Ki(l) {
+    let e, t, n, s, o, i, f, r, a, u = (
         /*variant*/
         l[8] === "default" && /*show_eta_bar*/
         l[18] && /*show_progress*/
-        l[6] === "full" && At(l)
+        l[6] === "full" && Qt(l)
     );
 
-    function _(m, p) {
+    function _(b, C) {
         if (
             /*progress*/
-            m[7]
+            b[7]
         )
-            return Ni;
+            return Xi;
         if (
             /*queue_position*/
-            m[2] !== null && /*queue_size*/
-            m[3] !== void 0 && /*queue_position*/
-            m[2] >= 0
+            b[2] !== null && /*queue_size*/
+            b[3] !== void 0 && /*queue_position*/
+            b[2] >= 0
         )
-            return Bi;
+            return Ui;
         if (
             /*queue_position*/
-            m[2] === 0
+            b[2] === 0
         )
-            return Ti;
+            return Oi;
     }
-    let d = _(l),
-        h = d && d(l),
-        M = (
+    let c = _(l),
+        h = c && c(l),
+        L = (
             /*timer*/
-            l[5] && Kt(l)
+            l[5] && el(l)
         );
-    const H = [Ai, ji],
-        k = [];
+    const H = [Ji, Wi],
+        p = [];
 
-    function Z(m, p) {
+    function v(b, C) {
         return (
             /*last_progress_level*/
-            m[15] != null ? 0 : (
+            b[15] != null ? 0 : (
                 /*show_progress*/
-                m[6] === "full" ? 1 : -1
+                b[6] === "full" ? 1 : -1
             )
         );
     }
-    ~(i = Z(l)) && (f = k[i] = H[i](l));
-    let c = ! /*timer*/
-        l[5] && Jt(l);
+    ~(o = v(l)) && (i = p[o] = H[o](l));
+    let m = ! /*timer*/
+        l[5] && fl(l);
     return {
         c() {
-            u && u.c(), e = G(), t = ae("div"), h && h.c(), n = G(), M && M.c(), s = G(), f && f.c(), a = G(), c && c.c(), r = Fe(), te(t, "class", "progress-text svelte-vopvsi"), X(
+            u && u.c(), e = X(), t = oe("div"), h && h.c(), n = X(), L && L.c(), s = X(), i && i.c(), f = X(), m && m.c(), r = Ee(), x(t, "class", "progress-text svelte-vopvsi"), U(
                 t,
                 "meta-text-center",
                 /*variant*/
                 l[8] === "center"
-            ), X(
+            ), U(
                 t,
                 "meta-text",
                 /*variant*/
                 l[8] === "default"
             );
         },
-        m(m, p) {
-            u && u.m(m, p), L(m, e, p), L(m, t, p), h && h.m(t, null), ge(t, n), M && M.m(t, null), L(m, s, p), ~i && k[i].m(m, p), L(m, a, p), c && c.m(m, p), L(m, r, p), o = !0;
+        m(b, C) {
+            u && u.m(b, C), V(b, e, C), V(b, t, C), h && h.m(t, null), be(t, n), L && L.m(t, null), V(b, s, C), ~o && p[o].m(b, C), V(b, f, C), m && m.m(b, C), V(b, r, C), a = !0;
         },
-        p(m, p) {
+        p(b, C) {
             /*variant*/
-            m[8] === "default" && /*show_eta_bar*/
-                m[18] && /*show_progress*/
-                m[6] === "full" ? u ? u.p(m, p) : (u = At(m), u.c(), u.m(e.parentNode, e)) : u && (u.d(1), u = null), d === (d = _(m)) && h ? h.p(m, p) : (h && h.d(1), h = d && d(m), h && (h.c(), h.m(t, n))), /*timer*/
-                m[5] ? M ? M.p(m, p) : (M = Kt(m), M.c(), M.m(t, null)) : M && (M.d(1), M = null), (!o || p[0] & /*variant*/
-                    256) && X(
+            b[8] === "default" && /*show_eta_bar*/
+                b[18] && /*show_progress*/
+                b[6] === "full" ? u ? u.p(b, C) : (u = Qt(b), u.c(), u.m(e.parentNode, e)) : u && (u.d(1), u = null), c === (c = _(b)) && h ? h.p(b, C) : (h && h.d(1), h = c && c(b), h && (h.c(), h.m(t, n))), /*timer*/
+                b[5] ? L ? L.p(b, C) : (L = el(b), L.c(), L.m(t, null)) : L && (L.d(1), L = null), (!a || C[0] & /*variant*/
+                    256) && U(
                     t,
                     "meta-text-center",
                     /*variant*/
-                    m[8] === "center"
-                ), (!o || p[0] & /*variant*/
-                    256) && X(
+                    b[8] === "center"
+                ), (!a || C[0] & /*variant*/
+                    256) && U(
                     t,
                     "meta-text",
                     /*variant*/
-                    m[8] === "default"
+                    b[8] === "default"
                 );
-            let V = i;
-            i = Z(m), i === V ? ~i && k[i].p(m, p) : (f && (st(), re(k[V], 1, 1, () => {
-                    k[V] = null;
-                }), it()), ~i ? (f = k[i], f ? f.p(m, p) : (f = k[i] = H[i](m), f.c()), ee(f, 1), f.m(a.parentNode, a)) : f = null), /*timer*/
-                m[5] ? c && (st(), re(c, 1, 1, () => {
-                    c = null;
-                }), it()) : c ? (c.p(m, p), p[0] & /*timer*/
-                    32 && ee(c, 1)) : (c = Jt(m), c.c(), ee(c, 1), c.m(r.parentNode, r));
+            let T = o;
+            o = v(b), o === T ? ~o && p[o].p(b, C) : (i && (mt(), fe(p[T], 1, 1, () => {
+                    p[T] = null;
+                }), dt()), ~o ? (i = p[o], i ? i.p(b, C) : (i = p[o] = H[o](b), i.c()), Q(i, 1), i.m(f.parentNode, f)) : i = null), /*timer*/
+                b[5] ? m && (mt(), fe(m, 1, 1, () => {
+                    m = null;
+                }), dt()) : m ? (m.p(b, C), C[0] & /*timer*/
+                    32 && Q(m, 1)) : (m = fl(b), m.c(), Q(m, 1), m.m(r.parentNode, r));
         },
-        i(m) {
-            o || (ee(f), ee(c), o = !0);
+        i(b) {
+            a || (Q(i), Q(m), a = !0);
         },
-        o(m) {
-            re(f), re(c), o = !1;
+        o(b) {
+            fe(i), fe(m), a = !1;
         },
-        d(m) {
-            m && (y(e), y(t), y(s), y(a), y(r)), u && u.d(m), h && h.d(), M && M.d(), ~i && k[i].d(m), c && c.d(m);
+        d(b) {
+            b && (M(e), M(t), M(s), M(f), M(r)), u && u.d(b), h && h.d(), L && L.d(), ~o && p[o].d(b), m && m.d(b);
         }
     };
 }
 
-function At(l) {
+function Qt(l) {
     let e, t = `translateX(${/*eta_level*/
   (l[17] || 0) * 100 - 100}%)`;
     return {
         c() {
-            e = ae("div"), te(e, "class", "eta-bar svelte-vopvsi"), be(e, "transform", t);
+            e = oe("div"), x(e, "class", "eta-bar svelte-vopvsi"), ce(e, "transform", t);
         },
         m(n, s) {
-            L(n, e, s);
+            V(n, e, s);
         },
         p(n, s) {
             s[0] & /*eta_level*/
                 131072 && t !== (t = `translateX(${/*eta_level*/
-      (n[17] || 0) * 100 - 100}%)`) && be(e, "transform", t);
+      (n[17] || 0) * 100 - 100}%)`) && ce(e, "transform", t);
         },
         d(n) {
-            n && y(e);
+            n && M(e);
         }
     };
 }
 
-function Ti(l) {
+function Oi(l) {
     let e;
     return {
         c() {
             e = z("processing |");
         },
         m(t, n) {
-            L(t, e, n);
+            V(t, e, n);
         },
-        p: ft,
+        p: ht,
         d(t) {
-            t && y(e);
+            t && M(e);
         }
     };
 }
 
-function Bi(l) {
+function Ui(l) {
     let e, t = (
             /*queue_position*/
             l[2] + 1 + ""
         ),
-        n, s, i, f;
+        n, s, o, i;
     return {
         c() {
-            e = z("queue: "), n = z(t), s = z("/"), i = z(
+            e = z("queue: "), n = z(t), s = z("/"), o = z(
                 /*queue_size*/
                 l[3]
-            ), f = z(" |");
+            ), i = z(" |");
         },
-        m(a, r) {
-            L(a, e, r), L(a, n, r), L(a, s, r), L(a, i, r), L(a, f, r);
+        m(f, r) {
+            V(f, e, r), V(f, n, r), V(f, s, r), V(f, o, r), V(f, i, r);
         },
-        p(a, r) {
+        p(f, r) {
             r[0] & /*queue_position*/
                 4 && t !== (t = /*queue_position*/
-                    a[2] + 1 + "") && O(n, t), r[0] & /*queue_size*/
-                8 && O(
-                    i,
+                    f[2] + 1 + "") && G(n, t), r[0] & /*queue_size*/
+                8 && G(
+                    o,
                     /*queue_size*/
-                    a[3]
+                    f[3]
                 );
         },
-        d(a) {
-            a && (y(e), y(n), y(s), y(i), y(f));
+        d(f) {
+            f && (M(e), M(n), M(s), M(o), M(i));
         }
     };
 }
 
-function Ni(l) {
-    let e, t = Ke(
+function Xi(l) {
+    let e, t = Re(
             /*progress*/
             l[7]
         ),
         n = [];
     for (let s = 0; s < t.length; s += 1)
-        n[s] = Yt(jt(l, t, s));
+        n[s] = $t(Jt(l, t, s));
     return {
         c() {
             for (let s = 0; s < n.length; s += 1)
                 n[s].c();
-            e = Fe();
+            e = Ee();
         },
-        m(s, i) {
-            for (let f = 0; f < n.length; f += 1)
-                n[f] && n[f].m(s, i);
-            L(s, e, i);
+        m(s, o) {
+            for (let i = 0; i < n.length; i += 1)
+                n[i] && n[i].m(s, o);
+            V(s, e, o);
         },
-        p(s, i) {
-            if (i[0] & /*progress*/
+        p(s, o) {
+            if (o[0] & /*progress*/
                 128) {
-                t = Ke(
+                t = Re(
                     /*progress*/
                     s[7]
                 );
-                let f;
-                for (f = 0; f < t.length; f += 1) {
-                    const a = jt(s, t, f);
-                    n[f] ? n[f].p(a, i) : (n[f] = Yt(a), n[f].c(), n[f].m(e.parentNode, e));
+                let i;
+                for (i = 0; i < t.length; i += 1) {
+                    const f = Jt(s, t, i);
+                    n[i] ? n[i].p(f, o) : (n[i] = $t(f), n[i].c(), n[i].m(e.parentNode, e));
                 }
-                for (; f < n.length; f += 1)
-                    n[f].d(1);
+                for (; i < n.length; i += 1)
+                    n[i].d(1);
                 n.length = t.length;
             }
         },
         d(s) {
-            s && y(e), dl(n, s);
+            s && M(e), Ll(n, s);
         }
     };
 }
 
-function Pt(l) {
+function xt(l) {
     let e, t = (
             /*p*/
             l[41].unit + ""
         ),
-        n, s, i = " ",
-        f;
+        n, s, o = " ",
+        i;
 
-    function a(u, _) {
+    function f(u, _) {
         return (
             /*p*/
-            u[41].length != null ? Ii : Di
+            u[41].length != null ? Ri : Gi
         );
     }
-    let r = a(l),
-        o = r(l);
+    let r = f(l),
+        a = r(l);
     return {
         c() {
-            o.c(), e = G(), n = z(t), s = z(" | "), f = z(i);
+            a.c(), e = X(), n = z(t), s = z(" | "), i = z(o);
         },
         m(u, _) {
-            o.m(u, _), L(u, e, _), L(u, n, _), L(u, s, _), L(u, f, _);
+            a.m(u, _), V(u, e, _), V(u, n, _), V(u, s, _), V(u, i, _);
         },
         p(u, _) {
-            r === (r = a(u)) && o ? o.p(u, _) : (o.d(1), o = r(u), o && (o.c(), o.m(e.parentNode, e))), _[0] & /*progress*/
+            r === (r = f(u)) && a ? a.p(u, _) : (a.d(1), a = r(u), a && (a.c(), a.m(e.parentNode, e))), _[0] & /*progress*/
                 128 && t !== (t = /*p*/
-                    u[41].unit + "") && O(n, t);
+                    u[41].unit + "") && G(n, t);
         },
         d(u) {
-            u && (y(e), y(n), y(s), y(f)), o.d(u);
+            u && (M(e), M(n), M(s), M(i)), a.d(u);
         }
     };
 }
 
-function Di(l) {
-    let e = qe(
+function Gi(l) {
+    let e = Fe(
             /*p*/
             l[41].index || 0
         ) + "",
         t;
     return {
         c() {
             t = z(e);
         },
         m(n, s) {
-            L(n, t, s);
+            V(n, t, s);
         },
         p(n, s) {
             s[0] & /*progress*/
-                128 && e !== (e = qe(
+                128 && e !== (e = Fe(
                     /*p*/
                     n[41].index || 0
-                ) + "") && O(t, e);
+                ) + "") && G(t, e);
         },
         d(n) {
-            n && y(t);
+            n && M(t);
         }
     };
 }
 
-function Ii(l) {
-    let e = qe(
+function Ri(l) {
+    let e = Fe(
             /*p*/
             l[41].index || 0
         ) + "",
-        t, n, s = qe(
+        t, n, s = Fe(
             /*p*/
             l[41].length
         ) + "",
-        i;
+        o;
     return {
         c() {
-            t = z(e), n = z("/"), i = z(s);
+            t = z(e), n = z("/"), o = z(s);
         },
-        m(f, a) {
-            L(f, t, a), L(f, n, a), L(f, i, a);
+        m(i, f) {
+            V(i, t, f), V(i, n, f), V(i, o, f);
         },
-        p(f, a) {
-            a[0] & /*progress*/
-                128 && e !== (e = qe(
+        p(i, f) {
+            f[0] & /*progress*/
+                128 && e !== (e = Fe(
                     /*p*/
-                    f[41].index || 0
-                ) + "") && O(t, e), a[0] & /*progress*/
-                128 && s !== (s = qe(
+                    i[41].index || 0
+                ) + "") && G(t, e), f[0] & /*progress*/
+                128 && s !== (s = Fe(
                     /*p*/
-                    f[41].length
-                ) + "") && O(i, s);
+                    i[41].length
+                ) + "") && G(o, s);
         },
-        d(f) {
-            f && (y(t), y(n), y(i));
+        d(i) {
+            i && (M(t), M(n), M(o));
         }
     };
 }
 
-function Yt(l) {
+function $t(l) {
     let e, t = (
         /*p*/
-        l[41].index != null && Pt(l)
+        l[41].index != null && xt(l)
     );
     return {
         c() {
-            t && t.c(), e = Fe();
+            t && t.c(), e = Ee();
         },
         m(n, s) {
-            t && t.m(n, s), L(n, e, s);
+            t && t.m(n, s), V(n, e, s);
         },
         p(n, s) {
             /*p*/
-            n[41].index != null ? t ? t.p(n, s) : (t = Pt(n), t.c(), t.m(e.parentNode, e)) : t && (t.d(1), t = null);
+            n[41].index != null ? t ? t.p(n, s) : (t = xt(n), t.c(), t.m(e.parentNode, e)) : t && (t.d(1), t = null);
         },
         d(n) {
-            n && y(e), t && t.d(n);
+            n && M(e), t && t.d(n);
         }
     };
 }
 
-function Kt(l) {
+function el(l) {
     let e, t = (
             /*eta*/
             l[0] ? `/${/*formatted_eta*/
     l[19]}` : ""
         ),
         n, s;
     return {
         c() {
             e = z(
                 /*formatted_timer*/
                 l[20]
             ), n = z(t), s = z("s");
         },
-        m(i, f) {
-            L(i, e, f), L(i, n, f), L(i, s, f);
+        m(o, i) {
+            V(o, e, i), V(o, n, i), V(o, s, i);
         },
-        p(i, f) {
-            f[0] & /*formatted_timer*/
-                1048576 && O(
+        p(o, i) {
+            i[0] & /*formatted_timer*/
+                1048576 && G(
                     e,
                     /*formatted_timer*/
-                    i[20]
-                ), f[0] & /*eta, formatted_eta*/
+                    o[20]
+                ), i[0] & /*eta, formatted_eta*/
                 524289 && t !== (t = /*eta*/
-                    i[0] ? `/${/*formatted_eta*/
-      i[19]}` : "") && O(n, t);
+                    o[0] ? `/${/*formatted_eta*/
+      o[19]}` : "") && G(n, t);
         },
-        d(i) {
-            i && (y(e), y(n), y(s));
+        d(o) {
+            o && (M(e), M(n), M(s));
         }
     };
 }
 
-function ji(l) {
+function Wi(l) {
     let e, t;
-    return e = new yi({
+    return e = new Ei({
         props: {
             margin: (
                 /*variant*/
                 l[8] === "default"
             )
         }
     }), {
         c() {
-            ul(e.$$.fragment);
+            pl(e.$$.fragment);
         },
         m(n, s) {
-            bl(e, n, s), t = !0;
+            Hl(e, n, s), t = !0;
         },
         p(n, s) {
-            const i = {};
+            const o = {};
             s[0] & /*variant*/
-                256 && (i.margin = /*variant*/
-                    n[8] === "default"), e.$set(i);
+                256 && (o.margin = /*variant*/
+                    n[8] === "default"), e.$set(o);
         },
         i(n) {
-            t || (ee(e.$$.fragment, n), t = !0);
+            t || (Q(e.$$.fragment, n), t = !0);
         },
         o(n) {
-            re(e.$$.fragment, n), t = !1;
+            fe(e.$$.fragment, n), t = !1;
         },
         d(n) {
-            cl(e, n);
+            yl(e, n);
         }
     };
 }
 
-function Ai(l) {
-    let e, t, n, s, i, f = `${/*last_progress_level*/
+function Ji(l) {
+    let e, t, n, s, o, i = `${/*last_progress_level*/
   l[15] * 100}%`,
-        a = (
+        f = (
             /*progress*/
-            l[7] != null && Ut(l)
+            l[7] != null && tl(l)
         );
     return {
         c() {
-            e = ae("div"), t = ae("div"), a && a.c(), n = G(), s = ae("div"), i = ae("div"), te(t, "class", "progress-level-inner svelte-vopvsi"), te(i, "class", "progress-bar svelte-vopvsi"), be(i, "width", f), te(s, "class", "progress-bar-wrap svelte-vopvsi"), te(e, "class", "progress-level svelte-vopvsi");
+            e = oe("div"), t = oe("div"), f && f.c(), n = X(), s = oe("div"), o = oe("div"), x(t, "class", "progress-level-inner svelte-vopvsi"), x(o, "class", "progress-bar svelte-vopvsi"), ce(o, "width", i), x(s, "class", "progress-bar-wrap svelte-vopvsi"), x(e, "class", "progress-level svelte-vopvsi");
         },
-        m(r, o) {
-            L(r, e, o), ge(e, t), a && a.m(t, null), ge(e, n), ge(e, s), ge(s, i), l[31](i);
+        m(r, a) {
+            V(r, e, a), be(e, t), f && f.m(t, null), be(e, n), be(e, s), be(s, o), l[31](o);
         },
-        p(r, o) {
+        p(r, a) {
             /*progress*/
-            r[7] != null ? a ? a.p(r, o) : (a = Ut(r), a.c(), a.m(t, null)) : a && (a.d(1), a = null), o[0] & /*last_progress_level*/
-                32768 && f !== (f = `${/*last_progress_level*/
-      r[15] * 100}%`) && be(i, "width", f);
+            r[7] != null ? f ? f.p(r, a) : (f = tl(r), f.c(), f.m(t, null)) : f && (f.d(1), f = null), a[0] & /*last_progress_level*/
+                32768 && i !== (i = `${/*last_progress_level*/
+      r[15] * 100}%`) && ce(o, "width", i);
         },
-        i: ft,
-        o: ft,
+        i: ht,
+        o: ht,
         d(r) {
-            r && y(e), a && a.d(), l[31](null);
+            r && M(e), f && f.d(), l[31](null);
         }
     };
 }
 
-function Ut(l) {
-    let e, t = Ke(
+function tl(l) {
+    let e, t = Re(
             /*progress*/
             l[7]
         ),
         n = [];
     for (let s = 0; s < t.length; s += 1)
-        n[s] = Wt(It(l, t, s));
+        n[s] = ol(Wt(l, t, s));
     return {
         c() {
             for (let s = 0; s < n.length; s += 1)
                 n[s].c();
-            e = Fe();
+            e = Ee();
         },
-        m(s, i) {
-            for (let f = 0; f < n.length; f += 1)
-                n[f] && n[f].m(s, i);
-            L(s, e, i);
+        m(s, o) {
+            for (let i = 0; i < n.length; i += 1)
+                n[i] && n[i].m(s, o);
+            V(s, e, o);
         },
-        p(s, i) {
-            if (i[0] & /*progress_level, progress*/
+        p(s, o) {
+            if (o[0] & /*progress_level, progress*/
                 16512) {
-                t = Ke(
+                t = Re(
                     /*progress*/
                     s[7]
                 );
-                let f;
-                for (f = 0; f < t.length; f += 1) {
-                    const a = It(s, t, f);
-                    n[f] ? n[f].p(a, i) : (n[f] = Wt(a), n[f].c(), n[f].m(e.parentNode, e));
+                let i;
+                for (i = 0; i < t.length; i += 1) {
+                    const f = Wt(s, t, i);
+                    n[i] ? n[i].p(f, o) : (n[i] = ol(f), n[i].c(), n[i].m(e.parentNode, e));
                 }
-                for (; f < n.length; f += 1)
-                    n[f].d(1);
+                for (; i < n.length; i += 1)
+                    n[i].d(1);
                 n.length = t.length;
             }
         },
         d(s) {
-            s && y(e), dl(n, s);
+            s && M(e), Ll(n, s);
         }
     };
 }
 
-function Xt(l) {
-    let e, t, n, s, i = (
+function ll(l) {
+    let e, t, n, s, o = (
             /*i*/
-            l[43] !== 0 && Pi()
+            l[43] !== 0 && Qi()
         ),
-        f = (
+        i = (
             /*p*/
-            l[41].desc != null && Gt(l)
+            l[41].desc != null && nl(l)
         ),
-        a = (
+        f = (
             /*p*/
             l[41].desc != null && /*progress_level*/
             l[14] && /*progress_level*/
             l[14][
                 /*i*/
                 l[43]
-            ] != null && Ot()
+            ] != null && il()
         ),
         r = (
             /*progress_level*/
-            l[14] != null && Rt(l)
+            l[14] != null && sl(l)
         );
     return {
         c() {
-            i && i.c(), e = G(), f && f.c(), t = G(), a && a.c(), n = G(), r && r.c(), s = Fe();
+            o && o.c(), e = X(), i && i.c(), t = X(), f && f.c(), n = X(), r && r.c(), s = Ee();
         },
-        m(o, u) {
-            i && i.m(o, u), L(o, e, u), f && f.m(o, u), L(o, t, u), a && a.m(o, u), L(o, n, u), r && r.m(o, u), L(o, s, u);
+        m(a, u) {
+            o && o.m(a, u), V(a, e, u), i && i.m(a, u), V(a, t, u), f && f.m(a, u), V(a, n, u), r && r.m(a, u), V(a, s, u);
         },
-        p(o, u) {
+        p(a, u) {
             /*p*/
-            o[41].desc != null ? f ? f.p(o, u) : (f = Gt(o), f.c(), f.m(t.parentNode, t)) : f && (f.d(1), f = null), /*p*/
-                o[41].desc != null && /*progress_level*/
-                o[14] && /*progress_level*/
-                o[14][
+            a[41].desc != null ? i ? i.p(a, u) : (i = nl(a), i.c(), i.m(t.parentNode, t)) : i && (i.d(1), i = null), /*p*/
+                a[41].desc != null && /*progress_level*/
+                a[14] && /*progress_level*/
+                a[14][
                     /*i*/
-                    o[43]
-                ] != null ? a || (a = Ot(), a.c(), a.m(n.parentNode, n)) : a && (a.d(1), a = null), /*progress_level*/
-                o[14] != null ? r ? r.p(o, u) : (r = Rt(o), r.c(), r.m(s.parentNode, s)) : r && (r.d(1), r = null);
+                    a[43]
+                ] != null ? f || (f = il(), f.c(), f.m(n.parentNode, n)) : f && (f.d(1), f = null), /*progress_level*/
+                a[14] != null ? r ? r.p(a, u) : (r = sl(a), r.c(), r.m(s.parentNode, s)) : r && (r.d(1), r = null);
         },
-        d(o) {
-            o && (y(e), y(t), y(n), y(s)), i && i.d(o), f && f.d(o), a && a.d(o), r && r.d(o);
+        d(a) {
+            a && (M(e), M(t), M(n), M(s)), o && o.d(a), i && i.d(a), f && f.d(a), r && r.d(a);
         }
     };
 }
 
-function Pi(l) {
+function Qi(l) {
     let e;
     return {
         c() {
             e = z(" /");
         },
         m(t, n) {
-            L(t, e, n);
+            V(t, e, n);
         },
         d(t) {
-            t && y(e);
+            t && M(e);
         }
     };
 }
 
-function Gt(l) {
+function nl(l) {
     let e = (
             /*p*/
             l[41].desc + ""
         ),
         t;
     return {
         c() {
             t = z(e);
         },
         m(n, s) {
-            L(n, t, s);
+            V(n, t, s);
         },
         p(n, s) {
             s[0] & /*progress*/
                 128 && e !== (e = /*p*/
-                    n[41].desc + "") && O(t, e);
+                    n[41].desc + "") && G(t, e);
         },
         d(n) {
-            n && y(t);
+            n && M(t);
         }
     };
 }
 
-function Ot(l) {
+function il(l) {
     let e;
     return {
         c() {
             e = z("-");
         },
         m(t, n) {
-            L(t, e, n);
+            V(t, e, n);
         },
         d(t) {
-            t && y(e);
+            t && M(e);
         }
     };
 }
 
-function Rt(l) {
+function sl(l) {
     let e = (100 * /*progress_level*/
             (l[14][
                 /*i*/
                 l[43]
             ] || 0)).toFixed(1) + "",
         t, n;
     return {
         c() {
             t = z(e), n = z("%");
         },
-        m(s, i) {
-            L(s, t, i), L(s, n, i);
+        m(s, o) {
+            V(s, t, o), V(s, n, o);
         },
-        p(s, i) {
-            i[0] & /*progress_level*/
+        p(s, o) {
+            o[0] & /*progress_level*/
                 16384 && e !== (e = (100 * /*progress_level*/
                     (s[14][
                         /*i*/
                         s[43]
-                    ] || 0)).toFixed(1) + "") && O(t, e);
+                    ] || 0)).toFixed(1) + "") && G(t, e);
         },
         d(s) {
-            s && (y(t), y(n));
+            s && (M(t), M(n));
         }
     };
 }
 
-function Wt(l) {
+function ol(l) {
     let e, t = (
         /*p*/
         (l[41].desc != null || /*progress_level*/
             l[14] && /*progress_level*/
             l[14][
                 /*i*/
                 l[43]
-            ] != null) && Xt(l)
+            ] != null) && ll(l)
     );
     return {
         c() {
-            t && t.c(), e = Fe();
+            t && t.c(), e = Ee();
         },
         m(n, s) {
-            t && t.m(n, s), L(n, e, s);
+            t && t.m(n, s), V(n, e, s);
         },
         p(n, s) {
             /*p*/
             n[41].desc != null || /*progress_level*/
                 n[14] && /*progress_level*/
                 n[14][
                     /*i*/
                     n[43]
-                ] != null ? t ? t.p(n, s) : (t = Xt(n), t.c(), t.m(e.parentNode, e)) : t && (t.d(1), t = null);
+                ] != null ? t ? t.p(n, s) : (t = ll(n), t.c(), t.m(e.parentNode, e)) : t && (t.d(1), t = null);
         },
         d(n) {
-            n && y(e), t && t.d(n);
+            n && M(e), t && t.d(n);
         }
     };
 }
 
-function Jt(l) {
+function fl(l) {
     let e, t, n, s;
-    const i = (
+    const o = (
             /*#slots*/
             l[30]["additional-loading-text"]
         ),
-        f = _l(
-            i,
+        i = Cl(
+            o,
             l,
             /*$$scope*/
             l[29],
-            Dt
+            Rt
         );
     return {
         c() {
-            e = ae("p"), t = z(
+            e = oe("p"), t = z(
                 /*loading_text*/
                 l[9]
-            ), n = G(), f && f.c(), te(e, "class", "loading svelte-vopvsi");
+            ), n = X(), i && i.c(), x(e, "class", "loading svelte-vopvsi");
         },
-        m(a, r) {
-            L(a, e, r), ge(e, t), L(a, n, r), f && f.m(a, r), s = !0;
+        m(f, r) {
+            V(f, e, r), be(e, t), V(f, n, r), i && i.m(f, r), s = !0;
         },
-        p(a, r) {
+        p(f, r) {
             (!s || r[0] & /*loading_text*/
-                512) && O(
+                512) && G(
                 t,
                 /*loading_text*/
-                a[9]
-            ), f && f.p && (!s || r[0] & /*$$scope*/
-                536870912) && gl(
-                f,
+                f[9]
+            ), i && i.p && (!s || r[0] & /*$$scope*/
+                536870912) && ql(
                 i,
-                a,
+                o,
+                f,
                 /*$$scope*/
-                a[29],
-                s ? hl(
-                    i,
+                f[29],
+                s ? Vl(
+                    o,
                     /*$$scope*/
-                    a[29],
+                    f[29],
                     r,
-                    Si
-                ) : ml(
+                    Pi
+                ) : Ml(
                     /*$$scope*/
-                    a[29]
+                    f[29]
                 ),
-                Dt
+                Rt
             );
         },
-        i(a) {
-            s || (ee(f, a), s = !0);
+        i(f) {
+            s || (Q(i, f), s = !0);
         },
-        o(a) {
-            re(f, a), s = !1;
+        o(f) {
+            fe(i, f), s = !1;
         },
-        d(a) {
-            a && (y(e), y(n)), f && f.d(a);
+        d(f) {
+            f && (M(e), M(n)), i && i.d(f);
         }
     };
 }
 
-function Yi(l) {
-    let e, t, n, s, i;
-    const f = [Ei, zi],
-        a = [];
+function xi(l) {
+    let e, t, n, s, o;
+    const i = [Ki, Yi],
+        f = [];
 
-    function r(o, u) {
+    function r(a, u) {
         return (
             /*status*/
-            o[4] === "pending" ? 0 : (
+            a[4] === "pending" ? 0 : (
                 /*status*/
-                o[4] === "error" ? 1 : -1
+                a[4] === "error" ? 1 : -1
             )
         );
     }
-    return ~(t = r(l)) && (n = a[t] = f[t](l)), {
+    return ~(t = r(l)) && (n = f[t] = i[t](l)), {
         c() {
-            e = ae("div"), n && n.c(), te(e, "class", s = "wrap " + /*variant*/
+            e = oe("div"), n && n.c(), x(e, "class", s = "wrap " + /*variant*/
                 l[8] + " " + /*show_progress*/
-                l[6] + " svelte-vopvsi"), X(e, "hide", ! /*status*/
+                l[6] + " svelte-vopvsi"), U(e, "hide", ! /*status*/
                 l[4] || /*status*/
                 l[4] === "complete" || /*show_progress*/
-                l[6] === "hidden"), X(
+                l[6] === "hidden"), U(
                 e,
                 "translucent",
                 /*variant*/
                 l[8] === "center" && /*status*/
                 (l[4] === "pending" || /*status*/
                     l[4] === "error") || /*translucent*/
                 l[11] || /*show_progress*/
                 l[6] === "minimal"
-            ), X(
+            ), U(
                 e,
                 "generating",
                 /*status*/
                 l[4] === "generating"
-            ), X(
+            ), U(
                 e,
                 "border",
                 /*border*/
                 l[12]
-            ), be(
+            ), ce(
                 e,
                 "position",
                 /*absolute*/
                 l[10] ? "absolute" : "static"
-            ), be(
+            ), ce(
                 e,
                 "padding",
                 /*absolute*/
                 l[10] ? "0" : "var(--size-8) 0"
             );
         },
-        m(o, u) {
-            L(o, e, u), ~t && a[t].m(e, null), l[33](e), i = !0;
+        m(a, u) {
+            V(a, e, u), ~t && f[t].m(e, null), l[33](e), o = !0;
         },
-        p(o, u) {
+        p(a, u) {
             let _ = t;
-            t = r(o), t === _ ? ~t && a[t].p(o, u) : (n && (st(), re(a[_], 1, 1, () => {
-                    a[_] = null;
-                }), it()), ~t ? (n = a[t], n ? n.p(o, u) : (n = a[t] = f[t](o), n.c()), ee(n, 1), n.m(e, null)) : n = null), (!i || u[0] & /*variant, show_progress*/
+            t = r(a), t === _ ? ~t && f[t].p(a, u) : (n && (mt(), fe(f[_], 1, 1, () => {
+                    f[_] = null;
+                }), dt()), ~t ? (n = f[t], n ? n.p(a, u) : (n = f[t] = i[t](a), n.c()), Q(n, 1), n.m(e, null)) : n = null), (!o || u[0] & /*variant, show_progress*/
                     320 && s !== (s = "wrap " + /*variant*/
-                        o[8] + " " + /*show_progress*/
-                        o[6] + " svelte-vopvsi")) && te(e, "class", s), (!i || u[0] & /*variant, show_progress, status, show_progress*/
-                    336) && X(e, "hide", ! /*status*/
-                    o[4] || /*status*/
-                    o[4] === "complete" || /*show_progress*/
-                    o[6] === "hidden"), (!i || u[0] & /*variant, show_progress, variant, status, translucent, show_progress*/
-                    2384) && X(
+                        a[8] + " " + /*show_progress*/
+                        a[6] + " svelte-vopvsi")) && x(e, "class", s), (!o || u[0] & /*variant, show_progress, status, show_progress*/
+                    336) && U(e, "hide", ! /*status*/
+                    a[4] || /*status*/
+                    a[4] === "complete" || /*show_progress*/
+                    a[6] === "hidden"), (!o || u[0] & /*variant, show_progress, variant, status, translucent, show_progress*/
+                    2384) && U(
                     e,
                     "translucent",
                     /*variant*/
-                    o[8] === "center" && /*status*/
-                    (o[4] === "pending" || /*status*/
-                        o[4] === "error") || /*translucent*/
-                    o[11] || /*show_progress*/
-                    o[6] === "minimal"
-                ), (!i || u[0] & /*variant, show_progress, status*/
-                    336) && X(
+                    a[8] === "center" && /*status*/
+                    (a[4] === "pending" || /*status*/
+                        a[4] === "error") || /*translucent*/
+                    a[11] || /*show_progress*/
+                    a[6] === "minimal"
+                ), (!o || u[0] & /*variant, show_progress, status*/
+                    336) && U(
                     e,
                     "generating",
                     /*status*/
-                    o[4] === "generating"
-                ), (!i || u[0] & /*variant, show_progress, border*/
-                    4416) && X(
+                    a[4] === "generating"
+                ), (!o || u[0] & /*variant, show_progress, border*/
+                    4416) && U(
                     e,
                     "border",
                     /*border*/
-                    o[12]
+                    a[12]
                 ), u[0] & /*absolute*/
-                1024 && be(
+                1024 && ce(
                     e,
                     "position",
                     /*absolute*/
-                    o[10] ? "absolute" : "static"
+                    a[10] ? "absolute" : "static"
                 ), u[0] & /*absolute*/
-                1024 && be(
+                1024 && ce(
                     e,
                     "padding",
                     /*absolute*/
-                    o[10] ? "0" : "var(--size-8) 0"
+                    a[10] ? "0" : "var(--size-8) 0"
                 );
         },
-        i(o) {
-            i || (ee(n), i = !0);
+        i(a) {
+            o || (Q(n), o = !0);
         },
-        o(o) {
-            re(n), i = !1;
+        o(a) {
+            fe(n), o = !1;
         },
-        d(o) {
-            o && y(e), ~t && a[t].d(), l[33](null);
+        d(a) {
+            a && M(e), ~t && f[t].d(), l[33](null);
         }
     };
 }
-var Ki = function(l, e, t, n) {
-    function s(i) {
-        return i instanceof t ? i : new t(function(f) {
-            f(i);
+var $i = function(l, e, t, n) {
+    function s(o) {
+        return o instanceof t ? o : new t(function(i) {
+            i(o);
         });
     }
-    return new(t || (t = Promise))(function(i, f) {
-        function a(u) {
+    return new(t || (t = Promise))(function(o, i) {
+        function f(u) {
             try {
-                o(n.next(u));
+                a(n.next(u));
             } catch (_) {
-                f(_);
+                i(_);
             }
         }
 
         function r(u) {
             try {
-                o(n.throw(u));
+                a(n.throw(u));
             } catch (_) {
-                f(_);
+                i(_);
             }
         }
 
-        function o(u) {
-            u.done ? i(u.value) : s(u.value).then(a, r);
+        function a(u) {
+            u.done ? o(u.value) : s(u.value).then(f, r);
         }
-        o((n = n.apply(l, e || [])).next());
+        a((n = n.apply(l, e || [])).next());
     });
 };
-let Ne = [],
-    et = !1;
+let Ae = [],
+    rt = !1;
 
-function Ui(l) {
-    return Ki(this, arguments, void 0, function*(e, t = !0) {
+function es(l) {
+    return $i(this, arguments, void 0, function*(e, t = !0) {
         if (!(window.__gradio_mode__ === "website" || window.__gradio_mode__ !== "app" && t !== !0)) {
-            if (Ne.push(e), !et)
-                et = !0;
+            if (Ae.push(e), !rt)
+                rt = !0;
             else
                 return;
-            yield qi(), requestAnimationFrame(() => {
+            yield Di(), requestAnimationFrame(() => {
                 let n = [0, 0];
-                for (let s = 0; s < Ne.length; s++) {
-                    const f = Ne[s].getBoundingClientRect();
-                    (s === 0 || f.top + window.scrollY <= n[0]) && (n[0] = f.top + window.scrollY, n[1] = s);
+                for (let s = 0; s < Ae.length; s++) {
+                    const i = Ae[s].getBoundingClientRect();
+                    (s === 0 || i.top + window.scrollY <= n[0]) && (n[0] = i.top + window.scrollY, n[1] = s);
                 }
                 window.scrollTo({
                     top: n[0] - 20,
                     behavior: "smooth"
-                }), et = !1, Ne = [];
+                }), rt = !1, Ae = [];
             });
         }
     });
 }
 
-function Xi(l, e, t) {
+function ts(l, e, t) {
     let n, {
         $$slots: s = {},
-        $$scope: i
+        $$scope: o
     } = e;
     this && this.__awaiter;
-    const f = Zi();
+    const i = ji();
     let {
-        i18n: a
+        i18n: f
     } = e, {
         eta: r = null
     } = e, {
-        queue_position: o
+        queue_position: a
     } = e, {
         queue_size: u
     } = e, {
         status: _
     } = e, {
-        scroll_to_output: d = !1
+        scroll_to_output: c = !1
     } = e, {
         timer: h = !0
     } = e, {
-        show_progress: M = "full"
+        show_progress: L = "full"
     } = e, {
         message: H = null
     } = e, {
-        progress: k = null
+        progress: p = null
     } = e, {
-        variant: Z = "default"
+        variant: v = "default"
     } = e, {
-        loading_text: c = "Loading..."
+        loading_text: m = "Loading..."
     } = e, {
-        absolute: m = !0
+        absolute: b = !0
     } = e, {
-        translucent: p = !1
+        translucent: C = !1
     } = e, {
-        border: V = !1
+        border: T = !1
     } = e, {
-        autoscroll: w
-    } = e, E, j = !1, R = 0, D = 0, le = null, ne = null, we = 0, P = null, de, U = null, ve = !0;
-    const he = () => {
-        t(0, r = t(27, le = t(19, pe = null))), t(25, R = performance.now()), t(26, D = 0), j = !0, ke();
+        autoscroll: k
+    } = e, N, I = !1, ae = 0, j = 0, le = null, ne = null, ge = 0, Y = null, re, O = null, we = !0;
+    const _e = () => {
+        t(0, r = t(27, le = t(19, ke = null))), t(25, ae = performance.now()), t(26, j = 0), I = !0, ve();
     };
 
-    function ke() {
+    function ve() {
         requestAnimationFrame(() => {
-            t(26, D = (performance.now() - R) / 1e3), j && ke();
+            t(26, j = (performance.now() - ae) / 1e3), I && ve();
         });
     }
 
-    function g() {
-        t(26, D = 0), t(0, r = t(27, le = t(19, pe = null))), j && (j = !1);
+    function w() {
+        t(26, j = 0), t(0, r = t(27, le = t(19, ke = null))), I && (I = !1);
     }
-    Hi(() => {
-        j && g();
+    Ii(() => {
+        I && w();
     });
-    let pe = null;
+    let ke = null;
 
-    function Ue(v) {
-        Bt[v ? "unshift" : "push"](() => {
-            U = v, t(16, U), t(7, k), t(14, P), t(15, de);
+    function We(y) {
+        Xt[y ? "unshift" : "push"](() => {
+            O = y, t(16, O), t(7, p), t(14, Y), t(15, re);
         });
     }
-    const Xe = () => {
-        f("clear_status");
+    const Je = () => {
+        i("clear_status");
     };
 
-    function Ge(v) {
-        Bt[v ? "unshift" : "push"](() => {
-            E = v, t(13, E);
+    function Qe(y) {
+        Xt[y ? "unshift" : "push"](() => {
+            N = y, t(13, N);
         });
     }
-    return l.$$set = (v) => {
-        "i18n" in v && t(1, a = v.i18n), "eta" in v && t(0, r = v.eta), "queue_position" in v && t(2, o = v.queue_position), "queue_size" in v && t(3, u = v.queue_size), "status" in v && t(4, _ = v.status), "scroll_to_output" in v && t(22, d = v.scroll_to_output), "timer" in v && t(5, h = v.timer), "show_progress" in v && t(6, M = v.show_progress), "message" in v && t(23, H = v.message), "progress" in v && t(7, k = v.progress), "variant" in v && t(8, Z = v.variant), "loading_text" in v && t(9, c = v.loading_text), "absolute" in v && t(10, m = v.absolute), "translucent" in v && t(11, p = v.translucent), "border" in v && t(12, V = v.border), "autoscroll" in v && t(24, w = v.autoscroll), "$$scope" in v && t(29, i = v.$$scope);
+    return l.$$set = (y) => {
+        "i18n" in y && t(1, f = y.i18n), "eta" in y && t(0, r = y.eta), "queue_position" in y && t(2, a = y.queue_position), "queue_size" in y && t(3, u = y.queue_size), "status" in y && t(4, _ = y.status), "scroll_to_output" in y && t(22, c = y.scroll_to_output), "timer" in y && t(5, h = y.timer), "show_progress" in y && t(6, L = y.show_progress), "message" in y && t(23, H = y.message), "progress" in y && t(7, p = y.progress), "variant" in y && t(8, v = y.variant), "loading_text" in y && t(9, m = y.loading_text), "absolute" in y && t(10, b = y.absolute), "translucent" in y && t(11, C = y.translucent), "border" in y && t(12, T = y.border), "autoscroll" in y && t(24, k = y.autoscroll), "$$scope" in y && t(29, o = y.$$scope);
     }, l.$$.update = () => {
         l.$$.dirty[0] & /*eta, old_eta, timer_start, eta_from_start*/
-            436207617 && (r === null && t(0, r = le), r != null && le !== r && (t(28, ne = (performance.now() - R) / 1e3 + r), t(19, pe = ne.toFixed(1)), t(27, le = r))), l.$$.dirty[0] & /*eta_from_start, timer_diff*/
-            335544320 && t(17, we = ne === null || ne <= 0 || !D ? null : Math.min(D / ne, 1)), l.$$.dirty[0] & /*progress*/
-            128 && k != null && t(18, ve = !1), l.$$.dirty[0] & /*progress, progress_level, progress_bar, last_progress_level*/
-            114816 && (k != null ? t(14, P = k.map((v) => {
-                if (v.index != null && v.length != null)
-                    return v.index / v.length;
-                if (v.progress != null)
-                    return v.progress;
-            })) : t(14, P = null), P ? (t(15, de = P[P.length - 1]), U && (de === 0 ? t(16, U.style.transition = "0", U) : t(16, U.style.transition = "150ms", U))) : t(15, de = void 0)), l.$$.dirty[0] & /*status*/
-            16 && (_ === "pending" ? he() : g()), l.$$.dirty[0] & /*el, scroll_to_output, status, autoscroll*/
-            20979728 && E && d && (_ === "pending" || _ === "complete") && Ui(E, w), l.$$.dirty[0] & /*status, message*/
+            436207617 && (r === null && t(0, r = le), r != null && le !== r && (t(28, ne = (performance.now() - ae) / 1e3 + r), t(19, ke = ne.toFixed(1)), t(27, le = r))), l.$$.dirty[0] & /*eta_from_start, timer_diff*/
+            335544320 && t(17, ge = ne === null || ne <= 0 || !j ? null : Math.min(j / ne, 1)), l.$$.dirty[0] & /*progress*/
+            128 && p != null && t(18, we = !1), l.$$.dirty[0] & /*progress, progress_level, progress_bar, last_progress_level*/
+            114816 && (p != null ? t(14, Y = p.map((y) => {
+                if (y.index != null && y.length != null)
+                    return y.index / y.length;
+                if (y.progress != null)
+                    return y.progress;
+            })) : t(14, Y = null), Y ? (t(15, re = Y[Y.length - 1]), O && (re === 0 ? t(16, O.style.transition = "0", O) : t(16, O.style.transition = "150ms", O))) : t(15, re = void 0)), l.$$.dirty[0] & /*status*/
+            16 && (_ === "pending" ? _e() : w()), l.$$.dirty[0] & /*el, scroll_to_output, status, autoscroll*/
+            20979728 && N && c && (_ === "pending" || _ === "complete") && es(N, k), l.$$.dirty[0] & /*status, message*/
             8388624, l.$$.dirty[0] & /*timer_diff*/
-            67108864 && t(20, n = D.toFixed(1));
+            67108864 && t(20, n = j.toFixed(1));
     }, [
         r,
+        f,
         a,
-        o,
         u,
         _,
         h,
-        M,
-        k,
-        Z,
-        c,
-        m,
+        L,
         p,
-        V,
-        E,
-        P,
-        de,
-        U,
+        v,
+        m,
+        b,
+        C,
+        T,
+        N,
+        Y,
+        re,
+        O,
+        ge,
         we,
-        ve,
-        pe,
+        ke,
         n,
-        f,
-        d,
+        i,
+        c,
         H,
-        w,
-        R,
-        D,
+        k,
+        ae,
+        j,
         le,
         ne,
-        i,
+        o,
         s,
-        Ue,
-        Xe,
-        Ge
+        We,
+        Je,
+        Qe
     ];
 }
-class Gi extends Li {
+class ls extends Ti {
     constructor(e) {
-        super(), Mi(
+        super(), Bi(
             this,
             e,
-            Xi,
-            Yi,
-            Vi, {
+            ts,
+            xi,
+            Ni, {
                 i18n: 1,
                 eta: 0,
                 queue_position: 2,
                 queue_size: 3,
                 status: 4,
                 scroll_to_output: 22,
                 timer: 5,
@@ -3435,167 +3710,167 @@
             },
             null,
             [-1, -1]
         );
     }
 }
 const {
-    SvelteComponent: Oi,
-    add_iframe_resize_listener: Ri,
-    add_render_callback: Wi,
-    append: Ji,
-    attr: Qi,
-    binding_callbacks: xi,
-    detach: $i,
-    element: es,
-    init: ts,
-    insert: ls,
-    noop: Qt,
-    safe_not_equal: ns,
-    set_data: is,
-    text: ss,
-    toggle_class: Ve
+    SvelteComponent: ns,
+    add_iframe_resize_listener: is,
+    add_render_callback: ss,
+    append: os,
+    attr: fs,
+    binding_callbacks: as,
+    detach: rs,
+    element: us,
+    init: _s,
+    insert: cs,
+    noop: al,
+    safe_not_equal: ds,
+    set_data: ms,
+    text: hs,
+    toggle_class: qe
 } = window.__gradio__svelte__internal, {
-    onMount: fs
+    onMount: bs
 } = window.__gradio__svelte__internal;
 
-function os(l) {
+function gs(l) {
     let e, t = (
             /*value*/
             (l[0] ? (
                 /*value*/
                 l[0]
             ) : "") + ""
         ),
         n, s;
     return {
         c() {
-            e = es("div"), n = ss(t), Qi(e, "class", "svelte-84cxb8"), Wi(() => (
+            e = us("div"), n = hs(t), fs(e, "class", "svelte-84cxb8"), ss(() => (
                 /*div_elementresize_handler*/
                 l[5].call(e)
-            )), Ve(
+            )), qe(
                 e,
                 "table",
                 /*type*/
                 l[1] === "table"
-            ), Ve(
+            ), qe(
                 e,
                 "gallery",
                 /*type*/
                 l[1] === "gallery"
-            ), Ve(
+            ), qe(
                 e,
                 "selected",
                 /*selected*/
                 l[2]
             );
         },
-        m(i, f) {
-            ls(i, e, f), Ji(e, n), s = Ri(
+        m(o, i) {
+            cs(o, e, i), os(e, n), s = is(
                 e,
                 /*div_elementresize_handler*/
                 l[5].bind(e)
             ), l[6](e);
         },
-        p(i, [f]) {
-            f & /*value*/
+        p(o, [i]) {
+            i & /*value*/
                 1 && t !== (t = /*value*/
-                    (i[0] ? (
+                    (o[0] ? (
                         /*value*/
-                        i[0]
-                    ) : "") + "") && is(n, t), f & /*type*/
-                2 && Ve(
+                        o[0]
+                    ) : "") + "") && ms(n, t), i & /*type*/
+                2 && qe(
                     e,
                     "table",
                     /*type*/
-                    i[1] === "table"
-                ), f & /*type*/
-                2 && Ve(
+                    o[1] === "table"
+                ), i & /*type*/
+                2 && qe(
                     e,
                     "gallery",
                     /*type*/
-                    i[1] === "gallery"
-                ), f & /*selected*/
-                4 && Ve(
+                    o[1] === "gallery"
+                ), i & /*selected*/
+                4 && qe(
                     e,
                     "selected",
                     /*selected*/
-                    i[2]
+                    o[2]
                 );
         },
-        i: Qt,
-        o: Qt,
-        d(i) {
-            i && $i(e), s(), l[6](null);
+        i: al,
+        o: al,
+        d(o) {
+            o && rs(e), s(), l[6](null);
         }
     };
 }
 
-function as(l, e, t) {
+function ws(l, e, t) {
     let {
         value: n
     } = e, {
         type: s
     } = e, {
-        selected: i = !1
-    } = e, f, a;
+        selected: o = !1
+    } = e, i, f;
 
-    function r(_, d) {
-        !_ || !d || (a.style.setProperty("--local-text-width", `${d < 150 ? d : 200}px`), t(4, a.style.whiteSpace = "unset", a));
+    function r(_, c) {
+        !_ || !c || (f.style.setProperty("--local-text-width", `${c < 150 ? c : 200}px`), t(4, f.style.whiteSpace = "unset", f));
     }
-    fs(() => {
-        r(a, f);
+    bs(() => {
+        r(f, i);
     });
 
-    function o() {
-        f = this.clientWidth, t(3, f);
+    function a() {
+        i = this.clientWidth, t(3, i);
     }
 
     function u(_) {
-        xi[_ ? "unshift" : "push"](() => {
-            a = _, t(4, a);
+        as[_ ? "unshift" : "push"](() => {
+            f = _, t(4, f);
         });
     }
     return l.$$set = (_) => {
-        "value" in _ && t(0, n = _.value), "type" in _ && t(1, s = _.type), "selected" in _ && t(2, i = _.selected);
-    }, [n, s, i, f, a, o, u];
+        "value" in _ && t(0, n = _.value), "type" in _ && t(1, s = _.type), "selected" in _ && t(2, o = _.selected);
+    }, [n, s, o, i, f, a, u];
 }
-class ys extends Oi {
+class Es extends ns {
     constructor(e) {
-        super(), ts(this, e, as, os, ns, {
+        super(), _s(this, e, ws, gs, ds, {
             value: 0,
             type: 1,
             selected: 2
         });
     }
 }
 const {
-    SvelteComponent: rs,
-    add_flush_callback: xt,
-    assign: us,
-    bind: $t,
-    binding_callbacks: el,
-    check_outros: _s,
-    create_component: rt,
-    destroy_component: ut,
-    detach: cs,
-    flush: F,
-    get_spread_object: ds,
-    get_spread_update: ms,
-    group_outros: hs,
-    init: bs,
-    insert: gs,
-    mount_component: _t,
-    safe_not_equal: ws,
-    space: vs,
-    transition_in: He,
-    transition_out: Ee
+    SvelteComponent: vs,
+    add_flush_callback: rl,
+    assign: ks,
+    bind: ul,
+    binding_callbacks: _l,
+    check_outros: ps,
+    create_component: Ct,
+    destroy_component: yt,
+    detach: Cs,
+    flush: Z,
+    get_spread_object: ys,
+    get_spread_update: Ls,
+    group_outros: Ms,
+    init: Vs,
+    insert: Hs,
+    mount_component: Lt,
+    safe_not_equal: qs,
+    space: Fs,
+    transition_in: Ze,
+    transition_out: Ne
 } = window.__gradio__svelte__internal;
 
-function tl(l) {
+function cl(l) {
     let e, t;
     const n = [{
             autoscroll: (
                 /*gradio*/
                 l[2].autoscroll
             )
         }, {
@@ -3604,80 +3879,80 @@
                 l[2].i18n
             )
         },
         /*loading_status*/
         l[18]
     ];
     let s = {};
-    for (let i = 0; i < n.length; i += 1)
-        s = us(s, n[i]);
-    return e = new Gi({
+    for (let o = 0; o < n.length; o += 1)
+        s = ks(s, n[o]);
+    return e = new ls({
         props: s
     }), e.$on(
         "clear_status",
         /*clear_status_handler*/
         l[24]
     ), {
         c() {
-            rt(e.$$.fragment);
+            Ct(e.$$.fragment);
         },
-        m(i, f) {
-            _t(e, i, f), t = !0;
+        m(o, i) {
+            Lt(e, o, i), t = !0;
         },
-        p(i, f) {
-            const a = f[0] & /*gradio, loading_status*/
-                262148 ? ms(n, [
-                    f[0] & /*gradio*/
+        p(o, i) {
+            const f = i[0] & /*gradio, loading_status*/
+                262148 ? Ls(n, [
+                    i[0] & /*gradio*/
                     4 && {
                         autoscroll: (
                             /*gradio*/
-                            i[2].autoscroll
+                            o[2].autoscroll
                         )
                     },
-                    f[0] & /*gradio*/
+                    i[0] & /*gradio*/
                     4 && {
                         i18n: (
                             /*gradio*/
-                            i[2].i18n
+                            o[2].i18n
                         )
                     },
-                    f[0] & /*loading_status*/
-                    262144 && ds(
+                    i[0] & /*loading_status*/
+                    262144 && ys(
                         /*loading_status*/
-                        i[18]
+                        o[18]
                     )
                 ]) : {};
-            e.$set(a);
+            e.$set(f);
         },
-        i(i) {
-            t || (He(e.$$.fragment, i), t = !0);
+        i(o) {
+            t || (Ze(e.$$.fragment, o), t = !0);
         },
-        o(i) {
-            Ee(e.$$.fragment, i), t = !1;
+        o(o) {
+            Ne(e.$$.fragment, o), t = !1;
         },
-        d(i) {
-            ut(e, i);
+        d(o) {
+            yt(e, o);
         }
     };
 }
 
-function ks(l) {
-    let e, t, n, s, i, f = (
+function Zs(l) {
+    let e, t, n, s, o, i = (
         /*loading_status*/
-        l[18] && tl(l)
+        l[18] && cl(l)
     );
 
-    function a(u) {
+    function f(u) {
         l[25](u);
     }
 
     function r(u) {
         l[26](u);
     }
-    let o = {
+    let a = {
         label: (
             /*label*/
             l[3]
         ),
         info: (
             /*info*/
             l[4]
@@ -3734,20 +4009,20 @@
             l[22]
         ),
         disabled: ! /*interactive*/
             l[23]
     };
     return (
         /*value*/
-        l[0] !== void 0 && (o.value = /*value*/
+        l[0] !== void 0 && (a.value = /*value*/
             l[0]), /*value_is_output*/
-        l[1] !== void 0 && (o.value_is_output = /*value_is_output*/
-            l[1]), t = new di({
-            props: o
-        }), el.push(() => $t(t, "value", a)), el.push(() => $t(t, "value_is_output", r)), t.$on(
+        l[1] !== void 0 && (a.value_is_output = /*value_is_output*/
+            l[1]), t = new yi({
+            props: a
+        }), _l.push(() => ul(t, "value", f)), _l.push(() => ul(t, "value_is_output", r)), t.$on(
             "change",
             /*change_handler*/
             l[27]
         ), t.$on(
             "input",
             /*input_handler*/
             l[28]
@@ -3765,84 +4040,84 @@
             l[31]
         ), t.$on(
             "focus",
             /*focus_handler*/
             l[32]
         ), {
             c() {
-                f && f.c(), e = vs(), rt(t.$$.fragment);
+                i && i.c(), e = Fs(), Ct(t.$$.fragment);
             },
             m(u, _) {
-                f && f.m(u, _), gs(u, e, _), _t(t, u, _), i = !0;
+                i && i.m(u, _), Hs(u, e, _), Lt(t, u, _), o = !0;
             },
             p(u, _) {
                 /*loading_status*/
-                u[18] ? f ? (f.p(u, _), _[0] & /*loading_status*/
-                    262144 && He(f, 1)) : (f = tl(u), f.c(), He(f, 1), f.m(e.parentNode, e)) : f && (hs(), Ee(f, 1, 1, () => {
-                    f = null;
-                }), _s());
-                const d = {};
+                u[18] ? i ? (i.p(u, _), _[0] & /*loading_status*/
+                    262144 && Ze(i, 1)) : (i = cl(u), i.c(), Ze(i, 1), i.m(e.parentNode, e)) : i && (Ms(), Ne(i, 1, 1, () => {
+                    i = null;
+                }), ps());
+                const c = {};
                 _[0] & /*label*/
-                    8 && (d.label = /*label*/
+                    8 && (c.label = /*label*/
                         u[3]), _[0] & /*info*/
-                    16 && (d.info = /*info*/
+                    16 && (c.info = /*info*/
                         u[4]), _[0] & /*show_label*/
-                    1024 && (d.show_label = /*show_label*/
+                    1024 && (c.show_label = /*show_label*/
                         u[10]), _[0] & /*lines*/
-                    256 && (d.lines = /*lines*/
+                    256 && (c.lines = /*lines*/
                         u[8]), _[0] & /*type*/
-                    16384 && (d.type = /*type*/
+                    16384 && (c.type = /*type*/
                         u[14]), _[0] & /*rtl*/
-                    524288 && (d.rtl = /*rtl*/
+                    524288 && (c.rtl = /*rtl*/
                         u[19]), _[0] & /*text_align*/
-                    1048576 && (d.text_align = /*text_align*/
+                    1048576 && (c.text_align = /*text_align*/
                         u[20]), _[0] & /*max_lines, lines*/
-                    2304 && (d.max_lines = /*max_lines*/
+                    2304 && (c.max_lines = /*max_lines*/
                         u[11] ? (
                             /*max_lines*/
                             u[11]
                         ) : (
                             /*lines*/
                             u[8] + 1
                         )), _[0] & /*prompts*/
-                    4096 && (d.prompts = /*prompts*/
+                    4096 && (c.prompts = /*prompts*/
                         u[12]), _[0] & /*suffixes*/
-                    8192 && (d.suffixes = /*suffixes*/
+                    8192 && (c.suffixes = /*suffixes*/
                         u[13]), _[0] & /*placeholder*/
-                    512 && (d.placeholder = /*placeholder*/
+                    512 && (c.placeholder = /*placeholder*/
                         u[9]), _[0] & /*autofocus*/
-                    2097152 && (d.autofocus = /*autofocus*/
+                    2097152 && (c.autofocus = /*autofocus*/
                         u[21]), _[0] & /*container*/
-                    32768 && (d.container = /*container*/
+                    32768 && (c.container = /*container*/
                         u[15]), _[0] & /*autoscroll*/
-                    4194304 && (d.autoscroll = /*autoscroll*/
+                    4194304 && (c.autoscroll = /*autoscroll*/
                         u[22]), _[0] & /*interactive*/
-                    8388608 && (d.disabled = ! /*interactive*/
+                    8388608 && (c.disabled = ! /*interactive*/
                         u[23]), !n && _[0] & /*value*/
-                    1 && (n = !0, d.value = /*value*/
-                        u[0], xt(() => n = !1)), !s && _[0] & /*value_is_output*/
-                    2 && (s = !0, d.value_is_output = /*value_is_output*/
-                        u[1], xt(() => s = !1)), t.$set(d);
+                    1 && (n = !0, c.value = /*value*/
+                        u[0], rl(() => n = !1)), !s && _[0] & /*value_is_output*/
+                    2 && (s = !0, c.value_is_output = /*value_is_output*/
+                        u[1], rl(() => s = !1)), t.$set(c);
             },
             i(u) {
-                i || (He(f), He(t.$$.fragment, u), i = !0);
+                o || (Ze(i), Ze(t.$$.fragment, u), o = !0);
             },
             o(u) {
-                Ee(f), Ee(t.$$.fragment, u), i = !1;
+                Ne(i), Ne(t.$$.fragment, u), o = !1;
             },
             d(u) {
-                u && cs(e), f && f.d(u), ut(t, u);
+                u && Cs(e), i && i.d(u), yt(t, u);
             }
         }
     );
 }
 
-function ps(l) {
+function Ss(l) {
     let e, t;
-    return e = new El({
+    return e = new Xl({
         props: {
             visible: (
                 /*visible*/
                 l[7]
             ),
             elem_id: (
                 /*elem_id*/
@@ -3862,171 +4137,171 @@
             ),
             allow_overflow: !1,
             padding: (
                 /*container*/
                 l[15]
             ),
             $$slots: {
-                default: [ks]
+                default: [Zs]
             },
             $$scope: {
                 ctx: l
             }
         }
     }), {
         c() {
-            rt(e.$$.fragment);
+            Ct(e.$$.fragment);
         },
         m(n, s) {
-            _t(e, n, s), t = !0;
+            Lt(e, n, s), t = !0;
         },
         p(n, s) {
-            const i = {};
+            const o = {};
             s[0] & /*visible*/
-                128 && (i.visible = /*visible*/
+                128 && (o.visible = /*visible*/
                     n[7]), s[0] & /*elem_id*/
-                32 && (i.elem_id = /*elem_id*/
+                32 && (o.elem_id = /*elem_id*/
                     n[5]), s[0] & /*elem_classes*/
-                64 && (i.elem_classes = /*elem_classes*/
+                64 && (o.elem_classes = /*elem_classes*/
                     n[6]), s[0] & /*scale*/
-                65536 && (i.scale = /*scale*/
+                65536 && (o.scale = /*scale*/
                     n[16]), s[0] & /*min_width*/
-                131072 && (i.min_width = /*min_width*/
+                131072 && (o.min_width = /*min_width*/
                     n[17]), s[0] & /*container*/
-                32768 && (i.padding = /*container*/
+                32768 && (o.padding = /*container*/
                     n[15]), s[0] & /*label, info, show_label, lines, type, rtl, text_align, max_lines, prompts, suffixes, placeholder, autofocus, container, autoscroll, interactive, value, value_is_output, gradio, loading_status*/
                 16580383 | s[1] & /*$$scope*/
-                4 && (i.$$scope = {
+                4 && (o.$$scope = {
                     dirty: s,
                     ctx: n
-                }), e.$set(i);
+                }), e.$set(o);
         },
         i(n) {
-            t || (He(e.$$.fragment, n), t = !0);
+            t || (Ze(e.$$.fragment, n), t = !0);
         },
         o(n) {
-            Ee(e.$$.fragment, n), t = !1;
+            Ne(e.$$.fragment, n), t = !1;
         },
         d(n) {
-            ut(e, n);
+            yt(e, n);
         }
     };
 }
 
-function Cs(l, e, t) {
+function zs(l, e, t) {
     let {
         gradio: n
     } = e, {
         label: s = "Textbox"
     } = e, {
-        info: i = void 0
+        info: o = void 0
     } = e, {
-        elem_id: f = ""
+        elem_id: i = ""
     } = e, {
-        elem_classes: a = []
+        elem_classes: f = []
     } = e, {
         visible: r = !0
     } = e, {
-        value: o = ""
+        value: a = ""
     } = e, {
         lines: u
     } = e, {
         placeholder: _ = ""
     } = e, {
-        show_label: d
+        show_label: c
     } = e, {
         max_lines: h
     } = e, {
-        prompts: M = []
+        prompts: L = []
     } = e, {
         suffixes: H = []
     } = e, {
-        type: k = "text"
+        type: p = "text"
     } = e, {
-        container: Z = !0
+        container: v = !0
     } = e, {
-        scale: c = null
+        scale: m = null
     } = e, {
-        min_width: m = void 0
+        min_width: b = void 0
     } = e, {
-        loading_status: p = void 0
+        loading_status: C = void 0
     } = e, {
-        value_is_output: V = !1
+        value_is_output: T = !1
     } = e, {
-        rtl: w = !1
+        rtl: k = !1
     } = e, {
-        text_align: E = void 0
+        text_align: N = void 0
     } = e, {
-        autofocus: j = !1
+        autofocus: I = !1
     } = e, {
-        autoscroll: R = !0
+        autoscroll: ae = !0
     } = e, {
-        interactive: D
+        interactive: j
     } = e;
-    const le = () => n.dispatch("clear_status", p);
+    const le = () => n.dispatch("clear_status", C);
 
-    function ne(g) {
-        o = g, t(0, o);
+    function ne(w) {
+        a = w, t(0, a);
     }
 
-    function we(g) {
-        V = g, t(1, V);
+    function ge(w) {
+        T = w, t(1, T);
     }
-    const P = () => n.dispatch("change", o),
-        de = () => n.dispatch("input"),
-        U = () => n.dispatch("submit"),
-        ve = () => n.dispatch("blur"),
-        he = (g) => n.dispatch("select", g.detail),
-        ke = () => n.dispatch("focus");
-    return l.$$set = (g) => {
-        "gradio" in g && t(2, n = g.gradio), "label" in g && t(3, s = g.label), "info" in g && t(4, i = g.info), "elem_id" in g && t(5, f = g.elem_id), "elem_classes" in g && t(6, a = g.elem_classes), "visible" in g && t(7, r = g.visible), "value" in g && t(0, o = g.value), "lines" in g && t(8, u = g.lines), "placeholder" in g && t(9, _ = g.placeholder), "show_label" in g && t(10, d = g.show_label), "max_lines" in g && t(11, h = g.max_lines), "prompts" in g && t(12, M = g.prompts), "suffixes" in g && t(13, H = g.suffixes), "type" in g && t(14, k = g.type), "container" in g && t(15, Z = g.container), "scale" in g && t(16, c = g.scale), "min_width" in g && t(17, m = g.min_width), "loading_status" in g && t(18, p = g.loading_status), "value_is_output" in g && t(1, V = g.value_is_output), "rtl" in g && t(19, w = g.rtl), "text_align" in g && t(20, E = g.text_align), "autofocus" in g && t(21, j = g.autofocus), "autoscroll" in g && t(22, R = g.autoscroll), "interactive" in g && t(23, D = g.interactive);
+    const Y = () => n.dispatch("change", a),
+        re = () => n.dispatch("input"),
+        O = () => n.dispatch("submit"),
+        we = () => n.dispatch("blur"),
+        _e = (w) => n.dispatch("select", w.detail),
+        ve = () => n.dispatch("focus");
+    return l.$$set = (w) => {
+        "gradio" in w && t(2, n = w.gradio), "label" in w && t(3, s = w.label), "info" in w && t(4, o = w.info), "elem_id" in w && t(5, i = w.elem_id), "elem_classes" in w && t(6, f = w.elem_classes), "visible" in w && t(7, r = w.visible), "value" in w && t(0, a = w.value), "lines" in w && t(8, u = w.lines), "placeholder" in w && t(9, _ = w.placeholder), "show_label" in w && t(10, c = w.show_label), "max_lines" in w && t(11, h = w.max_lines), "prompts" in w && t(12, L = w.prompts), "suffixes" in w && t(13, H = w.suffixes), "type" in w && t(14, p = w.type), "container" in w && t(15, v = w.container), "scale" in w && t(16, m = w.scale), "min_width" in w && t(17, b = w.min_width), "loading_status" in w && t(18, C = w.loading_status), "value_is_output" in w && t(1, T = w.value_is_output), "rtl" in w && t(19, k = w.rtl), "text_align" in w && t(20, N = w.text_align), "autofocus" in w && t(21, I = w.autofocus), "autoscroll" in w && t(22, ae = w.autoscroll), "interactive" in w && t(23, j = w.interactive);
     }, [
-        o,
-        V,
+        a,
+        T,
         n,
         s,
+        o,
         i,
         f,
-        a,
         r,
         u,
         _,
-        d,
+        c,
         h,
-        M,
+        L,
         H,
-        k,
-        Z,
-        c,
-        m,
         p,
-        w,
-        E,
+        v,
+        m,
+        b,
+        C,
+        k,
+        N,
+        I,
+        ae,
         j,
-        R,
-        D,
         le,
         ne,
+        ge,
+        Y,
+        re,
+        O,
         we,
-        P,
-        de,
-        U,
-        ve,
-        he,
-        ke
+        _e,
+        ve
     ];
 }
-class Ls extends rs {
+class Ts extends vs {
     constructor(e) {
-        super(), bs(
+        super(), Vs(
             this,
             e,
-            Cs,
-            ps,
-            ws, {
+            zs,
+            Ss,
+            qs, {
                 gradio: 2,
                 label: 3,
                 info: 4,
                 elem_id: 5,
                 elem_classes: 6,
                 visible: 7,
                 value: 0,
@@ -4054,200 +4329,200 @@
     }
     get gradio() {
         return this.$$.ctx[2];
     }
     set gradio(e) {
         this.$$set({
             gradio: e
-        }), F();
+        }), Z();
     }
     get label() {
         return this.$$.ctx[3];
     }
     set label(e) {
         this.$$set({
             label: e
-        }), F();
+        }), Z();
     }
     get info() {
         return this.$$.ctx[4];
     }
     set info(e) {
         this.$$set({
             info: e
-        }), F();
+        }), Z();
     }
     get elem_id() {
         return this.$$.ctx[5];
     }
     set elem_id(e) {
         this.$$set({
             elem_id: e
-        }), F();
+        }), Z();
     }
     get elem_classes() {
         return this.$$.ctx[6];
     }
     set elem_classes(e) {
         this.$$set({
             elem_classes: e
-        }), F();
+        }), Z();
     }
     get visible() {
         return this.$$.ctx[7];
     }
     set visible(e) {
         this.$$set({
             visible: e
-        }), F();
+        }), Z();
     }
     get value() {
         return this.$$.ctx[0];
     }
     set value(e) {
         this.$$set({
             value: e
-        }), F();
+        }), Z();
     }
     get lines() {
         return this.$$.ctx[8];
     }
     set lines(e) {
         this.$$set({
             lines: e
-        }), F();
+        }), Z();
     }
     get placeholder() {
         return this.$$.ctx[9];
     }
     set placeholder(e) {
         this.$$set({
             placeholder: e
-        }), F();
+        }), Z();
     }
     get show_label() {
         return this.$$.ctx[10];
     }
     set show_label(e) {
         this.$$set({
             show_label: e
-        }), F();
+        }), Z();
     }
     get max_lines() {
         return this.$$.ctx[11];
     }
     set max_lines(e) {
         this.$$set({
             max_lines: e
-        }), F();
+        }), Z();
     }
     get prompts() {
         return this.$$.ctx[12];
     }
     set prompts(e) {
         this.$$set({
             prompts: e
-        }), F();
+        }), Z();
     }
     get suffixes() {
         return this.$$.ctx[13];
     }
     set suffixes(e) {
         this.$$set({
             suffixes: e
-        }), F();
+        }), Z();
     }
     get type() {
         return this.$$.ctx[14];
     }
     set type(e) {
         this.$$set({
             type: e
-        }), F();
+        }), Z();
     }
     get container() {
         return this.$$.ctx[15];
     }
     set container(e) {
         this.$$set({
             container: e
-        }), F();
+        }), Z();
     }
     get scale() {
         return this.$$.ctx[16];
     }
     set scale(e) {
         this.$$set({
             scale: e
-        }), F();
+        }), Z();
     }
     get min_width() {
         return this.$$.ctx[17];
     }
     set min_width(e) {
         this.$$set({
             min_width: e
-        }), F();
+        }), Z();
     }
     get loading_status() {
         return this.$$.ctx[18];
     }
     set loading_status(e) {
         this.$$set({
             loading_status: e
-        }), F();
+        }), Z();
     }
     get value_is_output() {
         return this.$$.ctx[1];
     }
     set value_is_output(e) {
         this.$$set({
             value_is_output: e
-        }), F();
+        }), Z();
     }
     get rtl() {
         return this.$$.ctx[19];
     }
     set rtl(e) {
         this.$$set({
             rtl: e
-        }), F();
+        }), Z();
     }
     get text_align() {
         return this.$$.ctx[20];
     }
     set text_align(e) {
         this.$$set({
             text_align: e
-        }), F();
+        }), Z();
     }
     get autofocus() {
         return this.$$.ctx[21];
     }
     set autofocus(e) {
         this.$$set({
             autofocus: e
-        }), F();
+        }), Z();
     }
     get autoscroll() {
         return this.$$.ctx[22];
     }
     set autoscroll(e) {
         this.$$set({
             autoscroll: e
-        }), F();
+        }), Z();
     }
     get interactive() {
         return this.$$.ctx[23];
     }
     set interactive(e) {
         this.$$set({
             interactive: e
-        }), F();
+        }), Z();
     }
 }
 export {
-    ys as BaseExample,
-    di as BaseTextbox,
-    Ls as
+    Es as BaseExample,
+    yi as BaseTextbox,
+    Ts as
     default
 };
```

### Comparing `gradio_clickabletextbox-0.0.1/backend/gradio_clickabletextbox/templates/component/style.css` & `gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/templates/component/style.css`

 * *Files 6% similar despite different names*

```diff
@@ -1 +1 @@
-.block.svelte-nl1om8{position:relative;margin:0;box-shadow:var(--block-shadow);border-width:var(--block-border-width);border-color:var(--block-border-color);border-radius:var(--block-radius);background:var(--block-background-fill);width:100%;line-height:var(--line-sm)}.block.border_focus.svelte-nl1om8{border-color:var(--color-accent)}.block.border_contrast.svelte-nl1om8{border-color:var(--body-text-color)}.padded.svelte-nl1om8{padding:var(--block-padding)}.hidden.svelte-nl1om8{display:none}.hide-container.svelte-nl1om8{margin:0;box-shadow:none;--block-border-width:0;background:transparent;padding:0;overflow:visible}div.svelte-1hnfib2{margin-bottom:var(--spacing-lg);color:var(--block-info-text-color);font-weight:var(--block-info-text-weight);font-size:var(--block-info-text-size);line-height:var(--line-sm)}span.has-info.svelte-22c38v{margin-bottom:var(--spacing-xs)}span.svelte-22c38v:not(.has-info){margin-bottom:var(--spacing-lg)}span.svelte-22c38v{display:inline-block;position:relative;z-index:var(--layer-4);border:solid var(--block-title-border-width) var(--block-title-border-color);border-radius:var(--block-title-radius);background:var(--block-title-background-fill);padding:var(--block-title-padding);color:var(--block-title-text-color);font-weight:var(--block-title-text-weight);font-size:var(--block-title-text-size);line-height:var(--line-sm)}.hide.svelte-22c38v{margin:0;height:0}label.svelte-9gxdi0{display:inline-flex;align-items:center;z-index:var(--layer-2);box-shadow:var(--block-label-shadow);border:var(--block-label-border-width) solid var(--border-color-primary);border-top:none;border-left:none;border-radius:var(--block-label-radius);background:var(--block-label-background-fill);padding:var(--block-label-padding);pointer-events:none;color:var(--block-label-text-color);font-weight:var(--block-label-text-weight);font-size:var(--block-label-text-size);line-height:var(--line-sm)}.gr-group label.svelte-9gxdi0{border-top-left-radius:0}label.float.svelte-9gxdi0{position:absolute;top:var(--block-label-margin);left:var(--block-label-margin)}label.svelte-9gxdi0:not(.float){position:static;margin-top:var(--block-label-margin);margin-left:var(--block-label-margin)}.hide.svelte-9gxdi0{height:0}span.svelte-9gxdi0{opacity:.8;margin-right:var(--size-2);width:calc(var(--block-label-text-size) - 1px);height:calc(var(--block-label-text-size) - 1px)}.hide-label.svelte-9gxdi0{box-shadow:none;border-width:0;background:transparent;overflow:visible}button.svelte-1lrphxw{display:flex;justify-content:center;align-items:center;gap:1px;z-index:var(--layer-2);border-radius:var(--radius-sm);color:var(--block-label-text-color);border:1px solid transparent}button[disabled].svelte-1lrphxw{opacity:.5;box-shadow:none}button[disabled].svelte-1lrphxw:hover{cursor:not-allowed}.padded.svelte-1lrphxw{padding:2px;background:var(--bg-color);box-shadow:var(--shadow-drop);border:1px solid var(--button-secondary-border-color)}button.svelte-1lrphxw:hover,button.highlight.svelte-1lrphxw{cursor:pointer;color:var(--color-accent)}.padded.svelte-1lrphxw:hover{border:2px solid var(--button-secondary-border-color-hover);padding:1px;color:var(--block-label-text-color)}span.svelte-1lrphxw{padding:0 1px;font-size:10px}div.svelte-1lrphxw{padding:2px;display:flex;align-items:flex-end}.small.svelte-1lrphxw{width:14px;height:14px}.medium.svelte-1lrphxw{width:20px;height:20px}.large.svelte-1lrphxw{width:22px;height:22px}.pending.svelte-1lrphxw{animation:svelte-1lrphxw-flash .5s infinite}@keyframes svelte-1lrphxw-flash{0%{opacity:.5}50%{opacity:1}to{opacity:.5}}.transparent.svelte-1lrphxw{background:transparent;border:none;box-shadow:none}.empty.svelte-3w3rth{display:flex;justify-content:center;align-items:center;margin-top:calc(0px - var(--size-6));height:var(--size-full)}.icon.svelte-3w3rth{opacity:.5;height:var(--size-5);color:var(--body-text-color)}.small.svelte-3w3rth{min-height:calc(var(--size-32) - 20px)}.large.svelte-3w3rth{min-height:calc(var(--size-64) - 20px)}.unpadded_box.svelte-3w3rth{margin-top:0}.small_parent.svelte-3w3rth{min-height:100%!important}.dropdown-arrow.svelte-145leq6{fill:currentColor}.wrap.svelte-kzcjhc{display:flex;flex-direction:column;justify-content:center;align-items:center;min-height:var(--size-60);color:var(--block-label-text-color);line-height:var(--line-md);height:100%;padding-top:var(--size-3)}.or.svelte-kzcjhc{color:var(--body-text-color-subdued);display:flex}.icon-wrap.svelte-kzcjhc{width:30px;margin-bottom:var(--spacing-lg)}@media (--screen-md){.wrap.svelte-kzcjhc{font-size:var(--text-lg)}}.hovered.svelte-kzcjhc{color:var(--color-accent)}div.svelte-q32hvf{border-top:1px solid transparent;display:flex;max-height:100%;justify-content:center;align-items:center;gap:var(--spacing-sm);height:auto;align-items:flex-end;color:var(--block-label-text-color);flex-shrink:0}.show_border.svelte-q32hvf{border-top:1px solid var(--block-border-color);margin-top:var(--spacing-xxl);box-shadow:var(--shadow-drop)}.source-selection.svelte-1jp3vgd{display:flex;align-items:center;justify-content:center;border-top:1px solid var(--border-color-primary);width:95%;bottom:0;left:0;right:0;margin-left:auto;margin-right:auto}.icon.svelte-1jp3vgd{width:22px;height:22px;margin:var(--spacing-lg) var(--spacing-xs);padding:var(--spacing-xs);color:var(--neutral-400);border-radius:var(--radius-md)}.selected.svelte-1jp3vgd{color:var(--color-accent)}.icon.svelte-1jp3vgd:hover,.icon.svelte-1jp3vgd:focus{color:var(--color-accent)}label.svelte-n6pmag.svelte-n6pmag.svelte-n6pmag{display:block;width:100%}textarea.svelte-n6pmag.svelte-n6pmag.svelte-n6pmag{display:block;position:relative;outline:none!important;box-shadow:var(--input-shadow);background:var(--input-background-fill);padding:var(--input-padding);width:100%;color:var(--body-text-color);font-weight:var(--input-text-weight);font-size:var(--input-text-size);line-height:var(--line-sm);border:none}label.svelte-n6pmag.svelte-n6pmag.svelte-n6pmag:not(.container){height:100%}textarea.svelte-n6pmag.svelte-n6pmag.svelte-n6pmag:disabled{-webkit-text-fill-color:var(--body-text-color);-webkit-opacity:1;opacity:1}textarea.svelte-n6pmag.svelte-n6pmag.svelte-n6pmag:focus{box-shadow:var(--input-shadow-focus);border-color:var(--input-border-color-focus)}textarea.svelte-n6pmag.svelte-n6pmag.svelte-n6pmag::placeholder{color:var(--input-placeholder-color)}.extend_button.svelte-n6pmag.svelte-n6pmag.svelte-n6pmag{display:flex;position:absolute;top:45px;right:20px;align-items:center;background:var(--block-label-background-fill);width:20px;height:20px;overflow:hidden;color:var(--block-label-color);font:var(--font-sans);font-size:var(--button-small-text-size)}.extend_button.svelte-n6pmag:hover path.svelte-n6pmag.svelte-n6pmag{--ring-color:var(--color-accent);filter:brightness(1.1);transform:scale(1.05);fill:#ff6700}.menu_section.svelte-n6pmag.svelte-n6pmag.svelte-n6pmag{padding:12px 0 0;align-items:center;color:#100700;font-family:Inter;font-size:13px;font-style:normal;font-weight:300;line-height:24px;display:flex;flex-direction:column;align-items:flex-start;gap:8px}.menu.svelte-n6pmag ul.svelte-n6pmag.svelte-n6pmag{list-style-type:none;display:flex;align-items:flex-start;align-content:flex-start;gap:4px 12px;flex-wrap:wrap;flex-direction:column;width:100%}.menu.svelte-n6pmag.svelte-n6pmag.svelte-n6pmag{border-radius:0 0 15px 15px;background:#cccccc1a;margin:0 16px;padding:0 14px 12px}.menu.svelte-n6pmag li.svelte-n6pmag.svelte-n6pmag{width:100%}.text_extension_button.svelte-n6pmag.svelte-n6pmag.svelte-n6pmag{border-radius:15px;border:.5px solid #ff9a57;background:#fff4ea;cursor:pointer;display:flex;padding:4px 12px;align-items:center;gap:4px}.text_extension_button_prompt.svelte-n6pmag.svelte-n6pmag.svelte-n6pmag{display:flex;width:100%;padding:8px 12px;justify-content:space-between;align-items:center;border-radius:10px;border:.5px solid #ff9a57;background:#fff4ea;color:#101111;text-align:justify;font-size:13px;font-style:normal;font-weight:300;line-height:normal;gap:4px;flex-wrap:wrap;flex-direction:row}.text_extension_button_prompt.svelte-n6pmag.svelte-n6pmag.svelte-n6pmag:hover{color:#fff;fill:#fff;text-align:center;font-size:13px;font-style:normal;font-weight:300;border-radius:10px;border:.5px solid #ff9a57;background:var(--Light-Orange, #ff9a57)}.text_extension_button_prompt.svelte-n6pmag:hover svg.svelte-n6pmag path.svelte-n6pmag{fill:#fff}.text_extension_button.svelte-n6pmag.svelte-n6pmag.svelte-n6pmag:hover{color:#fff;text-align:center;font-size:13px;font-style:normal;font-weight:300;border-radius:10px;border:.5px solid #ff9a57;background:var(--Light-Orange, #ff9a57)}.text_extension_button.svelte-n6pmag:hover svg.svelte-n6pmag path.svelte-n6pmag{fill:#fff}svg.svelte-43sxxs.svelte-43sxxs{width:var(--size-20);height:var(--size-20)}svg.svelte-43sxxs path.svelte-43sxxs{fill:var(--loader-color)}div.svelte-43sxxs.svelte-43sxxs{z-index:var(--layer-2)}.margin.svelte-43sxxs.svelte-43sxxs{margin:var(--size-4)}.wrap.svelte-vopvsi.svelte-vopvsi{display:flex;flex-direction:column;justify-content:center;align-items:center;z-index:var(--layer-top);transition:opacity .1s ease-in-out;border-radius:var(--block-radius);background:var(--block-background-fill);padding:0 var(--size-6);max-height:var(--size-screen-h);overflow:hidden}.wrap.center.svelte-vopvsi.svelte-vopvsi{top:0;right:0;left:0}.wrap.default.svelte-vopvsi.svelte-vopvsi{top:0;right:0;bottom:0;left:0}.hide.svelte-vopvsi.svelte-vopvsi{opacity:0;pointer-events:none}.generating.svelte-vopvsi.svelte-vopvsi{animation:svelte-vopvsi-pulse 2s cubic-bezier(.4,0,.6,1) infinite;border:2px solid var(--color-accent);background:transparent;z-index:var(--layer-1);pointer-events:none}.translucent.svelte-vopvsi.svelte-vopvsi{background:none}@keyframes svelte-vopvsi-pulse{0%,to{opacity:1}50%{opacity:.5}}.loading.svelte-vopvsi.svelte-vopvsi{z-index:var(--layer-2);color:var(--body-text-color)}.eta-bar.svelte-vopvsi.svelte-vopvsi{position:absolute;top:0;right:0;bottom:0;left:0;transform-origin:left;opacity:.8;z-index:var(--layer-1);transition:10ms;background:var(--background-fill-secondary)}.progress-bar-wrap.svelte-vopvsi.svelte-vopvsi{border:1px solid var(--border-color-primary);background:var(--background-fill-primary);width:55.5%;height:var(--size-4)}.progress-bar.svelte-vopvsi.svelte-vopvsi{transform-origin:left;background-color:var(--loader-color);width:var(--size-full);height:var(--size-full)}.progress-level.svelte-vopvsi.svelte-vopvsi{display:flex;flex-direction:column;align-items:center;gap:1;z-index:var(--layer-2);width:var(--size-full)}.progress-level-inner.svelte-vopvsi.svelte-vopvsi{margin:var(--size-2) auto;color:var(--body-text-color);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text.svelte-vopvsi.svelte-vopvsi{position:absolute;top:0;right:0;z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text-center.svelte-vopvsi.svelte-vopvsi{display:flex;position:absolute;top:0;right:0;justify-content:center;align-items:center;transform:translateY(var(--size-6));z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono);text-align:center}.error.svelte-vopvsi.svelte-vopvsi{box-shadow:var(--shadow-drop);border:solid 1px var(--error-border-color);border-radius:var(--radius-full);background:var(--error-background-fill);padding-right:var(--size-4);padding-left:var(--size-4);color:var(--error-text-color);font-weight:var(--weight-semibold);font-size:var(--text-lg);line-height:var(--line-lg);font-family:var(--font)}.minimal.svelte-vopvsi .progress-text.svelte-vopvsi{background:var(--block-background-fill)}.border.svelte-vopvsi.svelte-vopvsi{border:1px solid var(--border-color-primary)}.clear-status.svelte-vopvsi.svelte-vopvsi{position:absolute;display:flex;top:var(--size-2);right:var(--size-2);justify-content:flex-end;gap:var(--spacing-sm);z-index:var(--layer-1)}.toast-body.svelte-solcu7{display:flex;position:relative;right:0;left:0;align-items:center;margin:var(--size-6) var(--size-4);margin:auto;border-radius:var(--container-radius);overflow:hidden;pointer-events:auto}.toast-body.error.svelte-solcu7{border:1px solid var(--color-red-700);background:var(--color-red-50)}.dark .toast-body.error.svelte-solcu7{border:1px solid var(--color-red-500);background-color:var(--color-grey-950)}.toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-700);background:var(--color-yellow-50)}.dark .toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-500);background-color:var(--color-grey-950)}.toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-700);background:var(--color-grey-50)}.dark .toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-500);background-color:var(--color-grey-950)}.toast-title.svelte-solcu7{display:flex;align-items:center;font-weight:var(--weight-bold);font-size:var(--text-lg);line-height:var(--line-sm);text-transform:capitalize}.toast-title.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-title.error.svelte-solcu7{color:var(--color-red-50)}.toast-title.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-title.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-title.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-title.info.svelte-solcu7{color:var(--color-grey-50)}.toast-close.svelte-solcu7{margin:0 var(--size-3);border-radius:var(--size-3);padding:0px var(--size-1-5);font-size:var(--size-5);line-height:var(--size-5)}.toast-close.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-close.error.svelte-solcu7{color:var(--color-red-500)}.toast-close.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-close.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-close.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-close.info.svelte-solcu7{color:var(--color-grey-500)}.toast-text.svelte-solcu7{font-size:var(--text-lg)}.toast-text.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-text.error.svelte-solcu7{color:var(--color-red-50)}.toast-text.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-text.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-text.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-text.info.svelte-solcu7{color:var(--color-grey-50)}.toast-details.svelte-solcu7{margin:var(--size-3) var(--size-3) var(--size-3) 0;width:100%}.toast-icon.svelte-solcu7{display:flex;position:absolute;position:relative;flex-shrink:0;justify-content:center;align-items:center;margin:var(--size-2);border-radius:var(--radius-full);padding:var(--size-1);padding-left:calc(var(--size-1) - 1px);width:35px;height:35px}.toast-icon.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-icon.error.svelte-solcu7{color:var(--color-red-500)}.toast-icon.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-icon.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-icon.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-icon.info.svelte-solcu7{color:var(--color-grey-500)}@keyframes svelte-solcu7-countdown{0%{transform:scaleX(1)}to{transform:scaleX(0)}}.timer.svelte-solcu7{position:absolute;bottom:0;left:0;transform-origin:0 0;animation:svelte-solcu7-countdown 10s linear forwards;width:100%;height:var(--size-1)}.timer.error.svelte-solcu7{background:var(--color-red-700)}.dark .timer.error.svelte-solcu7{background:var(--color-red-500)}.timer.warning.svelte-solcu7{background:var(--color-yellow-700)}.dark .timer.warning.svelte-solcu7{background:var(--color-yellow-500)}.timer.info.svelte-solcu7{background:var(--color-grey-700)}.dark .timer.info.svelte-solcu7{background:var(--color-grey-500)}.toast-wrap.svelte-gatr8h{display:flex;position:fixed;top:var(--size-4);right:var(--size-4);flex-direction:column;align-items:end;gap:var(--size-2);z-index:var(--layer-top);width:calc(100% - var(--size-8))}@media (--screen-sm){.toast-wrap.svelte-gatr8h{width:calc(var(--size-96) + var(--size-10))}}.gallery.svelte-84cxb8{padding:var(--size-1) var(--size-2)}div.svelte-84cxb8{overflow:hidden;min-width:var(--local-text-width);white-space:nowrap}
+.block.svelte-nl1om8{position:relative;margin:0;box-shadow:var(--block-shadow);border-width:var(--block-border-width);border-color:var(--block-border-color);border-radius:var(--block-radius);background:var(--block-background-fill);width:100%;line-height:var(--line-sm)}.block.border_focus.svelte-nl1om8{border-color:var(--color-accent)}.block.border_contrast.svelte-nl1om8{border-color:var(--body-text-color)}.padded.svelte-nl1om8{padding:var(--block-padding)}.hidden.svelte-nl1om8{display:none}.hide-container.svelte-nl1om8{margin:0;box-shadow:none;--block-border-width:0;background:transparent;padding:0;overflow:visible}div.svelte-1hnfib2{margin-bottom:var(--spacing-lg);color:var(--block-info-text-color);font-weight:var(--block-info-text-weight);font-size:var(--block-info-text-size);line-height:var(--line-sm)}span.has-info.svelte-22c38v{margin-bottom:var(--spacing-xs)}span.svelte-22c38v:not(.has-info){margin-bottom:var(--spacing-lg)}span.svelte-22c38v{display:inline-block;position:relative;z-index:var(--layer-4);border:solid var(--block-title-border-width) var(--block-title-border-color);border-radius:var(--block-title-radius);background:var(--block-title-background-fill);padding:var(--block-title-padding);color:var(--block-title-text-color);font-weight:var(--block-title-text-weight);font-size:var(--block-title-text-size);line-height:var(--line-sm)}.hide.svelte-22c38v{margin:0;height:0}label.svelte-9gxdi0{display:inline-flex;align-items:center;z-index:var(--layer-2);box-shadow:var(--block-label-shadow);border:var(--block-label-border-width) solid var(--border-color-primary);border-top:none;border-left:none;border-radius:var(--block-label-radius);background:var(--block-label-background-fill);padding:var(--block-label-padding);pointer-events:none;color:var(--block-label-text-color);font-weight:var(--block-label-text-weight);font-size:var(--block-label-text-size);line-height:var(--line-sm)}.gr-group label.svelte-9gxdi0{border-top-left-radius:0}label.float.svelte-9gxdi0{position:absolute;top:var(--block-label-margin);left:var(--block-label-margin)}label.svelte-9gxdi0:not(.float){position:static;margin-top:var(--block-label-margin);margin-left:var(--block-label-margin)}.hide.svelte-9gxdi0{height:0}span.svelte-9gxdi0{opacity:.8;margin-right:var(--size-2);width:calc(var(--block-label-text-size) - 1px);height:calc(var(--block-label-text-size) - 1px)}.hide-label.svelte-9gxdi0{box-shadow:none;border-width:0;background:transparent;overflow:visible}button.svelte-1lrphxw{display:flex;justify-content:center;align-items:center;gap:1px;z-index:var(--layer-2);border-radius:var(--radius-sm);color:var(--block-label-text-color);border:1px solid transparent}button[disabled].svelte-1lrphxw{opacity:.5;box-shadow:none}button[disabled].svelte-1lrphxw:hover{cursor:not-allowed}.padded.svelte-1lrphxw{padding:2px;background:var(--bg-color);box-shadow:var(--shadow-drop);border:1px solid var(--button-secondary-border-color)}button.svelte-1lrphxw:hover,button.highlight.svelte-1lrphxw{cursor:pointer;color:var(--color-accent)}.padded.svelte-1lrphxw:hover{border:2px solid var(--button-secondary-border-color-hover);padding:1px;color:var(--block-label-text-color)}span.svelte-1lrphxw{padding:0 1px;font-size:10px}div.svelte-1lrphxw{padding:2px;display:flex;align-items:flex-end}.small.svelte-1lrphxw{width:14px;height:14px}.medium.svelte-1lrphxw{width:20px;height:20px}.large.svelte-1lrphxw{width:22px;height:22px}.pending.svelte-1lrphxw{animation:svelte-1lrphxw-flash .5s infinite}@keyframes svelte-1lrphxw-flash{0%{opacity:.5}50%{opacity:1}to{opacity:.5}}.transparent.svelte-1lrphxw{background:transparent;border:none;box-shadow:none}.empty.svelte-3w3rth{display:flex;justify-content:center;align-items:center;margin-top:calc(0px - var(--size-6));height:var(--size-full)}.icon.svelte-3w3rth{opacity:.5;height:var(--size-5);color:var(--body-text-color)}.small.svelte-3w3rth{min-height:calc(var(--size-32) - 20px)}.large.svelte-3w3rth{min-height:calc(var(--size-64) - 20px)}.unpadded_box.svelte-3w3rth{margin-top:0}.small_parent.svelte-3w3rth{min-height:100%!important}.dropdown-arrow.svelte-145leq6{fill:currentColor}.wrap.svelte-kzcjhc{display:flex;flex-direction:column;justify-content:center;align-items:center;min-height:var(--size-60);color:var(--block-label-text-color);line-height:var(--line-md);height:100%;padding-top:var(--size-3)}.or.svelte-kzcjhc{color:var(--body-text-color-subdued);display:flex}.icon-wrap.svelte-kzcjhc{width:30px;margin-bottom:var(--spacing-lg)}@media (--screen-md){.wrap.svelte-kzcjhc{font-size:var(--text-lg)}}.hovered.svelte-kzcjhc{color:var(--color-accent)}div.svelte-q32hvf{border-top:1px solid transparent;display:flex;max-height:100%;justify-content:center;align-items:center;gap:var(--spacing-sm);height:auto;align-items:flex-end;color:var(--block-label-text-color);flex-shrink:0}.show_border.svelte-q32hvf{border-top:1px solid var(--block-border-color);margin-top:var(--spacing-xxl);box-shadow:var(--shadow-drop)}.source-selection.svelte-1jp3vgd{display:flex;align-items:center;justify-content:center;border-top:1px solid var(--border-color-primary);width:95%;bottom:0;left:0;right:0;margin-left:auto;margin-right:auto}.icon.svelte-1jp3vgd{width:22px;height:22px;margin:var(--spacing-lg) var(--spacing-xs);padding:var(--spacing-xs);color:var(--neutral-400);border-radius:var(--radius-md)}.selected.svelte-1jp3vgd{color:var(--color-accent)}.icon.svelte-1jp3vgd:hover,.icon.svelte-1jp3vgd:focus{color:var(--color-accent)}label.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs{display:block;width:100%}textarea.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs{display:block;position:relative;outline:none!important;box-shadow:var(--input-shadow);background:var(--input-background-fill);padding:var(--input-padding);width:100%;color:var(--body-text-color);font-weight:var(--input-text-weight);font-size:var(--input-text-size);line-height:var(--line-sm);border:none}label.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs:not(.container){height:100%}textarea.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs:disabled{-webkit-text-fill-color:var(--body-text-color);-webkit-opacity:1;opacity:1}textarea.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs::placeholder{color:var(--input-placeholder-color)}.extend_button.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs{display:flex;position:relative;align-items:center;width:20px;height:20px;overflow:hidden;color:var(--block-label-color);font:var(--font-sans);font-size:var(--button-small-text-size)}.extend_button.svelte-82ixrs:hover path.svelte-82ixrs.svelte-82ixrs{--ring-color:var(--color-accent);filter:brightness(1.1);fill:#ff6700}.menu_section.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs{padding:12px 0 0;align-items:center;color:#100700;font-family:Inter;font-size:13px;font-style:normal;font-weight:300;line-height:24px;display:flex;flex-direction:column;align-items:flex-start;gap:8px}.menu.svelte-82ixrs ul.svelte-82ixrs.svelte-82ixrs{list-style-type:none;display:flex;align-items:flex-start;align-content:flex-start;gap:4px 12px;flex-wrap:wrap;flex-direction:column;width:100%}.menu.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs{border-radius:0 0 15px 15px;background:#cccccc1a;margin:0 16px;padding:0 14px 12px}.menu.svelte-82ixrs li.svelte-82ixrs.svelte-82ixrs{width:100%}.text_extension_button.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs{border-radius:15px;border:.5px solid #ff9a57;background:#fff4ea;cursor:pointer;display:flex;padding:4px 12px;align-items:center;gap:4px}.text_extension_button_prompt.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs{display:flex;width:100%;padding:8px 12px;justify-content:space-between;align-items:center;border-radius:10px;border:.5px solid #ff9a57;background:#fff4ea;color:#101111;text-align:left;font-size:13px;font-style:normal;font-weight:300;line-height:normal;gap:4px;flex-wrap:wrap;flex-direction:row}.text_extension_button_prompt.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs:hover{color:#fff;fill:#fff;background:var(--Light-Orange, #ff9a57)}.text_extension_button_prompt.svelte-82ixrs:hover svg.svelte-82ixrs path.svelte-82ixrs{fill:#fff}.text_extension_button.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs:hover{color:#fff;background:var(--Light-Orange, #ff9a57)}.text_extension_button.svelte-82ixrs:hover svg.svelte-82ixrs path.svelte-82ixrs{fill:#fff}.magic_container.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs{display:flex;position:relative;outline:none!important;box-shadow:var(--input-shadow);padding:var(--input-padding);width:100%;color:var(--body-text-color);font-weight:var(--input-text-weight);font-size:var(--input-text-size);line-height:var(--line-sm);border:none;scrollbar-width:none;resize:none;align-items:center}.scroll_hide_magic.svelte-82ixrs.svelte-82ixrs.svelte-82ixrs{display:block;position:relative;outline:none!important;box-shadow:none;padding:var(--input-padding);width:100%;color:var(--body-text-color);font-weight:var(--input-text-weight);font-size:var(--input-text-size);line-height:var(--line-sm);border:none;scrollbar-width:none;resize:none}svg.svelte-43sxxs.svelte-43sxxs{width:var(--size-20);height:var(--size-20)}svg.svelte-43sxxs path.svelte-43sxxs{fill:var(--loader-color)}div.svelte-43sxxs.svelte-43sxxs{z-index:var(--layer-2)}.margin.svelte-43sxxs.svelte-43sxxs{margin:var(--size-4)}.wrap.svelte-vopvsi.svelte-vopvsi{display:flex;flex-direction:column;justify-content:center;align-items:center;z-index:var(--layer-top);transition:opacity .1s ease-in-out;border-radius:var(--block-radius);background:var(--block-background-fill);padding:0 var(--size-6);max-height:var(--size-screen-h);overflow:hidden}.wrap.center.svelte-vopvsi.svelte-vopvsi{top:0;right:0;left:0}.wrap.default.svelte-vopvsi.svelte-vopvsi{top:0;right:0;bottom:0;left:0}.hide.svelte-vopvsi.svelte-vopvsi{opacity:0;pointer-events:none}.generating.svelte-vopvsi.svelte-vopvsi{animation:svelte-vopvsi-pulse 2s cubic-bezier(.4,0,.6,1) infinite;border:2px solid var(--color-accent);background:transparent;z-index:var(--layer-1);pointer-events:none}.translucent.svelte-vopvsi.svelte-vopvsi{background:none}@keyframes svelte-vopvsi-pulse{0%,to{opacity:1}50%{opacity:.5}}.loading.svelte-vopvsi.svelte-vopvsi{z-index:var(--layer-2);color:var(--body-text-color)}.eta-bar.svelte-vopvsi.svelte-vopvsi{position:absolute;top:0;right:0;bottom:0;left:0;transform-origin:left;opacity:.8;z-index:var(--layer-1);transition:10ms;background:var(--background-fill-secondary)}.progress-bar-wrap.svelte-vopvsi.svelte-vopvsi{border:1px solid var(--border-color-primary);background:var(--background-fill-primary);width:55.5%;height:var(--size-4)}.progress-bar.svelte-vopvsi.svelte-vopvsi{transform-origin:left;background-color:var(--loader-color);width:var(--size-full);height:var(--size-full)}.progress-level.svelte-vopvsi.svelte-vopvsi{display:flex;flex-direction:column;align-items:center;gap:1;z-index:var(--layer-2);width:var(--size-full)}.progress-level-inner.svelte-vopvsi.svelte-vopvsi{margin:var(--size-2) auto;color:var(--body-text-color);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text.svelte-vopvsi.svelte-vopvsi{position:absolute;top:0;right:0;z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text-center.svelte-vopvsi.svelte-vopvsi{display:flex;position:absolute;top:0;right:0;justify-content:center;align-items:center;transform:translateY(var(--size-6));z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono);text-align:center}.error.svelte-vopvsi.svelte-vopvsi{box-shadow:var(--shadow-drop);border:solid 1px var(--error-border-color);border-radius:var(--radius-full);background:var(--error-background-fill);padding-right:var(--size-4);padding-left:var(--size-4);color:var(--error-text-color);font-weight:var(--weight-semibold);font-size:var(--text-lg);line-height:var(--line-lg);font-family:var(--font)}.minimal.svelte-vopvsi .progress-text.svelte-vopvsi{background:var(--block-background-fill)}.border.svelte-vopvsi.svelte-vopvsi{border:1px solid var(--border-color-primary)}.clear-status.svelte-vopvsi.svelte-vopvsi{position:absolute;display:flex;top:var(--size-2);right:var(--size-2);justify-content:flex-end;gap:var(--spacing-sm);z-index:var(--layer-1)}.toast-body.svelte-solcu7{display:flex;position:relative;right:0;left:0;align-items:center;margin:var(--size-6) var(--size-4);margin:auto;border-radius:var(--container-radius);overflow:hidden;pointer-events:auto}.toast-body.error.svelte-solcu7{border:1px solid var(--color-red-700);background:var(--color-red-50)}.dark .toast-body.error.svelte-solcu7{border:1px solid var(--color-red-500);background-color:var(--color-grey-950)}.toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-700);background:var(--color-yellow-50)}.dark .toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-500);background-color:var(--color-grey-950)}.toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-700);background:var(--color-grey-50)}.dark .toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-500);background-color:var(--color-grey-950)}.toast-title.svelte-solcu7{display:flex;align-items:center;font-weight:var(--weight-bold);font-size:var(--text-lg);line-height:var(--line-sm);text-transform:capitalize}.toast-title.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-title.error.svelte-solcu7{color:var(--color-red-50)}.toast-title.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-title.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-title.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-title.info.svelte-solcu7{color:var(--color-grey-50)}.toast-close.svelte-solcu7{margin:0 var(--size-3);border-radius:var(--size-3);padding:0px var(--size-1-5);font-size:var(--size-5);line-height:var(--size-5)}.toast-close.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-close.error.svelte-solcu7{color:var(--color-red-500)}.toast-close.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-close.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-close.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-close.info.svelte-solcu7{color:var(--color-grey-500)}.toast-text.svelte-solcu7{font-size:var(--text-lg)}.toast-text.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-text.error.svelte-solcu7{color:var(--color-red-50)}.toast-text.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-text.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-text.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-text.info.svelte-solcu7{color:var(--color-grey-50)}.toast-details.svelte-solcu7{margin:var(--size-3) var(--size-3) var(--size-3) 0;width:100%}.toast-icon.svelte-solcu7{display:flex;position:absolute;position:relative;flex-shrink:0;justify-content:center;align-items:center;margin:var(--size-2);border-radius:var(--radius-full);padding:var(--size-1);padding-left:calc(var(--size-1) - 1px);width:35px;height:35px}.toast-icon.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-icon.error.svelte-solcu7{color:var(--color-red-500)}.toast-icon.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-icon.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-icon.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-icon.info.svelte-solcu7{color:var(--color-grey-500)}@keyframes svelte-solcu7-countdown{0%{transform:scaleX(1)}to{transform:scaleX(0)}}.timer.svelte-solcu7{position:absolute;bottom:0;left:0;transform-origin:0 0;animation:svelte-solcu7-countdown 10s linear forwards;width:100%;height:var(--size-1)}.timer.error.svelte-solcu7{background:var(--color-red-700)}.dark .timer.error.svelte-solcu7{background:var(--color-red-500)}.timer.warning.svelte-solcu7{background:var(--color-yellow-700)}.dark .timer.warning.svelte-solcu7{background:var(--color-yellow-500)}.timer.info.svelte-solcu7{background:var(--color-grey-700)}.dark .timer.info.svelte-solcu7{background:var(--color-grey-500)}.toast-wrap.svelte-gatr8h{display:flex;position:fixed;top:var(--size-4);right:var(--size-4);flex-direction:column;align-items:end;gap:var(--size-2);z-index:var(--layer-top);width:calc(100% - var(--size-8))}@media (--screen-sm){.toast-wrap.svelte-gatr8h{width:calc(var(--size-96) + var(--size-10))}}.gallery.svelte-84cxb8{padding:var(--size-1) var(--size-2)}div.svelte-84cxb8{overflow:hidden;min-width:var(--local-text-width);white-space:nowrap}
```

### Comparing `gradio_clickabletextbox-0.0.1/backend/gradio_clickabletextbox/templates/example/index.js` & `gradio_clickabletextbox-0.0.2/backend/gradio_clickabletextbox/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.1/demo/app.py` & `gradio_clickabletextbox-0.0.2/demo/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 import gradio as gr
 from gradio_clickabletextbox import ClickableTextbox
 
-prompts = ["This is a prompt", "This is another prompt", "This is a third prompt"
+prompts = ["This is a prompt", "This is another prompt", "This is a third prompt This is a third promptThis is a third promptThis is a third promptThis is a third promptThis is a third prompt This is a third prompt This is a third prompt"
            ]
 suffixes = ["This is a suffix", "This is another suffix", "This is a third suffix"
             ]
 demo = gr.Interface(
     lambda x: x,
     # interactive version of your component
-    ClickableTextbox(suffixes=suffixes, prompts=prompts,),
+    ClickableTextbox(suffixes=suffixes, prompts=prompts),
     ClickableTextbox(suffixes=suffixes, prompts=prompts,),
 )
 
 if __name__ == "__main__":
-    demo.launch(server_port=1234)
+    demo.launch(server_port=1235)
```

### Comparing `gradio_clickabletextbox-0.0.1/demo/css.css` & `gradio_clickabletextbox-0.0.2/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.1/demo/space.py` & `gradio_clickabletextbox-0.0.2/demo/space.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     ),
 ) as demo:
     gr.Markdown(
 """
 # `gradio_clickabletextbox`
 
 <div style="display: flex; gap: 7px;">
-<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%200.0.1%20-%20orange">  
+<a href="https://pypi.org/project/gradio_clickabletextbox/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/gradio_clickabletextbox"></a>  
 </div>
 
 Python library for easily interacting with trained machine learning models
 """, elem_classes=["md-custom"], header_links=True)
     app.render()
     gr.Markdown(
 """
@@ -38,27 +38,27 @@
 ## Usage
 
 ```python
 
 import gradio as gr
 from gradio_clickabletextbox import ClickableTextbox
 
-prompts = ["This is a prompt", "This is another prompt", "This is a third prompt"
+prompts = ["This is a prompt", "This is another prompt", "This is a third prompt This is a third promptThis is a third promptThis is a third promptThis is a third promptThis is a third prompt This is a third prompt This is a third prompt"
            ]
 suffixes = ["This is a suffix", "This is another suffix", "This is a third suffix"
             ]
 demo = gr.Interface(
     lambda x: x,
     # interactive version of your component
-    ClickableTextbox(suffixes=suffixes, prompts=prompts,),
+    ClickableTextbox(suffixes=suffixes, prompts=prompts),
     ClickableTextbox(suffixes=suffixes, prompts=prompts,),
 )
 
 if __name__ == "__main__":
-    demo.launch(server_port=1234)
+    demo.launch(server_port=1235)
 
 ```
 """, elem_classes=["md-custom"], header_links=True)
 
 
     gr.Markdown("""
 ## `ClickableTextbox`
```

### Comparing `gradio_clickabletextbox-0.0.1/frontend/Example.svelte` & `gradio_clickabletextbox-0.0.2/frontend/Example.svelte`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.1/frontend/Index.svelte` & `gradio_clickabletextbox-0.0.2/frontend/Index.svelte`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.1/frontend/package-lock.json` & `gradio_clickabletextbox-0.0.2/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.1/frontend/package.json` & `gradio_clickabletextbox-0.0.2/frontend/package.json`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.1/frontend/shared/Textbox.svelte` & `gradio_clickabletextbox-0.0.2/frontend/shared/Textbox.svelte`

 * *Files 8% similar despite different names*

```diff
@@ -3,40 +3,41 @@
 		beforeUpdate,
 		afterUpdate,
 		createEventDispatcher,
 		tick,
 	} from "svelte";
 	import { BlockTitle } from "@gradio/atoms";
 	import type { SelectData } from "@gradio/utils";
-	import { fade } from "svelte/transition";
+	import { fadeSlide } from "./transitions.js";
 
 	export let value = "";
 	export let value_is_output = false;
 	export let lines = 1;
 	export let placeholder = "Type here...";
 	export let label: string;
 	export let info: string | undefined = undefined;
 	export let disabled = false;
 	export let show_label = true;
 	export let container = true;
 	export let max_lines: number;
 	export let prompts: string[] = [];
 	export let suffixes: string[] = [];
-	export let type: "text" | "password" | "email" = "text";
 	export let rtl = false;
 	export let autofocus = false;
 	export let text_align: "left" | "right" | undefined = undefined;
 	export let autoscroll = true;
 
 	let el: HTMLTextAreaElement | HTMLInputElement;
 	let show_menu = false;
 	let can_scroll: boolean;
 	let previous_scroll_top = 0;
 	let user_has_scrolled_up = false;
 
+	let show_magic = prompts.length > 0 || suffixes.length > 0;
+
 	$: value, el && lines !== max_lines && resize({ target: el });
 
 	$: if (value === null) value = "";
 
 	const dispatch = createEventDispatcher<{
 		change: string;
 		submit: undefined;
@@ -172,54 +173,56 @@
 	}
 </script>
 
 <!-- svelte-ignore a11y-autofocus -->
 <label class:container>
 	<BlockTitle {show_label} {info}>{label}</BlockTitle>
 	<div class="input-container">
-		<textarea
-			data-testid="textbox"
-			use:text_area_resize={value}
-			class="scroll-hide"
-			dir={rtl ? "rtl" : "ltr"}
-			bind:value
-			bind:this={el}
-			{placeholder}
-			rows={lines}
-			{disabled}
-			{autofocus}
-			on:keypress={handle_keypress}
-			on:blur
-			on:select={handle_select}
-			on:focus
-			on:scroll={handle_scroll}
-			style={text_align ? "text-align: " + text_align : ""}
-		/>
-
-		{#if show_menu && (prompts.length > 0 || suffixes.length > 0)}
-			<button
-				class="extend_button"
-				on:click={handle_extension}
-				aria-label="Extend"
-				aria-roledescription="Extend text"
-			>
-				<svg
-					width="26"
-					height="26"
-					viewBox="0 0 26 26"
-					fill="none"
-					xmlns="http://www.w3.org/2000/svg"
+		{#if show_menu && show_magic}
+			<div class="magic_container">
+				<textarea
+					data-testid="textbox"
+					use:text_area_resize={value}
+					class={show_magic ? "scroll_hide_magic" : "scroll-hide"}
+					dir={rtl ? "rtl" : "ltr"}
+					bind:value
+					bind:this={el}
+					{placeholder}
+					rows={lines}
+					{disabled}
+					{autofocus}
+					on:keypress={handle_keypress}
+					on:blur
+					on:select={handle_select}
+					on:focus
+					on:scroll={handle_scroll}
+					style={text_align ? "text-align: " + text_align : ""}
+				/>
+				<button
+					class="extend_button"
+					on:click={handle_extension}
+					aria-label="Extend"
+					aria-roledescription="Extend text"
 				>
-					<path
-						d="M23.0978 15.6987L23.5777 15.2188L21.7538 13.3952L21.2739 13.8751L23.0978 15.6987ZM11.1253 2.74873L10.6454 3.22809L12.4035 4.98733L12.8834 4.50769L11.1253 2.74873ZM25.5996 9.23801H22.885V9.91673H25.5996V9.23801ZM10.6692 9.23801H7.95457V9.91673H10.6692V9.23801ZM21.8008 5.01533L23.5982 3.21773L23.118 2.73781L21.3206 4.53541L21.8008 5.01533ZM17.2391 7.29845L18.6858 8.74521C18.7489 8.80822 18.7989 8.88303 18.8331 8.96538C18.8672 9.04773 18.8847 9.13599 18.8847 9.22513C18.8847 9.31427 18.8672 9.40254 18.8331 9.48488C18.7989 9.56723 18.7489 9.64205 18.6858 9.70505L3.00501 25.3859C2.74013 25.6511 2.31061 25.6511 2.04517 25.3859L0.598406 23.9391C0.535351 23.8761 0.485329 23.8013 0.4512 23.719C0.417072 23.6366 0.399506 23.5483 0.399506 23.4592C0.399506 23.3701 0.417072 23.2818 0.4512 23.1995C0.485329 23.1171 0.535351 23.0423 0.598406 22.9793L16.2792 7.29845C16.3422 7.23533 16.417 7.18525 16.4994 7.15108C16.5817 7.11691 16.67 7.09932 16.7592 7.09932C16.8483 7.09932 16.9366 7.11691 17.019 7.15108C17.1013 7.18525 17.1761 7.23533 17.2391 7.29845ZM14.4231 13.2042L18.3792 9.24893L16.746 7.61541L12.7899 11.5713L14.4231 13.2042ZM17.4555 0.415771H16.7768V3.13037H17.4555V0.415771ZM17.4555 15.3462H16.7768V18.0608H17.4555V15.3462Z"
-						fill="#ff6700"
-					/>
-				</svg>
-			</button>
-			<div class="menu" transition:fade>
+					<svg
+						width="26"
+						height="26"
+						viewBox="0 0 26 26"
+						fill="none"
+						xmlns="http://www.w3.org/2000/svg"
+					>
+						<path
+							d="M23.0978 15.6987L23.5777 15.2188L21.7538 13.3952L21.2739 13.8751L23.0978 15.6987ZM11.1253 2.74873L10.6454 3.22809L12.4035 4.98733L12.8834 4.50769L11.1253 2.74873ZM25.5996 9.23801H22.885V9.91673H25.5996V9.23801ZM10.6692 9.23801H7.95457V9.91673H10.6692V9.23801ZM21.8008 5.01533L23.5982 3.21773L23.118 2.73781L21.3206 4.53541L21.8008 5.01533ZM17.2391 7.29845L18.6858 8.74521C18.7489 8.80822 18.7989 8.88303 18.8331 8.96538C18.8672 9.04773 18.8847 9.13599 18.8847 9.22513C18.8847 9.31427 18.8672 9.40254 18.8331 9.48488C18.7989 9.56723 18.7489 9.64205 18.6858 9.70505L3.00501 25.3859C2.74013 25.6511 2.31061 25.6511 2.04517 25.3859L0.598406 23.9391C0.535351 23.8761 0.485329 23.8013 0.4512 23.719C0.417072 23.6366 0.399506 23.5483 0.399506 23.4592C0.399506 23.3701 0.417072 23.2818 0.4512 23.1995C0.485329 23.1171 0.535351 23.0423 0.598406 22.9793L16.2792 7.29845C16.3422 7.23533 16.417 7.18525 16.4994 7.15108C16.5817 7.11691 16.67 7.09932 16.7592 7.09932C16.8483 7.09932 16.9366 7.11691 17.019 7.15108C17.1013 7.18525 17.1761 7.23533 17.2391 7.29845ZM14.4231 13.2042L18.3792 9.24893L16.746 7.61541L12.7899 11.5713L14.4231 13.2042ZM17.4555 0.415771H16.7768V3.13037H17.4555V0.415771ZM17.4555 15.3462H16.7768V18.0608H17.4555V15.3462Z"
+							fill="#ff6700"
+						/>
+					</svg>
+				</button>
+			</div>
+
+			<div class="menu" transition:fadeSlide>
 				{#if prompts.length > 0}
 					<div class="menu_section">
 						<span> Best prompt structures </span>
 						<ul>
 							{#each prompts as word}
 								<li>
 									<button
@@ -269,34 +272,73 @@
 									>
 								</li>
 							{/each}
 						</ul>
 					</div>
 				{/if}
 			</div>
-		{:else if prompts.length > 0 || suffixes.length > 0}
-			<button
-				class="extend_button"
-				on:click={handle_extension}
-				aria-label="Extend"
-				aria-roledescription="Extend text"
-			>
-				<svg
-					width="26"
-					height="26"
-					viewBox="0 0 26 26"
-					fill="none"
-					xmlns="http://www.w3.org/2000/svg"
+		{:else if !show_menu && show_magic}
+			<div class="magic_container">
+				<textarea
+					data-testid="textbox"
+					use:text_area_resize={value}
+					class={show_magic ? "scroll_hide_magic" : "scroll-hide"}
+					dir={rtl ? "rtl" : "ltr"}
+					bind:value
+					bind:this={el}
+					{placeholder}
+					rows={lines}
+					{disabled}
+					{autofocus}
+					on:keypress={handle_keypress}
+					on:blur
+					on:select={handle_select}
+					on:focus
+					on:scroll={handle_scroll}
+					style={text_align ? "text-align: " + text_align : ""}
+				/>
+				<button
+					class="extend_button"
+					on:click={handle_extension}
+					aria-label="Extend"
+					aria-roledescription="Extend text"
 				>
-					<path
-						d="M23.0978 15.6987L23.5777 15.2188L21.7538 13.3952L21.2739 13.8751L23.0978 15.6987ZM11.1253 2.74873L10.6454 3.22809L12.4035 4.98733L12.8834 4.50769L11.1253 2.74873ZM25.5996 9.23801H22.885V9.91673H25.5996V9.23801ZM10.6692 9.23801H7.95457V9.91673H10.6692V9.23801ZM21.8008 5.01533L23.5982 3.21773L23.118 2.73781L21.3206 4.53541L21.8008 5.01533ZM17.2391 7.29845L18.6858 8.74521C18.7489 8.80822 18.7989 8.88303 18.8331 8.96538C18.8672 9.04773 18.8847 9.13599 18.8847 9.22513C18.8847 9.31427 18.8672 9.40254 18.8331 9.48488C18.7989 9.56723 18.7489 9.64205 18.6858 9.70505L3.00501 25.3859C2.74013 25.6511 2.31061 25.6511 2.04517 25.3859L0.598406 23.9391C0.535351 23.8761 0.485329 23.8013 0.4512 23.719C0.417072 23.6366 0.399506 23.5483 0.399506 23.4592C0.399506 23.3701 0.417072 23.2818 0.4512 23.1995C0.485329 23.1171 0.535351 23.0423 0.598406 22.9793L16.2792 7.29845C16.3422 7.23533 16.417 7.18525 16.4994 7.15108C16.5817 7.11691 16.67 7.09932 16.7592 7.09932C16.8483 7.09932 16.9366 7.11691 17.019 7.15108C17.1013 7.18525 17.1761 7.23533 17.2391 7.29845ZM14.4231 13.2042L18.3792 9.24893L16.746 7.61541L12.7899 11.5713L14.4231 13.2042ZM17.4555 0.415771H16.7768V3.13037H17.4555V0.415771ZM17.4555 15.3462H16.7768V18.0608H17.4555V15.3462Z"
-						fill="#CCCCCC"
-					/>
-				</svg>
-			</button>
+					<svg
+						width="26"
+						height="26"
+						viewBox="0 0 26 26"
+						fill="none"
+						xmlns="http://www.w3.org/2000/svg"
+					>
+						<path
+							d="M23.0978 15.6987L23.5777 15.2188L21.7538 13.3952L21.2739 13.8751L23.0978 15.6987ZM11.1253 2.74873L10.6454 3.22809L12.4035 4.98733L12.8834 4.50769L11.1253 2.74873ZM25.5996 9.23801H22.885V9.91673H25.5996V9.23801ZM10.6692 9.23801H7.95457V9.91673H10.6692V9.23801ZM21.8008 5.01533L23.5982 3.21773L23.118 2.73781L21.3206 4.53541L21.8008 5.01533ZM17.2391 7.29845L18.6858 8.74521C18.7489 8.80822 18.7989 8.88303 18.8331 8.96538C18.8672 9.04773 18.8847 9.13599 18.8847 9.22513C18.8847 9.31427 18.8672 9.40254 18.8331 9.48488C18.7989 9.56723 18.7489 9.64205 18.6858 9.70505L3.00501 25.3859C2.74013 25.6511 2.31061 25.6511 2.04517 25.3859L0.598406 23.9391C0.535351 23.8761 0.485329 23.8013 0.4512 23.719C0.417072 23.6366 0.399506 23.5483 0.399506 23.4592C0.399506 23.3701 0.417072 23.2818 0.4512 23.1995C0.485329 23.1171 0.535351 23.0423 0.598406 22.9793L16.2792 7.29845C16.3422 7.23533 16.417 7.18525 16.4994 7.15108C16.5817 7.11691 16.67 7.09932 16.7592 7.09932C16.8483 7.09932 16.9366 7.11691 17.019 7.15108C17.1013 7.18525 17.1761 7.23533 17.2391 7.29845ZM14.4231 13.2042L18.3792 9.24893L16.746 7.61541L12.7899 11.5713L14.4231 13.2042ZM17.4555 0.415771H16.7768V3.13037H17.4555V0.415771ZM17.4555 15.3462H16.7768V18.0608H17.4555V15.3462Z"
+							fill="#CCCCCC"
+						/>
+					</svg>
+				</button>
+			</div>
+		{:else}
+			<textarea
+				data-testid="textbox"
+				use:text_area_resize={value}
+				class={show_magic ? "scroll_hide_magic" : "scroll-hide"}
+				dir={rtl ? "rtl" : "ltr"}
+				bind:value
+				bind:this={el}
+				{placeholder}
+				rows={lines}
+				{disabled}
+				{autofocus}
+				on:keypress={handle_keypress}
+				on:blur
+				on:select={handle_select}
+				on:focus
+				on:scroll={handle_scroll}
+				style={text_align ? "text-align: " + text_align : ""}
+			/>
 		{/if}
 	</div>
 </label>
 
 <style>
 	label {
 		display: block;
@@ -332,42 +374,33 @@
 	textarea:disabled {
 		-webkit-text-fill-color: var(--body-text-color);
 		-webkit-opacity: 1;
 		opacity: 1;
 	}
 
 	input:focus,
-	textarea:focus {
-		box-shadow: var(--input-shadow-focus);
-		border-color: var(--input-border-color-focus);
-	}
-
 	input::placeholder,
 	textarea::placeholder {
 		color: var(--input-placeholder-color);
 	}
 	.extend_button {
 		display: flex;
-		position: absolute;
-		top: 45px;
-		right: 20px;
+		position: relative;
 		align-items: center;
-		background: var(--block-label-background-fill);
 		width: 20px;
 		height: 20px;
 		overflow: hidden;
 		color: var(--block-label-color);
 		font: var(--font-sans);
 		font-size: var(--button-small-text-size);
 	}
 
 	.extend_button:hover path {
 		--ring-color: var(--color-accent);
 		filter: brightness(1.1);
-		transform: scale(1.05);
 		fill: #ff6700;
 	}
 
 	.menu_section {
 		padding: 12px 0px 0px 0px;
 		align-items: center;
 		color: #100700;
@@ -395,14 +428,15 @@
 
 	.menu {
 		border-radius: 0px 0px 15px 15px;
 		background: rgba(204, 204, 204, 0.1);
 		margin: 0px 16px;
 		padding: 0px 14px 12px 14px;
 	}
+
 	.menu li {
 		width: 100%;
 	}
 
 	.text_extension_button {
 		border-radius: 15px;
 		border: 0.5px solid #ff9a57;
@@ -420,45 +454,66 @@
 		padding: 8px 12px;
 		justify-content: space-between;
 		align-items: center;
 		border-radius: 10px;
 		border: 0.5px solid #ff9a57;
 		background: #fff4ea;
 		color: #101111;
-		text-align: justify;
+		text-align: left;
 		font-size: 13px;
 		font-style: normal;
 		font-weight: 300;
 		line-height: normal;
 		gap: 4px;
 		flex-wrap: wrap;
 		flex-direction: row;
 	}
 
 	.text_extension_button_prompt:hover {
 		color: #fff;
 		fill: #fff;
-		text-align: center;
-		font-size: 13px;
-		font-style: normal;
-		font-weight: 300;
-		border-radius: 10px;
-		border: 0.5px solid #ff9a57;
 		background: var(--Light-Orange, #ff9a57);
 	}
 	.text_extension_button_prompt:hover svg path {
 		fill: #fff;
 	}
 	.text_extension_button:hover {
 		color: #fff;
-		text-align: center;
-		font-size: 13px;
-		font-style: normal;
-		font-weight: 300;
-		border-radius: 10px;
-		border: 0.5px solid #ff9a57;
 		background: var(--Light-Orange, #ff9a57);
 	}
 	.text_extension_button:hover svg path {
 		fill: #fff;
 	}
+
+	.magic_container {
+		display: flex;
+		position: relative;
+		outline: none !important;
+		box-shadow: var(--input-shadow);
+		padding: var(--input-padding);
+		width: 100%;
+		color: var(--body-text-color);
+		font-weight: var(--input-text-weight);
+		font-size: var(--input-text-size);
+		line-height: var(--line-sm);
+		border: none;
+		scrollbar-width: none;
+		resize: none;
+		align-items: center;
+	}
+
+	.scroll_hide_magic {
+		display: block;
+		position: relative;
+		outline: none !important;
+		box-shadow: none;
+		padding: var(--input-padding);
+		width: 100%;
+		color: var(--body-text-color);
+		font-weight: var(--input-text-weight);
+		font-size: var(--input-text-size);
+		line-height: var(--line-sm);
+		border: none;
+		scrollbar-width: none;
+		resize: none;
+	}
 </style>
```

#### html2text {}

```diff
@@ -1,17 +1,27 @@
 show_label} {info}>{label}
-"rtl" : "ltr"} bind:value bind:this={el} {placeholder} rows={lines} {disabled}
-{autofocus} on:keypress={handle_keypress} on:blur on:select={handle_select} on:
-focus on:scroll={handle_scroll} style={text_align ? "text-align: " + text_align
-: ""} /> {#if show_menu && (prompts.length > 0 || suffixes.length > 0)}
+{#if show_menu && show_magic}
+"scroll_hide_magic" : "scroll-hide"} dir={rtl ? "rtl" : "ltr"} bind:value bind:
+this={el} {placeholder} rows={lines} {disabled} {autofocus} on:keypress=
+{handle_keypress} on:blur on:select={handle_select} on:focus on:scroll=
+{handle_scroll} style={text_align ? "text-align: " + text_align : ""} />
 {#if prompts.length > 0}
 Best prompt structures
     * {#each prompts as word}
     * > addToTextbox(word)} >{word}
 {/each}
 {/if} {#if suffixes.length > 0}
 Best style keywords
     * {#each suffixes as word}
     * > addToTextbox(word)} >{word}
 {/each}
 {/if}
-{:else if prompts.length > 0 || suffixes.length > 0} {/if}
+{:else if !show_menu && show_magic}
+"scroll_hide_magic" : "scroll-hide"} dir={rtl ? "rtl" : "ltr"} bind:value bind:
+this={el} {placeholder} rows={lines} {disabled} {autofocus} on:keypress=
+{handle_keypress} on:blur on:select={handle_select} on:focus on:scroll=
+{handle_scroll} style={text_align ? "text-align: " + text_align : ""} />
+{:else}
+"scroll_hide_magic" : "scroll-hide"} dir={rtl ? "rtl" : "ltr"} bind:value bind:
+this={el} {placeholder} rows={lines} {disabled} {autofocus} on:keypress=
+{handle_keypress} on:blur on:select={handle_select} on:focus on:scroll=
+{handle_scroll} style={text_align ? "text-align: " + text_align : ""} /> {/if}
```

### Comparing `gradio_clickabletextbox-0.0.1/README.md` & `gradio_clickabletextbox-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,10 @@
----
-tags: [gradio-custom-component, Textbox]
-title: gradio_clickabletextbox
-short_description:
-colorFrom: blue
-colorTo: yellow
-sdk: gradio
-pinned: false
-app_file: space.py
----
 
 # `gradio_clickabletextbox`
-<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%200.0.1%20-%20orange">  
+<a href="https://pypi.org/project/gradio_clickabletextbox/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/gradio_clickabletextbox"></a>  
 
 Python library for easily interacting with trained machine learning models
 
 ## Installation
 
 ```bash
 pip install gradio_clickabletextbox
@@ -23,27 +13,27 @@
 ## Usage
 
 ```python
 
 import gradio as gr
 from gradio_clickabletextbox import ClickableTextbox
 
-prompts = ["This is a prompt", "This is another prompt", "This is a third prompt"
+prompts = ["This is a prompt", "This is another prompt", "This is a third prompt This is a third promptThis is a third promptThis is a third promptThis is a third promptThis is a third prompt This is a third prompt This is a third prompt"
            ]
 suffixes = ["This is a suffix", "This is another suffix", "This is a third suffix"
             ]
 demo = gr.Interface(
     lambda x: x,
     # interactive version of your component
-    ClickableTextbox(suffixes=suffixes, prompts=prompts,),
+    ClickableTextbox(suffixes=suffixes, prompts=prompts),
     ClickableTextbox(suffixes=suffixes, prompts=prompts,),
 )
 
 if __name__ == "__main__":
-    demo.launch(server_port=1234)
+    demo.launch(server_port=1235)
 
 ```
 
 ## `ClickableTextbox`
 
 ### Initialization
```

### Comparing `gradio_clickabletextbox-0.0.1/pyproject.toml` & `gradio_clickabletextbox-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_clickabletextbox"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python library for easily interacting with trained machine learning models"
 readme = "README.md"
 license = "apache-2.0"
 requires-python = ">=3.8"
 authors = [{ name = "YOUR NAME", email = "YOUREMAIL@domain.com" }]
 keywords = ["gradio-custom-component", "gradio-template-Textbox"]
 # Add dependencies here
@@ -41,11 +41,11 @@
 # repository = "your github repository"
 # space = "your space url"
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
 [tool.hatch.build]
-artifacts = ["/backend/gradio_clickabletextbox/templates", "*.pyi"]
+artifacts = ["/backend/gradio_clickabletextbox/templates", "*.pyi", "/home/antoine/.cache/pypoetry/virtualenvs/gen-design-interface-xtCO5_LN-py3.10/lib/python3.10/site-packages/gradio_clickabletextbox/templates"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["/backend/gradio_clickabletextbox"]
```

### Comparing `gradio_clickabletextbox-0.0.1/PKG-INFO` & `gradio_clickabletextbox-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gradio_clickabletextbox
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library for easily interacting with trained machine learning models
 Author-email: YOUR NAME <YOUREMAIL@domain.com>
 License-Expression: Apache-2.0
 Keywords: gradio-custom-component,gradio-template-Textbox
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -19,27 +19,17 @@
 Requires-Python: >=3.8
 Requires-Dist: gradio<5.0,>=4.0
 Provides-Extra: dev
 Requires-Dist: build; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
 Description-Content-Type: text/markdown
 
----
-tags: [gradio-custom-component, Textbox]
-title: gradio_clickabletextbox
-short_description:
-colorFrom: blue
-colorTo: yellow
-sdk: gradio
-pinned: false
-app_file: space.py
----
 
 # `gradio_clickabletextbox`
-<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%200.0.1%20-%20orange">  
+<a href="https://pypi.org/project/gradio_clickabletextbox/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/gradio_clickabletextbox"></a>  
 
 Python library for easily interacting with trained machine learning models
 
 ## Installation
 
 ```bash
 pip install gradio_clickabletextbox
@@ -48,27 +38,27 @@
 ## Usage
 
 ```python
 
 import gradio as gr
 from gradio_clickabletextbox import ClickableTextbox
 
-prompts = ["This is a prompt", "This is another prompt", "This is a third prompt"
+prompts = ["This is a prompt", "This is another prompt", "This is a third prompt This is a third promptThis is a third promptThis is a third promptThis is a third promptThis is a third prompt This is a third prompt This is a third prompt"
            ]
 suffixes = ["This is a suffix", "This is another suffix", "This is a third suffix"
             ]
 demo = gr.Interface(
     lambda x: x,
     # interactive version of your component
-    ClickableTextbox(suffixes=suffixes, prompts=prompts,),
+    ClickableTextbox(suffixes=suffixes, prompts=prompts),
     ClickableTextbox(suffixes=suffixes, prompts=prompts,),
 )
 
 if __name__ == "__main__":
-    demo.launch(server_port=1234)
+    demo.launch(server_port=1235)
 
 ```
 
 ## `ClickableTextbox`
 
 ### Initialization
```

