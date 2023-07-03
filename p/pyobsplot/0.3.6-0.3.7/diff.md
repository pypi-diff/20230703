# Comparing `tmp/pyobsplot-0.3.6.tar.gz` & `tmp/pyobsplot-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobsplot-0.3.6.tar", max compression
+gzip compressed data, was "pyobsplot-0.3.7.tar", max compression
```

## Comparing `pyobsplot-0.3.6.tar` & `pyobsplot-0.3.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1071 2023-03-29 08:42:01.834769 pyobsplot-0.3.6/LICENSE
--rw-r--r--   0        0        0     4361 2023-06-06 12:48:48.704316 pyobsplot-0.3.6/README.md
--rw-r--r--   0        0        0     1303 2023-06-08 14:08:25.570442 pyobsplot-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      535 2023-04-23 14:58:02.739444 pyobsplot-0.3.6/src/pyobsplot/__init__.py
--rw-r--r--   0        0        0     3428 2023-06-08 13:58:25.559409 pyobsplot-0.3.6/src/pyobsplot/data.py
--rw-r--r--   0        0        0     2116 2023-06-02 14:29:52.114261 pyobsplot-0.3.6/src/pyobsplot/jsdom.py
--rw-r--r--   0        0        0     2363 2023-04-14 11:09:43.659346 pyobsplot-0.3.6/src/pyobsplot/jsmodules.py
--rw-r--r--   0        0        0     6828 2023-06-06 12:24:31.708831 pyobsplot-0.3.6/src/pyobsplot/obsplot.py
--rw-r--r--   0        0        0     6158 2023-06-02 14:23:54.640414 pyobsplot-0.3.6/src/pyobsplot/parsing.py
--rw-r--r--   0        0        0      701 2023-06-08 14:00:43.500033 pyobsplot-0.3.6/src/pyobsplot/static/styles.css
--rw-r--r--   0        0        0  1348137 2023-06-08 14:00:43.500033 pyobsplot-0.3.6/src/pyobsplot/static/widget.js
--rw-r--r--   0        0        0     2771 2023-06-08 14:08:35.350543 pyobsplot-0.3.6/src/pyobsplot/utils.py
--rw-r--r--   0        0        0     1635 2023-06-07 16:56:23.676710 pyobsplot-0.3.6/src/pyobsplot/widget.py
--rw-r--r--   0        0        0     5719 1970-01-01 00:00:00.000000 pyobsplot-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-03-29 08:42:01.834769 pyobsplot-0.3.7/LICENSE
+-rw-r--r--   0        0        0     4361 2023-06-06 12:48:48.704316 pyobsplot-0.3.7/README.md
+-rw-r--r--   0        0        0     1303 2023-07-03 12:20:09.373736 pyobsplot-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      536 2023-06-29 12:08:57.805896 pyobsplot-0.3.7/src/pyobsplot/__init__.py
+-rw-r--r--   0        0        0     3428 2023-06-08 13:58:25.559409 pyobsplot-0.3.7/src/pyobsplot/data.py
+-rw-r--r--   0        0        0     2363 2023-06-29 08:35:17.128683 pyobsplot-0.3.7/src/pyobsplot/js_modules.py
+-rw-r--r--   0        0        0     2116 2023-06-02 14:29:52.114261 pyobsplot-0.3.7/src/pyobsplot/jsdom.py
+-rw-r--r--   0        0        0     7106 2023-06-29 12:14:24.235900 pyobsplot-0.3.7/src/pyobsplot/obsplot.py
+-rw-r--r--   0        0        0     6158 2023-06-02 14:23:54.640414 pyobsplot-0.3.7/src/pyobsplot/parsing.py
+-rw-r--r--   0        0        0      745 2023-06-29 13:58:47.524270 pyobsplot-0.3.7/src/pyobsplot/static/static-styles.css
+-rw-r--r--   0        0        0  1353891 2023-06-29 13:58:47.524270 pyobsplot-0.3.7/src/pyobsplot/static/static-widget.js
+-rw-r--r--   0        0        0     2771 2023-06-29 08:08:10.143368 pyobsplot-0.3.7/src/pyobsplot/utils.py
+-rw-r--r--   0        0        0     1649 2023-06-28 13:02:16.644582 pyobsplot-0.3.7/src/pyobsplot/widget.py
+-rw-r--r--   0        0        0     5719 1970-01-01 00:00:00.000000 pyobsplot-0.3.7/PKG-INFO
```

### Comparing `pyobsplot-0.3.6/LICENSE` & `pyobsplot-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.6/README.md` & `pyobsplot-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.6/pyproject.toml` & `pyobsplot-0.3.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyobsplot"
-version = "0.3.6"
+version = "0.3.7"
 description = "Observable Plot in Jupyter notebooks and Quarto documents"
 authors = ["Julien Barnier <julien@nozav.org>"]
 license = "MIT"
 readme = "README.md"
 include = ["src/pyobsplot/static/*"]
 homepage = "https://github.com/juba/pyobsplot"
 documentation = "https://juba.github.io/pyobsplot"
@@ -19,15 +19,15 @@
 ]
 
 [tool.poetry.urls]
 changelog = "https://github.com/juba/pyobsplot/blob/main/NEWS.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-anywidget = {extras = ["dev"], version = "^0.4.3"}
+anywidget = {extras = ["dev"], version = "^0.6.0"}
 pandas = ">=1.2.0"
 polars = ">=0.16.0"
 pyarrow = "^11.0.0"
 ipywidgets = ">=8.0.0"
 jupyterlab_widgets = ">=3.0.0"
 jupyterlab = ">=3.6.0"
 requests = "^2.28.2"
```

### Comparing `pyobsplot-0.3.6/src/pyobsplot/__init__.py` & `pyobsplot-0.3.7/src/pyobsplot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,10 +8,10 @@
     __version__ = version("pyobsplot")
 except PackageNotFoundError:
     __version__ = "uninstalled"
 
 
 from .obsplot import Obsplot  # noqa:F401
 from .parsing import js  # noqa:F401
-from .jsmodules import Plot, d3, Math  # noqa:F401
+from .js_modules import Plot, d3, Math  # noqa:F401
 
 __all__ = ["Obsplot", "Plot", "d3", "Math", "js", "__version__"]
```

### Comparing `pyobsplot-0.3.6/src/pyobsplot/data.py` & `pyobsplot-0.3.7/src/pyobsplot/data.py`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.6/src/pyobsplot/jsdom.py` & `pyobsplot-0.3.7/src/pyobsplot/jsdom.py`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.6/src/pyobsplot/jsmodules.py` & `pyobsplot-0.3.7/src/pyobsplot/js_modules.py`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.6/src/pyobsplot/obsplot.py` & `pyobsplot-0.3.7/src/pyobsplot/obsplot.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,14 +96,30 @@
         return (
             f"<{type(self).__name__}>\n"
             f"theme: {self._theme!r}\n"
             f"debug: {self._debug!r}\n"
             f"default: {self._default!r}\n"
         )
 
+    @property
+    def theme(self):
+        return self._theme
+
+    @theme.setter
+    def theme(self, val):
+        self._theme = val
+
+    @property
+    def default(self):
+        return self._default
+
+    @default.setter
+    def default(self, val):
+        self._default = val
+
     def get_spec(self, *args, **kwargs):
         """
         Extract plot specification from args and kwargs, taking into account
         the alternative specification syntaxes.
         """
 
         # Only one dict arg -> spec passed as dict
```

### Comparing `pyobsplot-0.3.6/src/pyobsplot/parsing.py` & `pyobsplot-0.3.7/src/pyobsplot/parsing.py`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.6/src/pyobsplot/static/widget.js` & `pyobsplot-0.3.7/src/pyobsplot/static/static-widget.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -9546,16 +9546,16 @@
         triangles,
         coords
     } = d;
     for (let i = 0; i < triangles.length; i += 3) {
         const a4 = 2 * triangles[i],
             b = 2 * triangles[i + 1],
             c6 = 2 * triangles[i + 2],
-            cross2 = (coords[c6] - coords[a4]) * (coords[b + 1] - coords[a4 + 1]) - (coords[b] - coords[a4]) * (coords[c6 + 1] - coords[a4 + 1]);
-        if (cross2 > 1e-10)
+            cross3 = (coords[c6] - coords[a4]) * (coords[b + 1] - coords[a4 + 1]) - (coords[b] - coords[a4]) * (coords[c6 + 1] - coords[a4 + 1]);
+        if (cross3 > 1e-10)
             return false;
     }
     return true;
 }
 
 function jitter(x4, y4, r) {
     return [x4 + Math.sin(x4 + y4) * r, y4 + Math.cos(x4 - y4) * r];
@@ -17534,15 +17534,15 @@
         weekdayLookup = formatLookup(locale_weekdays),
         shortWeekdayRe = formatRe(locale_shortWeekdays),
         shortWeekdayLookup = formatLookup(locale_shortWeekdays),
         monthRe = formatRe(locale_months),
         monthLookup = formatLookup(locale_months),
         shortMonthRe = formatRe(locale_shortMonths),
         shortMonthLookup = formatLookup(locale_shortMonths);
-    var formats = {
+    var formats2 = {
         "a": formatShortWeekday,
         "A": formatWeekday2,
         "b": formatShortMonth,
         "B": formatMonth2,
         "c": null,
         "d": formatDayOfMonth,
         "e": formatDayOfMonth,
@@ -17636,22 +17636,22 @@
         "x": parseLocaleDate,
         "X": parseLocaleTime,
         "y": parseYear,
         "Y": parseFullYear,
         "Z": parseZone,
         "%": parseLiteralPercent
     };
-    formats.x = newFormat(locale_date, formats);
-    formats.X = newFormat(locale_time, formats);
-    formats.c = newFormat(locale_dateTime, formats);
+    formats2.x = newFormat(locale_date, formats2);
+    formats2.X = newFormat(locale_time, formats2);
+    formats2.c = newFormat(locale_dateTime, formats2);
     utcFormats.x = newFormat(locale_date, utcFormats);
     utcFormats.X = newFormat(locale_time, utcFormats);
     utcFormats.c = newFormat(locale_dateTime, utcFormats);
 
-    function newFormat(specifier, formats2) {
+    function newFormat(specifier, formats3) {
         return function(date2) {
             var string2 = [],
                 i = -1,
                 j = 0,
                 n = specifier.length,
                 c6, pad4, format3;
             if (!(date2 instanceof Date))
@@ -17659,15 +17659,15 @@
             while (++i < n) {
                 if (specifier.charCodeAt(i) === 37) {
                     string2.push(specifier.slice(j, i));
                     if ((pad4 = pads[c6 = specifier.charAt(++i)]) != null)
                         c6 = specifier.charAt(++i);
                     else
                         pad4 = c6 === "e" ? " " : "0";
-                    if (format3 = formats2[c6])
+                    if (format3 = formats3[c6])
                         c6 = format3(date2, pad4);
                     string2.push(c6);
                     j = i + 1;
                 }
             }
             string2.push(specifier.slice(j, i));
             return string2.join("");
@@ -17830,15 +17830,15 @@
     }
 
     function formatUTCQuarter(d) {
         return 1 + ~~(d.getUTCMonth() / 3);
     }
     return {
         format: function(specifier) {
-            var f = newFormat(specifier += "", formats);
+            var f = newFormat(specifier += "", formats2);
             f.toString = function() {
                 return specifier;
             };
             return f;
         },
         parse: function(specifier) {
             var p = newParse(specifier += "", false);
@@ -21616,14 +21616,36 @@
 function parse(string2, fallback) {
     if (!re2.test(string2 += ""))
         return typeof fallback === "function" ? fallback(string2) : fallback;
     return new Date(string2);
 }
 
 // node_modules/@observablehq/plot/src/time.js
+var durationSecond2 = 1e3;
+var durationMinute2 = durationSecond2 * 60;
+var durationHour2 = durationMinute2 * 60;
+var durationDay2 = durationHour2 * 24;
+var durationWeek2 = durationDay2 * 7;
+var durationMonth2 = durationDay2 * 30;
+var durationYear2 = durationDay2 * 365;
+var formats = [
+    ["millisecond", 0.5 * durationSecond2],
+    ["second", durationSecond2],
+    ["second", 30 * durationSecond2],
+    ["minute", durationMinute2],
+    ["minute", 30 * durationMinute2],
+    ["hour", durationHour2],
+    ["hour", 12 * durationHour2],
+    ["day", durationDay2],
+    ["day", 2 * durationDay2],
+    ["week", durationWeek2],
+    ["month", durationMonth2],
+    ["month", 3 * durationMonth2],
+    ["year", durationYear2]
+];
 var timeIntervals = /* @__PURE__ */ new Map([
     ["second", second],
     ["minute", timeMinute],
     ["hour", timeHour],
     ["day", timeDay],
     // TODO local time equivalent of unixDay?
     ["week", timeSunday],
@@ -21702,14 +21724,61 @@
 function isTimeYear(i) {
     if (!i)
         return false;
     const date2 = i.floor(new Date(2e3, 11, 31));
     return timeYear(date2) >= date2;
 }
 
+function formatTimeTicks(scale3, data, ticks2, anchor) {
+    const format3 = scale3.type === "time" ? timeFormat : utcFormat;
+    const template2 = anchor === "left" || anchor === "right" ? (f1, f2) => `
+${f1}
+${f2}` : anchor === "top" ? (f1, f2) => `${f2}
+${f1}` : (f1, f2) => `${f1}
+${f2}`;
+    switch (getTimeTicksInterval(scale3, data, ticks2)) {
+        case "millisecond":
+            return formatConditional(format3(".%L"), format3(":%M:%S"), template2);
+        case "second":
+            return formatConditional(format3(":%S"), format3("%-I:%M"), template2);
+        case "minute":
+            return formatConditional(format3("%-I:%M"), format3("%p"), template2);
+        case "hour":
+            return formatConditional(format3("%-I %p"), format3("%b %-d"), template2);
+        case "day":
+            return formatConditional(format3("%-d"), format3("%b"), template2);
+        case "week":
+            return formatConditional(format3("%-d"), format3("%b"), template2);
+        case "month":
+            return formatConditional(format3("%b"), format3("%Y"), template2);
+        case "year":
+            return format3("%Y");
+    }
+    throw new Error("unable to format time ticks");
+}
+
+function getTimeTicksInterval(scale3, data, ticks2) {
+    const medianStep = median(pairs(data, (a4, b) => Math.abs(b - a4) || NaN));
+    if (medianStep > 0)
+        return formats[bisector(([, step2]) => step2).right(formats, medianStep, 1, formats.length) - 1][0];
+    const [start2, stop] = extent(scale3.domain());
+    const count3 = typeof ticks2 === "number" ? ticks2 : 10;
+    const step = Math.abs(stop - start2) / count3;
+    return formats[bisector(([, step2]) => Math.log(step2)).center(formats, Math.log(step))][0];
+}
+
+function formatConditional(format1, format22, template2) {
+    return (x4, i, X3) => {
+        const f1 = format1(x4, i);
+        const f2 = format22(x4, i);
+        const j = i - orderof(X3);
+        return i !== j && X3[j] !== void 0 && f2 === format22(X3[j], j) ? f1 : template2(f1, f2);
+    };
+}
+
 // node_modules/@observablehq/plot/src/options.js
 var TypedArray = Object.getPrototypeOf(Uint8Array);
 var objectToString = Object.prototype.toString;
 
 function valueof(data, value, type2) {
     const valueType = typeof value;
     return valueType === "string" ? maybeTypedMap(data, field(value), type2) : valueType === "function" ? maybeTypedMap(data, value, type2) : valueType === "number" || value instanceof Date || valueType === "boolean" ? map4(data, constant2(value), type2) : typeof value?.transform === "function" ? maybeTypedArrayify(value.transform(data), type2) : maybeTypedArrayify(value, type2);
@@ -21875,14 +21944,18 @@
     return map4(index3, (i) => values2[i]);
 }
 
 function taker(f) {
     return f.length === 1 ? (index3, values2) => f(take(values2, index3)) : f;
 }
 
+function subarray(I, i, j) {
+    return I.subarray ? I.subarray(i, j) : I.slice(i, j);
+}
+
 function keyof2(value) {
     return value !== null && typeof value === "object" ? value.valueOf() : value;
 }
 
 function maybeInput(key, options) {
     if (options[key] !== void 0)
         return options[key];
@@ -23673,29 +23746,27 @@
     range: range5 = registry.get(key) === radius ? inferRadialRange(channels, domain) : registry.get(key) === length3 ? inferLengthRange(channels, domain) : registry.get(key) === opacity ? unit2 : void 0,
     interpolate = registry.get(key) === color2 ? scheme28 == null && range5 !== void 0 ? rgb_default : quantitativeScheme(scheme28 !== void 0 ? scheme28 : type2 === "cyclical" ? "rainbow" : "turbo") : round2 ? round_default : number_default,
     reverse: reverse3
 }) {
     interval2 = maybeRangeInterval(interval2, type2);
     if (type2 === "cyclical" || type2 === "sequential")
         type2 = "linear";
+    if (typeof interpolate !== "function")
+        interpolate = maybeInterpolator(interpolate);
     reverse3 = !!reverse3;
     if (range5 !== void 0) {
         const n = (domain = arrayify2(domain)).length;
         const m3 = (range5 = arrayify2(range5)).length;
-        if (n > m3) {
-            domain = domain.slice(0, m3);
-            warn(`Warning: the ${key} scale domain contains extra elements.`);
-        } else if (m3 > n) {
-            range5 = range5.slice(0, n);
-            warn(`Warning: the ${key} scale range contains extra elements.`);
+        if (n !== m3) {
+            if (interpolate.length === 1)
+                throw new Error("invalid piecewise interpolator");
+            interpolate = piecewise(interpolate, range5);
+            range5 = void 0;
         }
     }
-    if (typeof interpolate !== "function") {
-        interpolate = maybeInterpolator(interpolate);
-    }
     if (interpolate.length === 1) {
         if (reverse3) {
             interpolate = flip(interpolate);
             reverse3 = false;
         }
         if (range5 === void 0) {
             range5 = Float64Array.from(domain, (_, i) => i / (domain.length - 1));
@@ -25069,23 +25140,26 @@
     mark.imageFilter = impliedString(imageFilter, "none");
     mark.paintOrder = impliedString(paintOrder, "normal");
     mark.pointerEvents = impliedString(pointerEvents, "auto");
     mark.shapeRendering = impliedString(shapeRendering, "auto");
     return {
         title: {
             value: title,
-            optional: true
+            optional: true,
+            filter: null
         },
         href: {
             value: href,
-            optional: true
+            optional: true,
+            filter: null
         },
         ariaLabel: {
             value: variaLabel,
-            optional: true
+            optional: true,
+            filter: null
         },
         fill: {
             value: vfill,
             scale: "auto",
             optional: true
         },
         fillOpacity: {
@@ -25332,15 +25406,18 @@
     applyAttr(selection2, "stroke-linecap", mark.strokeLinecap);
     applyAttr(selection2, "stroke-miterlimit", mark.strokeMiterlimit);
     applyAttr(selection2, "stroke-dasharray", mark.strokeDasharray);
     applyAttr(selection2, "stroke-dashoffset", mark.strokeDashoffset);
     applyAttr(selection2, "shape-rendering", mark.shapeRendering);
     applyAttr(selection2, "filter", mark.imageFilter);
     applyAttr(selection2, "paint-order", mark.paintOrder);
-    applyAttr(selection2, "pointer-events", mark.pointerEvents);
+    const {
+        pointerEvents = context.pointerSticky === false ? "none" : void 0
+    } = mark;
+    applyAttr(selection2, "pointer-events", pointerEvents);
 }
 
 function applyDirectStyles(selection2, mark) {
     applyStyle(selection2, "mix-blend-mode", mark.mixBlendMode);
     applyAttr(selection2, "opacity", mark.opacity);
 }
 
@@ -26071,14 +26148,18 @@
         y: y4,
         channels,
         ...options,
         // Unlike other composed transforms, the render transform must be the
         // outermost render function because it will re-render dynamically in
         // response to pointer events.
         render: composeRender(function(index3, scales, values2, dimensions, context, next) {
+            context = {
+                ...context,
+                pointerSticky: false
+            };
             const svg2 = context.ownerSVGElement;
             const {
                 data
             } = context.getMarkState(this);
             let state = states.get(svg2);
             if (!state)
                 states.set(svg2, state = {
@@ -26114,14 +26195,15 @@
                 px: PX,
                 py: PY
             } = values2;
             const px2 = PX ? (i2) => PX[i2] : anchorX(values2, cx);
             const py2 = PY ? (i2) => PY[i2] : anchorY(values2, cy);
             let i;
             let g;
+            let s2;
             let f;
 
             function update(ii, ri) {
                 if (faceted) {
                     if (f)
                         f = cancelAnimationFrame(f);
                     if (ii == null)
@@ -26141,17 +26223,18 @@
                         return;
                     }
                 }
                 render3(ii);
             }
 
             function render3(ii) {
-                if (i === ii)
+                if (i === ii && s2 === state.sticky)
                     return;
                 i = ii;
+                s2 = context.pointerSticky = state.sticky;
                 const I = i == null ? [] : [i];
                 if (faceted)
                     I.fx = index3.fx, I.fy = index3.fy, I.fi = index3.fi;
                 const r = next(I, scales, values2, dimensions, context);
                 if (g) {
                     if (faceted) {
                         const p = g.parentNode;
@@ -26193,15 +26276,15 @@
                 if (i == null)
                     return;
                 if (state.sticky && state.roots.some((r) => r?.contains(event.target)))
                     return;
                 if (state.sticky)
                     state.sticky = false, state.renders.forEach((r) => r(null));
                 else
-                    state.sticky = true;
+                    state.sticky = true, render3(i);
                 event.stopImmediatePropagation();
             }
 
             function pointerleave(event) {
                 if (event.pointerType !== "mouse")
                     return;
                 if (!state.sticky)
@@ -26245,18 +26328,14 @@
 }
 
 // node_modules/@observablehq/plot/src/axes.js
 function inferFontVariant(scale3) {
     return isOrdinalScale(scale3) && scale3.interval === void 0 ? void 0 : "tabular-nums";
 }
 
-function maybeAutoTickFormat(tickFormat2, domain) {
-    return tickFormat2 === void 0 ? isTemporal(domain) ? formatIsoDate : string : typeof tickFormat2 === "function" ? tickFormat2 : (typeof tickFormat2 === "string" ? isTemporal(domain) ? utcFormat : format : constant2)(tickFormat2);
-}
-
 // node_modules/@observablehq/plot/src/legends/ramp.js
 function legendRamp(color3, options) {
     let {
         label = color3.label,
             tickSize = 6,
             width = 240,
             height = 44 + tickSize,
@@ -26342,263 +26421,14 @@
     ).attr("font-size", null).attr("font-family", null).attr("font-variant", impliedString(fontVariant, "normal")).call(tickAdjust).call((g) => g.select(".domain").remove());
     if (label !== void 0) {
         svg2.append("text").attr("x", marginLeft).attr("y", marginTop - 6).attr("fill", "currentColor").attr("font-weight", "bold").text(label);
     }
     return svg2.node();
 }
 
-// node_modules/@observablehq/plot/src/legends/swatches.js
-function maybeScale(scale3, key) {
-    if (key == null)
-        return key;
-    const s2 = scale3(key);
-    if (!s2)
-        throw new Error(`scale not found: ${key}`);
-    return s2;
-}
-
-function legendSwatches(color3, {
-    opacity: opacity2,
-    ...options
-} = {}) {
-    if (!isOrdinalScale(color3) && !isThresholdScale(color3))
-        throw new Error(`swatches legend requires ordinal or threshold color scale (not ${color3.type})`);
-    return legendItems(
-        color3,
-        options,
-        (selection2, scale3, width, height) => selection2.append("svg").attr("width", width).attr("height", height).attr("fill", scale3.scale).attr("fill-opacity", maybeNumberChannel(opacity2)[1]).append("rect").attr("width", "100%").attr("height", "100%")
-    );
-}
-
-function legendSymbols(symbol2, {
-    fill = symbol2.hint?.fill !== void 0 ? symbol2.hint.fill : "none",
-    fillOpacity = 1,
-    stroke = symbol2.hint?.stroke !== void 0 ? symbol2.hint.stroke : isNoneish(fill) ? "currentColor" : "none",
-    strokeOpacity = 1,
-    strokeWidth = 1.5,
-    r = 4.5,
-    ...options
-} = {}, scale3) {
-    const [vf, cf] = maybeColorChannel(fill);
-    const [vs, cs] = maybeColorChannel(stroke);
-    const sf = maybeScale(scale3, vf);
-    const ss = maybeScale(scale3, vs);
-    const size = r * r * Math.PI;
-    fillOpacity = maybeNumberChannel(fillOpacity)[1];
-    strokeOpacity = maybeNumberChannel(strokeOpacity)[1];
-    strokeWidth = maybeNumberChannel(strokeWidth)[1];
-    return legendItems(
-        symbol2,
-        options,
-        (selection2, scale4, width, height) => selection2.append("svg").attr("viewBox", "-8 -8 16 16").attr("width", width).attr("height", height).attr("fill", vf === "color" ? (d) => sf.scale(d) : cf).attr("fill-opacity", fillOpacity).attr("stroke", vs === "color" ? (d) => ss.scale(d) : cs).attr("stroke-opacity", strokeOpacity).attr("stroke-width", strokeWidth).append("path").attr("d", (d) => {
-            const p = pathRound();
-            symbol2.scale(d).draw(p, size);
-            return p;
-        })
-    );
-}
-
-function legendItems(scale3, options = {}, swatch) {
-    let {
-        columns,
-        tickFormat: tickFormat2,
-        fontVariant = inferFontVariant(scale3),
-        // TODO label,
-        swatchSize = 15,
-        swatchWidth = swatchSize,
-        swatchHeight = swatchSize,
-        marginLeft = 0,
-        className,
-        style,
-        width
-    } = options;
-    const context = createContext(options);
-    className = maybeClassName(className);
-    tickFormat2 = maybeAutoTickFormat(tickFormat2, scale3.domain);
-    const swatches = create2("div", context).attr(
-        "class",
-        `${className}-swatches ${className}-swatches-${columns != null ? "columns" : "wrap"}`
-    );
-    let extraStyle;
-    if (columns != null) {
-        extraStyle = `.${className}-swatches-columns .${className}-swatch {
-  display: flex;
-  align-items: center;
-  break-inside: avoid;
-  padding-bottom: 1px;
-}
-.${className}-swatches-columns .${className}-swatch::before {
-  flex-shrink: 0;
-}
-.${className}-swatches-columns .${className}-swatch-label {
-  white-space: nowrap;
-  overflow: hidden;
-  text-overflow: ellipsis;
-}`;
-        swatches.style("columns", columns).selectAll().data(scale3.domain).enter().append("div").attr("class", `${className}-swatch`).call(swatch, scale3, swatchWidth, swatchHeight).call(
-            (item) => item.append("div").attr("class", `${className}-swatch-label`).attr("title", tickFormat2).text(tickFormat2)
-        );
-    } else {
-        extraStyle = `.${className}-swatches-wrap {
-  display: flex;
-  align-items: center;
-  min-height: 33px;
-  flex-wrap: wrap;
-}
-.${className}-swatches-wrap .${className}-swatch {
-  display: inline-flex;
-  align-items: center;
-  margin-right: 1em;
-}`;
-        swatches.selectAll().data(scale3.domain).enter().append("span").attr("class", `${className}-swatch`).call(swatch, scale3, swatchWidth, swatchHeight).append(function() {
-            return this.ownerDocument.createTextNode(tickFormat2.apply(this, arguments));
-        });
-    }
-    return swatches.call(
-        (div) => div.insert("style", "*").text(
-            `.${className}-swatches {
-  font-family: system-ui, sans-serif;
-  font-size: 10px;
-  margin-bottom: 0.5em;
-}
-.${className}-swatch > svg {
-  margin-right: 0.5em;
-  overflow: visible;
-}
-${extraStyle}`
-        )
-    ).style("margin-left", marginLeft ? `${+marginLeft}px` : null).style("width", width === void 0 ? null : `${+width}px`).style("font-variant", impliedString(fontVariant, "normal")).call(applyInlineStyles, style).node();
-}
-
-// node_modules/@observablehq/plot/src/legends.js
-var legendRegistry = /* @__PURE__ */ new Map([
-    ["symbol", legendSymbols],
-    ["color", legendColor],
-    ["opacity", legendOpacity]
-]);
-
-function legend(options = {}) {
-    for (const [key, value] of legendRegistry) {
-        const scale3 = options[key];
-        if (isScaleOptions(scale3)) {
-            const context = createContext(options);
-            let hint;
-            if (key === "symbol") {
-                const {
-                    fill,
-                    stroke = fill === void 0 && isScaleOptions(options.color) ? "color" : void 0
-                } = options;
-                hint = {
-                    fill,
-                    stroke
-                };
-            }
-            return value(
-                normalizeScale(key, scale3, hint),
-                legendOptions(context, scale3, options),
-                (key2) => isScaleOptions(options[key2]) ? normalizeScale(key2, options[key2]) : null
-            );
-        }
-    }
-    throw new Error("unknown legend type; no scale found");
-}
-
-function exposeLegends(scales, context, defaults22 = {}) {
-    return (key, options) => {
-        if (!legendRegistry.has(key))
-            throw new Error(`unknown legend type: ${key}`);
-        if (!(key in scales))
-            return;
-        return legendRegistry.get(key)(scales[key], legendOptions(context, defaults22[key], options), (key2) => scales[key2]);
-    };
-}
-
-function legendOptions({
-    className,
-    ...context
-}, {
-    label,
-    ticks: ticks2,
-    tickFormat: tickFormat2
-} = {}, options) {
-    return inherit2(options, {
-        className,
-        ...context
-    }, {
-        label,
-        ticks: ticks2,
-        tickFormat: tickFormat2
-    });
-}
-
-function legendColor(color3, {
-    legend: legend2 = true,
-    ...options
-}) {
-    if (legend2 === true)
-        legend2 = color3.type === "ordinal" ? "swatches" : "ramp";
-    if (color3.domain === void 0)
-        return;
-    switch (`${legend2}`.toLowerCase()) {
-        case "swatches":
-            return legendSwatches(color3, options);
-        case "ramp":
-            return legendRamp(color3, options);
-        default:
-            throw new Error(`unknown legend type: ${legend2}`);
-    }
-}
-
-function legendOpacity({
-    type: type2,
-    interpolate,
-    ...scale3
-}, {
-    legend: legend2 = true,
-    color: color3 = rgb(0, 0, 0),
-    ...options
-}) {
-    if (!interpolate)
-        throw new Error(`${type2} opacity scales are not supported`);
-    if (legend2 === true)
-        legend2 = "ramp";
-    if (`${legend2}`.toLowerCase() !== "ramp")
-        throw new Error(`${legend2} opacity legends are not supported`);
-    return legendColor({
-        type: type2,
-        ...scale3,
-        interpolate: interpolateOpacity(color3)
-    }, {
-        legend: legend2,
-        ...options
-    });
-}
-
-function interpolateOpacity(color3) {
-    const {
-        r,
-        g,
-        b
-    } = rgb(color3) || rgb(0, 0, 0);
-    return (t) => `rgba(${r},${g},${b},${t})`;
-}
-
-function createLegends(scales, context, options) {
-    const legends = [];
-    for (const [key, value] of legendRegistry) {
-        const o = options[key];
-        if (o?.legend && key in scales) {
-            const legend2 = value(scales[key], legendOptions(context, scales[key], o), (key2) => scales[key2]);
-            if (legend2 != null)
-                legends.push(legend2);
-        }
-    }
-    return legends;
-}
-
 // node_modules/@observablehq/plot/src/math.js
 var radians3 = Math.PI / 180;
 
 // node_modules/@observablehq/plot/src/marker.js
 function markers(mark, {
     marker,
     markerStart = marker,
@@ -26895,15 +26725,15 @@
             marginLeft,
             marginBottom
         } = dimensions;
         const {
             insetTop,
             insetBottom
         } = this;
-        return create2("svg:g", context).call(applyIndirectStyles, this, dimensions).call(applyTransform, this, {
+        return create2("svg:g", context).call(applyIndirectStyles, this, dimensions, context).call(applyTransform, this, {
             x: X3 && x4
         }, offset, 0).call(
             (g) => g.selectAll().data(index3).enter().append("line").call(applyDirectStyles, this).attr("x1", X3 ? (i) => X3[i] : (marginLeft + width - marginRight) / 2).attr("x2", X3 ? (i) => X3[i] : (marginLeft + width - marginRight) / 2).attr("y1", Y13 && !isCollapsed(y4) ? (i) => Y13[i] + insetTop : marginTop + insetTop).attr(
                 "y2",
                 Y23 && !isCollapsed(y4) ? y4.bandwidth ? (i) => Y23[i] + y4.bandwidth() - insetBottom : (i) => Y23[i] - insetBottom : height - marginBottom - insetBottom
             ).call(applyChannelStyles, this, channels).call(applyMarkers, this, channels, context)
         ).node();
@@ -28109,19 +27939,19 @@
             lineAnchor,
             fontVariant,
             rotate: tickRotate,
             y: y4,
             ...options,
             dx: anchor === "left" ? +dx - tickSize - tickPadding + +insetLeft : +dx + +tickSize + +tickPadding - insetRight
         },
-        function(scale3, ticks2, channels) {
+        function(scale3, data2, ticks2, channels) {
             if (fontVariant === void 0)
                 this.fontVariant = inferFontVariant3(scale3);
             if (text2 === void 0)
-                channels.text = inferTextChannel(scale3, ticks2, tickFormat2);
+                channels.text = inferTextChannel(scale3, data2, ticks2, tickFormat2, anchor);
         }
     );
 }
 
 function axisTextKx(k2, anchor, data, {
     facetAnchor = anchor + (k2 === "x" ? "-empty" : ""),
     frameAnchor = anchor,
@@ -28152,19 +27982,19 @@
             lineAnchor,
             fontVariant,
             rotate: tickRotate,
             x: x4,
             ...options,
             dy: anchor === "bottom" ? +dy + +tickSize + +tickPadding - insetBottom : +dy - tickSize - tickPadding + +insetTop
         },
-        function(scale3, ticks2, channels) {
+        function(scale3, data2, ticks2, channels) {
             if (fontVariant === void 0)
                 this.fontVariant = inferFontVariant3(scale3);
             if (text2 === void 0)
-                channels.text = inferTextChannel(scale3, ticks2, tickFormat2);
+                channels.text = inferTextChannel(scale3, data2, ticks2, tickFormat2, anchor);
         }
     );
 }
 
 function gridY() {
     const [data, options] = maybeData(...arguments);
     return gridKy("y", anchorY2(options), data, options);
@@ -28259,95 +28089,98 @@
         shapeRendering,
         initializer: initializer2
     };
 }
 
 function axisMark(mark, k2, ariaLabel, data, options, initialize) {
     let channels;
-    const m3 = mark(
-        data,
-        initializer(options, function(data2, facets, _channels, scales, dimensions, context) {
-            const initializeFacets = data2 == null && (k2 === "fx" || k2 === "fy");
-            const {
-                [k2]: scale3
-            } = scales;
-            if (!scale3)
-                throw new Error(`missing scale: ${k2}`);
-            let {
-                ticks: ticks2,
-                tickSpacing,
-                interval: interval2
-            } = options;
-            if (isTemporalScale(scale3) && typeof ticks2 === "string")
-                interval2 = ticks2, ticks2 = void 0;
-            if (data2 == null) {
-                if (isIterable(ticks2)) {
-                    data2 = arrayify2(ticks2);
-                } else if (scale3.ticks) {
-                    if (ticks2 !== void 0) {
-                        data2 = scale3.ticks(ticks2);
+
+    function axisInitializer(data2, facets, _channels, scales, dimensions, context) {
+        const initializeFacets = data2 == null && (k2 === "fx" || k2 === "fy");
+        const {
+            [k2]: scale3
+        } = scales;
+        if (!scale3)
+            throw new Error(`missing scale: ${k2}`);
+        let {
+            ticks: ticks2,
+            tickSpacing,
+            interval: interval2
+        } = options;
+        if (isTemporalScale(scale3) && typeof ticks2 === "string")
+            interval2 = ticks2, ticks2 = void 0;
+        if (data2 == null) {
+            if (isIterable(ticks2)) {
+                data2 = arrayify2(ticks2);
+            } else if (scale3.ticks) {
+                if (ticks2 !== void 0) {
+                    data2 = scale3.ticks(ticks2);
+                } else {
+                    interval2 = maybeRangeInterval(interval2 === void 0 ? scale3.interval : interval2, scale3.type);
+                    if (interval2 !== void 0) {
+                        const [min4, max5] = extent(scale3.domain());
+                        data2 = interval2.range(min4, interval2.offset(interval2.floor(max5)));
                     } else {
-                        interval2 = maybeRangeInterval(interval2 === void 0 ? scale3.interval : interval2, scale3.type);
-                        if (interval2 !== void 0) {
-                            const [min4, max5] = extent(scale3.domain());
-                            data2 = interval2.range(min4, interval2.offset(interval2.floor(max5)));
-                        } else {
-                            const [min4, max5] = extent(scale3.range());
-                            ticks2 = (max5 - min4) / (tickSpacing === void 0 ? k2 === "x" ? 80 : 35 : tickSpacing);
-                            data2 = scale3.ticks(ticks2);
-                        }
+                        const [min4, max5] = extent(scale3.range());
+                        ticks2 = (max5 - min4) / (tickSpacing === void 0 ? k2 === "x" ? 80 : 35 : tickSpacing);
+                        data2 = scale3.ticks(ticks2);
                     }
-                } else {
-                    data2 = scale3.domain();
-                }
-                if (k2 === "y" || k2 === "x") {
-                    facets = [range4(data2)];
-                } else {
-                    channels[k2] = {
-                        scale: k2,
-                        value: identity6
-                    };
                 }
+            } else {
+                data2 = scale3.domain();
             }
-            initialize?.call(this, scale3, ticks2, channels);
-            const initializedChannels = Object.fromEntries(
-                Object.entries(channels).map(([name, channel]) => {
-                    return [name, {
-                        ...channel,
-                        value: valueof(data2, channel.value)
-                    }];
-                })
-            );
-            if (initializeFacets)
-                facets = context.filterFacets(data2, initializedChannels);
-            return {
-                data: data2,
-                facets,
-                channels: initializedChannels
-            };
-        })
-    );
+            if (k2 === "y" || k2 === "x") {
+                facets = [range4(data2)];
+            } else {
+                channels[k2] = {
+                    scale: k2,
+                    value: identity6
+                };
+            }
+        }
+        initialize?.call(this, scale3, data2, ticks2, channels);
+        const initializedChannels = Object.fromEntries(
+            Object.entries(channels).map(([name, channel]) => {
+                return [name, {
+                    ...channel,
+                    value: valueof(data2, channel.value)
+                }];
+            })
+        );
+        if (initializeFacets)
+            facets = context.filterFacets(data2, initializedChannels);
+        return {
+            data: data2,
+            facets,
+            channels: initializedChannels
+        };
+    }
+    const basicInitializer = initializer(options).initializer;
+    const m3 = mark(data, initializer({
+        ...options,
+        initializer: axisInitializer
+    }, basicInitializer));
     if (data == null) {
         channels = m3.channels;
         m3.channels = {};
     } else {
         channels = {};
     }
     m3.ariaLabel = ariaLabel;
     return m3;
 }
 
-function inferTextChannel(scale3, ticks2, tickFormat2) {
+function inferTextChannel(scale3, data, ticks2, tickFormat2, anchor) {
     return {
-        value: inferTickFormat(scale3, ticks2, tickFormat2)
+        value: inferTickFormat(scale3, data, ticks2, tickFormat2, anchor)
     };
 }
 
-function inferTickFormat(scale3, ticks2, tickFormat2) {
-    return scale3.tickFormat ? scale3.tickFormat(isIterable(ticks2) ? null : ticks2, tickFormat2) : tickFormat2 === void 0 ? isUtcYear(scale3.interval) ? utcFormat("%Y") : isTimeYear(scale3.interval) ? timeFormat("%Y") : formatDefault : typeof tickFormat2 === "string" ? (isTemporal(scale3.domain()) ? utcFormat : format)(tickFormat2) : constant2(tickFormat2);
+function inferTickFormat(scale3, data, ticks2, tickFormat2, anchor) {
+    return tickFormat2 === void 0 && isTemporalScale(scale3) ? formatTimeTicks(scale3, data, ticks2, anchor) : scale3.tickFormat ? scale3.tickFormat(isIterable(ticks2) ? null : ticks2, tickFormat2) : tickFormat2 === void 0 ? isUtcYear(scale3.interval) ? utcFormat("%Y") : isTimeYear(scale3.interval) ? timeFormat("%Y") : formatDefault : typeof tickFormat2 === "string" ? (isTemporal(scale3.domain()) ? utcFormat : format)(tickFormat2) : constant2(tickFormat2);
 }
 var shapeTickBottom = {
     draw(context, l) {
         context.moveTo(0, 0);
         context.lineTo(0, l);
     }
 };
@@ -28413,14 +28246,264 @@
     return isNoneish(labelArrow) ? false : typeof labelArrow === "boolean" ? labelArrow : keyword(labelArrow, "labelArrow", ["auto", "up", "right", "down", "left"]);
 }
 
 function isTemporalish(scale3) {
     return isTemporalScale(scale3) || scale3.interval != null;
 }
 
+// node_modules/@observablehq/plot/src/legends/swatches.js
+function maybeScale(scale3, key) {
+    if (key == null)
+        return key;
+    const s2 = scale3(key);
+    if (!s2)
+        throw new Error(`scale not found: ${key}`);
+    return s2;
+}
+
+function legendSwatches(color3, {
+    opacity: opacity2,
+    ...options
+} = {}) {
+    if (!isOrdinalScale(color3) && !isThresholdScale(color3))
+        throw new Error(`swatches legend requires ordinal or threshold color scale (not ${color3.type})`);
+    return legendItems(
+        color3,
+        options,
+        (selection2, scale3, width, height) => selection2.append("svg").attr("width", width).attr("height", height).attr("fill", scale3.scale).attr("fill-opacity", maybeNumberChannel(opacity2)[1]).append("rect").attr("width", "100%").attr("height", "100%")
+    );
+}
+
+function legendSymbols(symbol2, {
+    fill = symbol2.hint?.fill !== void 0 ? symbol2.hint.fill : "none",
+    fillOpacity = 1,
+    stroke = symbol2.hint?.stroke !== void 0 ? symbol2.hint.stroke : isNoneish(fill) ? "currentColor" : "none",
+    strokeOpacity = 1,
+    strokeWidth = 1.5,
+    r = 4.5,
+    ...options
+} = {}, scale3) {
+    const [vf, cf] = maybeColorChannel(fill);
+    const [vs, cs] = maybeColorChannel(stroke);
+    const sf = maybeScale(scale3, vf);
+    const ss = maybeScale(scale3, vs);
+    const size = r * r * Math.PI;
+    fillOpacity = maybeNumberChannel(fillOpacity)[1];
+    strokeOpacity = maybeNumberChannel(strokeOpacity)[1];
+    strokeWidth = maybeNumberChannel(strokeWidth)[1];
+    return legendItems(
+        symbol2,
+        options,
+        (selection2, scale4, width, height) => selection2.append("svg").attr("viewBox", "-8 -8 16 16").attr("width", width).attr("height", height).attr("fill", vf === "color" ? (d) => sf.scale(d) : cf).attr("fill-opacity", fillOpacity).attr("stroke", vs === "color" ? (d) => ss.scale(d) : cs).attr("stroke-opacity", strokeOpacity).attr("stroke-width", strokeWidth).append("path").attr("d", (d) => {
+            const p = pathRound();
+            symbol2.scale(d).draw(p, size);
+            return p;
+        })
+    );
+}
+
+function legendItems(scale3, options = {}, swatch) {
+    let {
+        columns,
+        tickFormat: tickFormat2,
+        fontVariant = inferFontVariant(scale3),
+        // TODO label,
+        swatchSize = 15,
+        swatchWidth = swatchSize,
+        swatchHeight = swatchSize,
+        marginLeft = 0,
+        className,
+        style,
+        width
+    } = options;
+    const context = createContext(options);
+    className = maybeClassName(className);
+    if (typeof tickFormat2 !== "function")
+        tickFormat2 = inferTickFormat(scale3.scale, scale3.domain, void 0, tickFormat2);
+    const swatches = create2("div", context).attr(
+        "class",
+        `${className}-swatches ${className}-swatches-${columns != null ? "columns" : "wrap"}`
+    );
+    let extraStyle;
+    if (columns != null) {
+        extraStyle = `.${className}-swatches-columns .${className}-swatch {
+  display: flex;
+  align-items: center;
+  break-inside: avoid;
+  padding-bottom: 1px;
+}
+.${className}-swatches-columns .${className}-swatch::before {
+  flex-shrink: 0;
+}
+.${className}-swatches-columns .${className}-swatch-label {
+  white-space: nowrap;
+  overflow: hidden;
+  text-overflow: ellipsis;
+}`;
+        swatches.style("columns", columns).selectAll().data(scale3.domain).enter().append("div").attr("class", `${className}-swatch`).call(swatch, scale3, swatchWidth, swatchHeight).call(
+            (item) => item.append("div").attr("class", `${className}-swatch-label`).attr("title", tickFormat2).text(tickFormat2)
+        );
+    } else {
+        extraStyle = `.${className}-swatches-wrap {
+  display: flex;
+  align-items: center;
+  min-height: 33px;
+  flex-wrap: wrap;
+}
+.${className}-swatches-wrap .${className}-swatch {
+  display: inline-flex;
+  align-items: center;
+  margin-right: 1em;
+}`;
+        swatches.selectAll().data(scale3.domain).enter().append("span").attr("class", `${className}-swatch`).call(swatch, scale3, swatchWidth, swatchHeight).append(function() {
+            return this.ownerDocument.createTextNode(tickFormat2.apply(this, arguments));
+        });
+    }
+    return swatches.call(
+        (div) => div.insert("style", "*").text(
+            `.${className}-swatches {
+  font-family: system-ui, sans-serif;
+  font-size: 10px;
+  margin-bottom: 0.5em;
+}
+.${className}-swatch > svg {
+  margin-right: 0.5em;
+  overflow: visible;
+}
+${extraStyle}`
+        )
+    ).style("margin-left", marginLeft ? `${+marginLeft}px` : null).style("width", width === void 0 ? null : `${+width}px`).style("font-variant", impliedString(fontVariant, "normal")).call(applyInlineStyles, style).node();
+}
+
+// node_modules/@observablehq/plot/src/legends.js
+var legendRegistry = /* @__PURE__ */ new Map([
+    ["symbol", legendSymbols],
+    ["color", legendColor],
+    ["opacity", legendOpacity]
+]);
+
+function legend(options = {}) {
+    for (const [key, value] of legendRegistry) {
+        const scale3 = options[key];
+        if (isScaleOptions(scale3)) {
+            const context = createContext(options);
+            let hint;
+            if (key === "symbol") {
+                const {
+                    fill,
+                    stroke = fill === void 0 && isScaleOptions(options.color) ? "color" : void 0
+                } = options;
+                hint = {
+                    fill,
+                    stroke
+                };
+            }
+            return value(
+                normalizeScale(key, scale3, hint),
+                legendOptions(context, scale3, options),
+                (key2) => isScaleOptions(options[key2]) ? normalizeScale(key2, options[key2]) : null
+            );
+        }
+    }
+    throw new Error("unknown legend type; no scale found");
+}
+
+function exposeLegends(scales, context, defaults22 = {}) {
+    return (key, options) => {
+        if (!legendRegistry.has(key))
+            throw new Error(`unknown legend type: ${key}`);
+        if (!(key in scales))
+            return;
+        return legendRegistry.get(key)(scales[key], legendOptions(context, defaults22[key], options), (key2) => scales[key2]);
+    };
+}
+
+function legendOptions({
+    className,
+    ...context
+}, {
+    label,
+    ticks: ticks2,
+    tickFormat: tickFormat2
+} = {}, options) {
+    return inherit2(options, {
+        className,
+        ...context
+    }, {
+        label,
+        ticks: ticks2,
+        tickFormat: tickFormat2
+    });
+}
+
+function legendColor(color3, {
+    legend: legend2 = true,
+    ...options
+}) {
+    if (legend2 === true)
+        legend2 = color3.type === "ordinal" ? "swatches" : "ramp";
+    if (color3.domain === void 0)
+        return;
+    switch (`${legend2}`.toLowerCase()) {
+        case "swatches":
+            return legendSwatches(color3, options);
+        case "ramp":
+            return legendRamp(color3, options);
+        default:
+            throw new Error(`unknown legend type: ${legend2}`);
+    }
+}
+
+function legendOpacity({
+    type: type2,
+    interpolate,
+    ...scale3
+}, {
+    legend: legend2 = true,
+    color: color3 = rgb(0, 0, 0),
+    ...options
+}) {
+    if (!interpolate)
+        throw new Error(`${type2} opacity scales are not supported`);
+    if (legend2 === true)
+        legend2 = "ramp";
+    if (`${legend2}`.toLowerCase() !== "ramp")
+        throw new Error(`${legend2} opacity legends are not supported`);
+    return legendColor({
+        type: type2,
+        ...scale3,
+        interpolate: interpolateOpacity(color3)
+    }, {
+        legend: legend2,
+        ...options
+    });
+}
+
+function interpolateOpacity(color3) {
+    const {
+        r,
+        g,
+        b
+    } = rgb(color3) || rgb(0, 0, 0);
+    return (t) => `rgba(${r},${g},${b},${t})`;
+}
+
+function createLegends(scales, context, options) {
+    const legends = [];
+    for (const [key, value] of legendRegistry) {
+        const o = options[key];
+        if (o?.legend && key in scales) {
+            const legend2 = value(scales[key], legendOptions(context, scales[key], o), (key2) => scales[key2]);
+            if (legend2 != null)
+                legends.push(legend2);
+        }
+    }
+    return legends;
+}
+
 // node_modules/@observablehq/plot/src/marks/frame.js
 var defaults4 = {
     ariaLabel: "frame",
     fill: "none",
     stroke: "currentColor"
 };
 var lineDefaults = {
@@ -28517,14 +28600,15 @@
             fontWeight,
             lineHeight = 1,
             lineWidth = 20,
             frameAnchor,
             textAnchor = "start",
             textOverflow,
             textPadding = 8,
+            title,
             pointerSize = 12,
             pathFilter = "drop-shadow(0 3px 4px rgba(0,0,0,0.2))"
         } = options;
         super(
             data, {
                 x: {
                     value: x12 != null && x22 != null ? null : x4,
@@ -28553,15 +28637,20 @@
                     scale: "x",
                     optional: x12 == null
                 },
                 y2: {
                     value: y22,
                     scale: "y",
                     optional: y12 == null
+                },
+                title: {
+                    value: title,
+                    optional: true
                 }
+                // filter: defined
             },
             options,
             defaults5
         );
         this.anchor = maybeAnchor(anchor, "anchor");
         this.previousAnchor = this.anchor ?? "top-left";
         this.frameAnchor = maybeFrameAnchor(frameAnchor);
@@ -29102,16 +29191,17 @@
                 let index3 = null;
                 if (indexes2) {
                     const faceted = facetStateByMark.has(mark);
                     index3 = indexes2[faceted ? f.i : 0];
                     index3 = mark.filter(index3, channels, values2);
                     if (index3.length === 0)
                         continue;
-                    if (faceted)
-                        index3.fx = f.x, index3.fy = f.y, index3.fi = f.i;
+                    if (!faceted && index3 === indexes2[0])
+                        index3 = subarray(index3);
+                    index3.fx = f.x, index3.fy = f.y, index3.fi = f.i;
                 }
                 const node = mark.render(index3, scales, values2, subdimensions, context);
                 if (node == null)
                     continue;
                 (g ??= select_default2(svg2).append("g")).append(() => node).datum(f);
                 for (const name of ["aria-label", "aria-description", "aria-hidden", "transform"]) {
                     if (node.hasAttribute(name)) {
@@ -31857,15 +31947,15 @@
                 Z = null;
             break;
         case "rule":
             markImpl = X3 ? ruleX : ruleY;
             colorMode = "stroke";
             break;
         case "bar":
-            markImpl = yZero ? isOrdinalReduced(xReduce, X3) ? barY : rectY : xZero ? isOrdinalReduced(yReduce, Y3) ? barX : rectX : isOrdinalReduced(xReduce, X3) && isOrdinalReduced(yReduce, Y3) ? cell : isOrdinalReduced(xReduce, X3) ? barY : isOrdinalReduced(yReduce, Y3) ? barX : xReduce != null ? rectX : yReduce != null ? rectY : rect;
+            markImpl = yZero ? isOrdinalReduced(xReduce, X3) ? barY : rectY : xZero ? isOrdinalReduced(yReduce, Y3) ? barX : rectX : isOrdinalReduced(xReduce, X3) && isOrdinalReduced(yReduce, Y3) ? cell : isOrdinalReduced(xReduce, X3) ? barY : isOrdinalReduced(yReduce, Y3) ? barX : xReduce != null ? rectX : yReduce != null ? rectY : colorReduce != null ? rect : cell;
             colorMode = "fill";
             break;
         default:
             throw new Error(`invalid mark: ${mark}`);
     }
     let markOptions2 = {
         fx,
@@ -32941,57 +33031,46 @@
     return W;
 }
 
 function interpolatorBarycentric({
     random = lcg(42)
 } = {}) {
     return (index3, width, height, X3, Y3, V) => {
-        const n = index3.length;
-        const nw = width >> 2;
-        const nh = (height >> 2) - 1;
-        const m3 = n + nw * 2 + nh * 2;
-        const XY2 = new Float64Array(m3 * 2);
-        for (let i2 = 0; i2 < n; ++i2)
-            XY2[i2 * 2] = X3[index3[i2]], XY2[i2 * 2 + 1] = Y3[index3[i2]];
-        let i = n;
-        const addPoint = (x4, y4) => (XY2[i * 2] = x4, XY2[i * 2 + 1] = y4, i++);
-        for (let j = 0; j <= nw; ++j)
-            addPoint(j / nw * width, 0), addPoint(j / nw * width, height);
-        for (let j = 0; j < nh; ++j)
-            addPoint(width, j / nh * height), addPoint(0, j / nh * height);
-        V = take(V, index3);
-        const delaunay = new Delaunay(XY2.subarray(0, n * 2));
-        for (let j = n, ij; j < m3; ++j)
-            V[j] = V[ij = delaunay.find(XY2[j * 2], XY2[j * 2 + 1], ij)];
         const {
             points,
-            triangles
-        } = new Delaunay(XY2);
-        const W = new V.constructor(width * height);
+            triangles,
+            hull: hull2
+        } = Delaunay.from(
+            index3,
+            (i) => X3[i],
+            (i) => Y3[i]
+        );
+        const W = new V.constructor(width * height).fill(NaN);
+        const S = new Uint8Array(width * height);
         const mix = mixer(V, random);
-        for (let i2 = 0; i2 < triangles.length; i2 += 3) {
-            const ta = triangles[i2];
-            const tb = triangles[i2 + 1];
-            const tc = triangles[i2 + 2];
+        for (let i = 0; i < triangles.length; i += 3) {
+            const ta = triangles[i];
+            const tb = triangles[i + 1];
+            const tc = triangles[i + 2];
             const Ax = points[2 * ta];
             const Bx = points[2 * tb];
             const Cx = points[2 * tc];
             const Ay = points[2 * ta + 1];
             const By = points[2 * tb + 1];
             const Cy = points[2 * tc + 1];
             const x12 = Math.min(Ax, Bx, Cx);
             const x22 = Math.max(Ax, Bx, Cx);
             const y12 = Math.min(Ay, By, Cy);
             const y22 = Math.max(Ay, By, Cy);
             const z = (By - Cy) * (Ax - Cx) + (Ay - Cy) * (Cx - Bx);
             if (!z)
                 continue;
-            const va = V[ta];
-            const vb = V[tb];
-            const vc = V[tc];
+            const va = V[index3[ta]];
+            const vb = V[index3[tb]];
+            const vc = V[index3[tc]];
             for (let x4 = Math.floor(x12); x4 < x22; ++x4) {
                 for (let y4 = Math.floor(y12); y4 < y22; ++y4) {
                     if (x4 < 0 || x4 >= width || y4 < 0 || y4 >= height)
                         continue;
                     const xp = x4 + 0.5;
                     const yp = y4 + 0.5;
                     const ga = ((By - Cy) * (xp - Cx) + (yp - Cy) * (Cx - Bx)) / z;
@@ -32999,22 +33078,94 @@
                         continue;
                     const gb = ((Cy - Ay) * (xp - Cx) + (yp - Cy) * (Ax - Cx)) / z;
                     if (gb < 0)
                         continue;
                     const gc = 1 - ga - gb;
                     if (gc < 0)
                         continue;
-                    W[x4 + width * y4] = mix(va, ga, vb, gb, vc, gc, x4, y4);
+                    const i2 = x4 + width * y4;
+                    W[i2] = mix(va, ga, vb, gb, vc, gc, x4, y4);
+                    S[i2] = 1;
                 }
             }
         }
+        extrapolateBarycentric(W, S, X3, Y3, V, width, height, hull2, index3, mix);
         return W;
     };
 }
 
+function extrapolateBarycentric(W, S, X3, Y3, V, width, height, hull2, index3, mix) {
+    X3 = Float64Array.from(hull2, (i) => X3[index3[i]]);
+    Y3 = Float64Array.from(hull2, (i) => Y3[index3[i]]);
+    V = Array.from(hull2, (i) => V[index3[i]]);
+    const n = X3.length;
+    const rays = Array.from({
+        length: n
+    }, (_, j) => ray(j, X3, Y3));
+    let k2 = 0;
+    for (let y4 = 0; y4 < height; ++y4) {
+        const yp = y4 + 0.5;
+        for (let x4 = 0; x4 < width; ++x4) {
+            const i = x4 + width * y4;
+            if (!S[i]) {
+                const xp = x4 + 0.5;
+                for (let l = 0; l < n; ++l) {
+                    const j = (n + k2 + (l % 2 ? (l + 1) / 2 : -l / 2)) % n;
+                    if (rays[j](xp, yp)) {
+                        const t = segmentProject(X3.at(j - 1), Y3.at(j - 1), X3[j], Y3[j], xp, yp);
+                        W[i] = mix(V.at(j - 1), t, V[j], 1 - t, V[j], 0, x4, y4);
+                        k2 = j;
+                        break;
+                    }
+                }
+            }
+        }
+    }
+}
+
+function segmentProject(x12, y12, x22, y22, x4, y4) {
+    const dx = x22 - x12;
+    const dy = y22 - y12;
+    const a4 = dx * (x22 - x4) + dy * (y22 - y4);
+    const b = dx * (x4 - x12) + dy * (y4 - y12);
+    return a4 > 0 && b > 0 ? a4 / (a4 + b) : +(a4 > b);
+}
+
+function cross2(xa, ya, xb, yb) {
+    return xa * yb - xb * ya;
+}
+
+function ray(j, X3, Y3) {
+    const n = X3.length;
+    const xc = X3.at(j - 2);
+    const yc = Y3.at(j - 2);
+    const xa = X3.at(j - 1);
+    const ya = Y3.at(j - 1);
+    const xb = X3[j];
+    const yb = Y3[j];
+    const xd = X3.at(j + 1 - n);
+    const yd = Y3.at(j + 1 - n);
+    const dxab = xa - xb;
+    const dyab = ya - yb;
+    const dxca = xc - xa;
+    const dyca = yc - ya;
+    const dxbd = xb - xd;
+    const dybd = yb - yd;
+    const hab = Math.hypot(dxab, dyab);
+    const hca = Math.hypot(dxca, dyca);
+    const hbd = Math.hypot(dxbd, dybd);
+    return (x4, y4) => {
+        const dxa = x4 - xa;
+        const dya = y4 - ya;
+        const dxb = x4 - xb;
+        const dyb = y4 - yb;
+        return cross2(dxa, dya, dxb, dyb) > -1e-6 && cross2(dxa, dya, dxab, dyab) * hca - cross2(dxa, dya, dxca, dyca) * hab > -1e-6 && cross2(dxb, dyb, dxbd, dybd) * hab - cross2(dxb, dyb, dxab, dyab) * hbd <= 0;
+    };
+}
+
 function interpolateNearest(index3, width, height, X3, Y3, V) {
     const W = new V.constructor(width * height);
     const delaunay = Delaunay.from(
         index3,
         (i) => X3[i],
         (i) => Y3[i]
     );
@@ -34816,18 +34967,21 @@
     delimiter,
     // how the path is separated
     frameAnchor,
     treeLayout = tree_default,
     treeSort,
     treeSeparation,
     treeAnchor,
+    treeFilter,
     ...options
 } = {}) {
     treeAnchor = maybeTreeAnchor(treeAnchor);
     treeSort = maybeTreeSort(treeSort);
+    if (treeFilter != null)
+        treeFilter = maybeNodeValue(treeFilter);
     if (frameAnchor === void 0)
         frameAnchor = treeAnchor.frameAnchor;
     const normalize4 = normalizer(delimiter);
     const outputs = treeOutputs(options, maybeNodeValue);
     const [X3, setX] = column();
     const [Y3, setY] = column();
     return {
@@ -34852,14 +35006,16 @@
             for (const facet of facets) {
                 const treeFacet = [];
                 const root3 = rootof(facet.filter((i) => P[i] != null)).each((node) => node.data = data[node.data]);
                 if (treeSort != null)
                     root3.sort(treeSort);
                 layout(root3);
                 for (const node of root3.descendants()) {
+                    if (treeFilter != null && !treeFilter(node))
+                        continue;
                     treeFacet.push(++treeIndex);
                     treeData[treeIndex] = node.data;
                     treeAnchor.position(node, treeIndex, X4, Y4);
                     for (const o of outputs)
                         o[output_values][treeIndex] = o[output_evaluate](node);
                 }
                 treeFacets.push(treeFacet);
@@ -34882,18 +35038,21 @@
     stroke = "#555",
     strokeWidth = 1.5,
     strokeOpacity = 0.5,
     treeLayout = tree_default,
     treeSort,
     treeSeparation,
     treeAnchor,
+    treeFilter,
     ...options
 } = {}) {
     treeAnchor = maybeTreeAnchor(treeAnchor);
     treeSort = maybeTreeSort(treeSort);
+    if (treeFilter != null)
+        treeFilter = maybeLinkValue(treeFilter);
     options = {
         curve,
         stroke,
         strokeWidth,
         strokeOpacity,
         ...options
     };
@@ -34932,14 +35091,16 @@
                     root3.sort(treeSort);
                 layout(root3);
                 for (const {
                         source,
                         target
                     }
                     of root3.links()) {
+                    if (treeFilter != null && !treeFilter(target, source))
+                        continue;
                     treeFacet.push(++treeIndex);
                     treeData[treeIndex] = target.data;
                     treeAnchor.position(source, treeIndex, X14, Y14);
                     treeAnchor.position(target, treeIndex, X24, Y24);
                     for (const o of outputs)
                         o[output_values][treeIndex] = o[output_evaluate](target, source);
                 }
@@ -35028,14 +35189,16 @@
     switch (value) {
         case "node:name":
             return nodeName;
         case "node:path":
             return nodePath;
         case "node:internal":
             return nodeInternal;
+        case "node:external":
+            return nodeExternal;
         case "node:depth":
             return nodeDepth;
         case "node:height":
             return nodeHeight;
     }
     throw new Error(`invalid node value: ${value}`);
 }
@@ -35059,14 +35222,16 @@
             return parentValue(nodeHeight);
         case "node:name":
             return nodeName;
         case "node:path":
             return nodePath;
         case "node:internal":
             return nodeInternal;
+        case "node:external":
+            return nodeExternal;
         case "node:depth":
             return nodeDepth;
         case "node:height":
             return nodeHeight;
     }
     throw new Error(`invalid link value: ${value}`);
 }
@@ -35087,14 +35252,18 @@
     return node.height;
 }
 
 function nodeInternal(node) {
     return !!node.children;
 }
 
+function nodeExternal(node) {
+    return !node.children;
+}
+
 function parentValue(evaluate) {
     return (child, parent) => parent == null ? void 0 : evaluate(parent);
 }
 
 function nameof(path2) {
     let i = path2.length;
     while (--i > 0)
@@ -35145,52 +35314,78 @@
     markerEnd = marker,
     dot: dotDot = isNoneish(markerStart) && isNoneish(markerEnd),
     text: textText = "node:name",
     textStroke = "white",
     title = "node:path",
     dx,
     dy,
+    textAnchor,
+    treeLayout = tree_default,
+    textLayout = treeLayout === tree_default || treeLayout === cluster_default ? "mirrored" : "normal",
+    tip: tip2,
     ...options
 } = {}) {
     if (dx === void 0)
         dx = maybeTreeAnchor(options.treeAnchor).dx;
+    if (textAnchor !== void 0)
+        throw new Error("textAnchor is not a configurable tree option");
+    textLayout = keyword(textLayout, "textLayout", ["mirrored", "normal"]);
+
+    function treeText(textOptions2) {
+        return text(
+            data,
+            treeNode({
+                treeLayout,
+                text: textText,
+                fill: fill === void 0 ? "currentColor" : fill,
+                stroke: textStroke,
+                dx,
+                dy,
+                title,
+                ...textOptions2,
+                ...options
+            })
+        );
+    }
     return marks(
         link3(
             data,
             treeLink({
+                treeLayout,
                 markerStart,
                 markerEnd,
                 stroke: stroke !== void 0 ? stroke : fill === void 0 ? "node:internal" : fill,
                 strokeWidth,
                 strokeOpacity,
                 strokeLinejoin,
                 strokeLinecap,
                 strokeMiterlimit,
                 strokeDasharray,
                 strokeDashoffset,
                 ...options
             })
         ),
         dotDot ? dot(data, treeNode({
+            treeLayout,
             fill: fill === void 0 ? "node:internal" : fill,
             title,
+            tip: tip2,
             ...options
         })) : null,
-        textText != null ? text(
-            data,
-            treeNode({
-                text: textText,
-                fill: fill === void 0 ? "currentColor" : fill,
-                stroke: textStroke,
-                dx,
-                dy,
-                title,
-                ...options
+        textText != null ? textLayout === "mirrored" ? [
+            treeText({
+                textAnchor: "start",
+                treeFilter: "node:external"
+            }),
+            treeText({
+                textAnchor: "end",
+                treeFilter: "node:internal",
+                dx: -dx
             })
-        ) : null
+        ] : treeText() : null
     );
 }
 
 function cluster(data, options) {
     return tree(data, {
         ...options,
         treeLayout: cluster_default
@@ -35646,67 +35841,63 @@
         }
     }
     if (typeof reduce2 !== "function")
         throw new Error(`invalid reduce: ${reduce2}`);
     return reduceArray(taker(reduce2));
 }
 
-function slice6(I, i, j) {
-    return I.subarray ? I.subarray(i, j) : I.slice(i, j);
-}
-
 function reduceAccessor2(f) {
     return (k2, s2, strict) => strict ? {
         mapIndex(I, S, T) {
-            const s3 = (i) => S[i] == null ? NaN : +S[i];
+            const v2 = (i) => S[i] == null ? NaN : +S[i];
             let nans = 0;
             for (let i = 0; i < k2 - 1; ++i)
-                if (isNaN(s3(i)))
+                if (isNaN(v2(i)))
                     ++nans;
             for (let i = 0, n = I.length - k2 + 1; i < n; ++i) {
-                if (isNaN(s3(i + k2 - 1)))
+                if (isNaN(v2(i + k2 - 1)))
                     ++nans;
-                T[I[i + s3]] = nans === 0 ? f(slice6(I, i, i + k2), s3) : NaN;
-                if (isNaN(s3(i)))
+                T[I[i + s2]] = nans === 0 ? f(subarray(I, i, i + k2), v2) : NaN;
+                if (isNaN(v2(i)))
                     --nans;
             }
         }
     } : {
         mapIndex(I, S, T) {
-            const s3 = (i) => S[i] == null ? NaN : +S[i];
-            for (let i = -s3; i < 0; ++i) {
-                T[I[i + s3]] = f(slice6(I, 0, i + k2), s3);
+            const v2 = (i) => S[i] == null ? NaN : +S[i];
+            for (let i = -s2; i < 0; ++i) {
+                T[I[i + s2]] = f(subarray(I, 0, i + k2), v2);
             }
-            for (let i = 0, n = I.length - s3; i < n; ++i) {
-                T[I[i + s3]] = f(slice6(I, i, i + k2), s3);
+            for (let i = 0, n = I.length - s2; i < n; ++i) {
+                T[I[i + s2]] = f(subarray(I, i, i + k2), v2);
             }
         }
     };
 }
 
 function reduceArray(f) {
     return (k2, s2, strict) => strict ? {
         mapIndex(I, S, T) {
             let count3 = 0;
             for (let i = 0; i < k2 - 1; ++i)
                 count3 += defined(S[I[i]]);
             for (let i = 0, n = I.length - k2 + 1; i < n; ++i) {
                 count3 += defined(S[I[i + k2 - 1]]);
                 if (count3 === k2)
-                    T[I[i + s2]] = f(slice6(I, i, i + k2), S);
+                    T[I[i + s2]] = f(subarray(I, i, i + k2), S);
                 count3 -= defined(S[I[i]]);
             }
         }
     } : {
         mapIndex(I, S, T) {
             for (let i = -s2; i < 0; ++i) {
-                T[I[i + s2]] = f(slice6(I, 0, i + k2), S);
+                T[I[i + s2]] = f(subarray(I, 0, i + k2), S);
             }
             for (let i = 0, n = I.length - s2; i < n; ++i) {
-                T[I[i + s2]] = f(slice6(I, i, i + k2), S);
+                T[I[i + s2]] = f(subarray(I, i, i + k2), S);
             }
         }
     };
 }
 
 function reduceSum2(k2, s2, strict) {
     return strict ? {
@@ -35985,15 +36176,15 @@
         return {
             data,
             facets: selectFacets
         };
     });
 }
 
-// node_modules/tslib/tslib.es6.js
+// node_modules/tslib/tslib.es6.mjs
 function __rest(s2, e) {
     var t = {};
     for (var p in s2)
         if (Object.prototype.hasOwnProperty.call(s2, p) && e.indexOf(p) < 0)
             t[p] = s2[p];
     if (s2 != null && typeof Object.getOwnPropertySymbols === "function")
         for (var i = 0, p = Object.getOwnPropertySymbols(s2); i < p.length; i++) {
@@ -38654,16 +38845,16 @@
         stride,
         children: children2
     } = data;
     const {
         [index3 * stride]: begin, [index3 * stride + 1]: end
     } = valueOffsets;
     const child = children2[0];
-    const slice7 = child.slice(begin, end - begin);
-    return new Vector2([slice7]);
+    const slice6 = child.slice(begin, end - begin);
+    return new Vector2([slice6]);
 };
 var getMap = (data, index3) => {
     const {
         valueOffsets,
         children: children2
     } = data;
     const {
@@ -38707,16 +38898,16 @@
 };
 var getFixedSizeList = (data, index3) => {
     const {
         stride,
         children: children2
     } = data;
     const child = children2[0];
-    const slice7 = child.slice(index3 * stride, stride);
-    return new Vector2([slice7]);
+    const slice6 = child.slice(index3 * stride, stride);
+    return new Vector2([slice6]);
 };
 GetVisitor.prototype.visitNull = wrapGet(getNull);
 GetVisitor.prototype.visitBool = wrapGet(getBool);
 GetVisitor.prototype.visitInt = wrapGet(getInt);
 GetVisitor.prototype.visitInt8 = wrapGet(getNumeric);
 GetVisitor.prototype.visitInt16 = wrapGet(getNumeric);
 GetVisitor.prototype.visitInt32 = wrapGet(getNumeric);
@@ -38759,17 +38950,17 @@
 GetVisitor.prototype.visitMap = wrapGet(getMap);
 var instance2 = new GetVisitor();
 
 // node_modules/apache-arrow/row/map.mjs
 var kKeys = Symbol.for("keys");
 var kVals = Symbol.for("vals");
 var MapRow = class {
-    constructor(slice7) {
-            this[kKeys] = new Vector2([slice7.children[0]]).memoize();
-            this[kVals] = slice7.children[1];
+    constructor(slice6) {
+            this[kKeys] = new Vector2([slice6.children[0]]).memoize();
+            this[kVals] = slice6.children[1];
             return new Proxy(this, new MapRowProxyHandler());
         }
         [Symbol.iterator]() {
             return new MapRowIterator(this[kKeys], this[kVals]);
         }
     get size() {
         return this[kKeys].length;
@@ -39925,31 +40116,31 @@
     const {
         [index3 * stride]: start2
     } = valueOffsets;
     const {
         [index3 * stride + 1]: end
     } = valueOffsets;
     const visit = instance5.getVisitFn(child.type);
-    const slice7 = child.slice(start2, end - start2);
+    const slice6 = child.slice(start2, end - start2);
     let size = 8;
     for (let idx = -1, len = end - start2; ++idx < len;) {
-        size += visit(slice7, idx);
+        size += visit(slice6, idx);
     }
     return size;
 };
 var getFixedSizeListByteLength = ({
     stride,
     children: children2
 }, index3) => {
     const child = children2[0];
-    const slice7 = child.slice(index3 * stride, stride);
+    const slice6 = child.slice(index3 * stride, stride);
     const visit = instance5.getVisitFn(child.type);
     let size = 0;
-    for (let idx = -1, len = slice7.length; ++idx < len;) {
-        size += visit(slice7, idx);
+    for (let idx = -1, len = slice6.length; ++idx < len;) {
+        size += visit(slice6, idx);
     }
     return size;
 };
 var getUnionByteLength = (data, index3) => {
     return data.type.mode === UnionMode.Dense ? getDenseUnionByteLength(data, index3) : getSparseUnionByteLength(data, index3);
 };
 var getDenseUnionByteLength = ({
@@ -40293,15 +40484,15 @@
     return "Vector";
 })(Vector2.prototype);
 var MemoizedVector = class extends Vector2 {
     constructor(vector2) {
         super(vector2.data);
         const get3 = this.get;
         const set4 = this.set;
-        const slice7 = this.slice;
+        const slice6 = this.slice;
         const cache = new Array(this.length);
         Object.defineProperty(this, "get", {
             value(index3) {
                 const cachedValue = cache[index3];
                 if (cachedValue !== void 0) {
                     return cachedValue;
                 }
@@ -40313,15 +40504,15 @@
         Object.defineProperty(this, "set", {
             value(index3, value) {
                 set4.call(this, index3, value);
                 cache[index3] = value;
             }
         });
         Object.defineProperty(this, "slice", {
-            value: (begin, end) => new MemoizedVector(slice7.call(this, begin, end))
+            value: (begin, end) => new MemoizedVector(slice6.call(this, begin, end))
         });
         Object.defineProperty(this, "isMemoized", {
             value: true
         });
         Object.defineProperty(this, "unmemoize", {
             value: () => new Vector2(this.data)
         });
@@ -45404,16 +45595,16 @@
     }
     /**
      * Return a zero-copy sub-section of this RecordBatch.
      * @param start The beginning of the specified portion of the RecordBatch.
      * @param end The end of the specified portion of the RecordBatch. This is exclusive of the element at the index 'end'.
      */
     slice(begin, end) {
-        const [slice7] = new Vector2([this.data]).slice(begin, end).data;
-        return new RecordBatch(this.schema, slice7);
+        const [slice6] = new Vector2([this.data]).slice(begin, end).data;
+        return new RecordBatch(this.schema, slice6);
     }
     /**
      * Returns a child Vector by name, or null if this Vector has no child with the given name.
      * @param name The name of the child to retrieve.
      */
     getChild(name) {
         var _b2;
@@ -48410,15 +48601,15 @@
 RecordBatchReader["throughDOM"] = recordBatchReaderThroughDOMStream;
 RecordBatchFileReader["throughDOM"] = recordBatchReaderThroughDOMStream;
 RecordBatchStreamReader["throughDOM"] = recordBatchReaderThroughDOMStream;
 RecordBatchWriter["throughDOM"] = recordBatchWriterThroughDOMStream;
 RecordBatchFileWriter["throughDOM"] = recordBatchWriterThroughDOMStream;
 RecordBatchStreamWriter["throughDOM"] = recordBatchWriterThroughDOMStream;
 
-// js/pyobsplot-js/parsing.js
+// packages/pyobsplot-js/parsing.js
 function unserialize_data(data, renderer) {
     let result = Array();
     for (let d of data) {
         if (d["pyobsplot-type"] == "DataFrame") {
             let value = d["value"];
             if (renderer == "jsdom") {
                 value = Buffer.from(value, "base64");
@@ -48500,15 +48691,15 @@
     }
     if (fun === void 0) {
         throw new Error(`${mod}.${method} is not defined`);
     }
     return fun;
 }
 
-// js/pyobsplot-js/plot.js
+// packages/pyobsplot-js/plot.js
 function generate_plot(spec, renderer) {
     let out;
     try {
         spec["data"] = unserialize_data(spec["data"], renderer);
         out = parse_spec(spec["code"], spec["data"]);
         if (spec["code"]["pyobsplot-type"] == "function") {
             out = out.plot();
@@ -48536,32 +48727,35 @@
     if (renderer == "jsdom") {
         console.log("<br>--- start pyobsplot debugging output ---<br>");
         console.log(out);
         console.log("<br>--- end pyobsplot debugging output ---</br>");
     }
 }
 
-// js/widget/widget.js
+// js/widget.js
 window.d3 = src_exports;
 window.Plot = src_exports2;
 
-function render(view) {
-    let spec = () => view.model.get("spec");
+function render({
+    model,
+    el
+}) {
+    let spec = () => model.get("spec");
     let plot_div = document.createElement("div");
     plot_div.classList.add("pyobsplot-plot");
     plot_div.classList.add(spec()["theme"]);
     let plot2 = generate_plot(spec(), "widget");
     plot_div.appendChild(plot2);
-    view.el.appendChild(plot_div);
-    view.model.on("change:spec", () => _onSpecValueChanged(view, view.el));
-    view.model.on("change:theme", () => _onThemeValueChanged(view, view.el));
+    el.appendChild(plot_div);
+    model.on("change:spec", () => _onSpecValueChanged(model, el));
+    model.on("change:theme", () => _onThemeValueChanged(model, el));
 }
 
-function _onSpecValueChanged(view, el) {
+function _onSpecValueChanged(model, el) {
     let plot2 = el.querySelector(".pyobsplot-plot");
     plot2.replaceChildren();
-    let spec = () => view.model.get("spec");
+    let spec = () => model.get("spec");
     plot2.appendChild(generate_plot(spec(), "widget"));
 }
 export {
     render
 };
```

### Comparing `pyobsplot-0.3.6/src/pyobsplot/utils.py` & `pyobsplot-0.3.7/src/pyobsplot/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import pathlib
 
 # Output directory of esbuild
 bundler_output_dir = pathlib.Path(__file__).parent / "static"
 
 # Minimum npm package version
-min_npm_version = "0.3.6"
+min_npm_version = "0.3.7"
 
 # Allowed default values
 allowed_defaults = [
     "marginTop",
     "marginRight",
     "marginBottom",
     "marginLeft",
```

### Comparing `pyobsplot-0.3.6/src/pyobsplot/widget.py` & `pyobsplot-0.3.7/src/pyobsplot/widget.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,18 +20,18 @@
     The specification can be given as a dict, a Plot function call or as
     Python kwargs.
     """
 
     # Disable _esm and _css watching and live reload to avoid "exception not rethrown"
     # error with pytest.
     _esm = anywidget._file_contents.FileContents(  # type: ignore
-        bundler_output_dir / "widget.js", start_thread=False
+        bundler_output_dir / "static-widget.js", start_thread=False
     )
     _css = anywidget._file_contents.FileContents(  # type: ignore
-        bundler_output_dir / "styles.css", start_thread=False
+        bundler_output_dir / "static-styles.css", start_thread=False
     )
     # spec traitlet : plot specification
     spec = traitlets.Dict().tag(sync=True)
 
     def __init__(
         self, spec, theme: str = default_theme, default: dict = {}, debug: bool = False
     ):
```

### Comparing `pyobsplot-0.3.6/PKG-INFO` & `pyobsplot-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobsplot
-Version: 0.3.6
+Version: 0.3.7
 Summary: Observable Plot in Jupyter notebooks and Quarto documents
 Home-page: https://github.com/juba/pyobsplot
 License: MIT
 Author: Julien Barnier
 Author-email: julien@nozav.org
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Dist: anywidget[dev] (>=0.4.3,<0.5.0)
+Requires-Dist: anywidget[dev] (>=0.6.0,<0.7.0)
 Requires-Dist: ipywidgets (>=8.0.0)
 Requires-Dist: jupyterlab (>=3.6.0)
 Requires-Dist: jupyterlab_widgets (>=3.0.0)
 Requires-Dist: pandas (>=1.2.0)
 Requires-Dist: polars (>=0.16.0)
 Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
```

