# Comparing `tmp/uproot_browser-0.4.2.tar.gz` & `tmp/uproot_browser-0.5.0.tar.gz`

## Comparing `uproot_browser-0.4.2.tar` & `uproot_browser-0.5.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/noxfile.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/.github/dependabot.yml
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/docs/make_logo.py
--rw-r--r--   0        0        0    71775 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/docs/_images/iterm.png
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/docs/_images/uproot-browser-logo.png
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/src/uproot_browser/__init__.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/src/uproot_browser/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/src/uproot_browser/_version.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/src/uproot_browser/_version.pyi
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/src/uproot_browser/dirs.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/src/uproot_browser/exceptions.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/src/uproot_browser/footer.py
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/src/uproot_browser/header.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/src/uproot_browser/plot.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/src/uproot_browser/plot_mpl.py
--rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/src/uproot_browser/plot_view.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/src/uproot_browser/py.typed
--rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/src/uproot_browser/tree.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/src/uproot_browser/tree_view.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/src/uproot_browser/tui.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/tests/test_dirs.py
--rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/tests/test_printouts.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/LICENSE
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/README.md
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    13684 2020-02-02 00:00:00.000000 uproot_browser-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/noxfile.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/docs/make_logo.py
+-rw-r--r--   0        0        0    71775 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/docs/_images/iterm.png
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/docs/_images/uproot-browser-logo.png
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/__init__.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/_version.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/_version.pyi
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/dirs.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/exceptions.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/plot.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/plot_mpl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/py.typed
+-rw-r--r--   0        0        0     5736 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/tree.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/tui/__init__.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/tui/browser.css
+-rw-r--r--   0        0        0     5348 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/tui/browser.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/tui/left_panel.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/tui/right_panel.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/tests/test_dirs.py
+-rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/tests/test_printouts.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/LICENSE
+-rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/README.md
+-rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    14217 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/PKG-INFO
```

### Comparing `uproot_browser-0.4.2/.pre-commit-config.yaml` & `uproot_browser-0.5.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
 - repo: https://github.com/psf/black
-  rev: 23.1.0
+  rev: 23.3.0
   hooks:
   - id: black
 
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.4.0
   hooks:
   - id: check-added-large-files
@@ -15,28 +15,28 @@
   - id: debug-statements
   - id: end-of-file-fixer
   - id: mixed-line-ending
   - id: requirements-txt-fixer
   - id: trailing-whitespace
 
 - repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: "v0.0.254"
+  rev: "v0.0.262"
   hooks:
     - id: ruff
       args: ["--fix", "--show-fixes"]
 
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: v1.0.1
+  rev: v1.2.0
   hooks:
   - id: mypy
     files: src
-    additional_dependencies: [rich>=12, click>=8.1.1, hist, numpy, textual==0.1.17]
+    additional_dependencies: [rich>=12, click>=8.1.1, hist, numpy, textual>0.18]
 
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.2.2
+  rev: v2.2.4
   hooks:
   - id: codespell
     args: [-L, "hist,iterm"]
 
 - repo: local
   hooks:
   - id: disallow-caps
```

### Comparing `uproot_browser-0.4.2/noxfile.py` & `uproot_browser-0.5.0/noxfile.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,7 +38,17 @@
 def build(session: nox.Session) -> None:
     """
     Build an SDist and wheel.
     """
 
     session.install("build")
     session.run("python", "-m", "build")
+
+
+@nox.session
+def make_logo(session: nox.Session) -> None:
+    """
+    Rerender the logo
+    """
+
+    session.install("pillow")
+    session.run("python", "docs/make_logo.py")
```

### Comparing `uproot_browser-0.4.2/.github/CONTRIBUTING.md` & `uproot_browser-0.5.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.4.2/.github/workflows/ci.yml` & `uproot_browser-0.5.0/.github/workflows/ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -50,14 +50,17 @@
 
     - name: Test package
       run: python -m pytest -ra
 
   pass:
     if: always()
     needs: [checks]
+    environment: pypi
+    permissions:
+      id-token: write
     runs-on: ubuntu-latest
     steps:
       - name: Decide whether the needed jobs succeeded or failed
         uses: re-actors/alls-green@release/v1
         with:
           jobs: ${{ toJSON(needs) }}
 
@@ -75,11 +78,9 @@
     - uses: actions/upload-artifact@v3
       with:
         path: dist
 
     - name: Check products
       run: pipx run twine check dist/*
 
-    - uses: pypa/gh-action-pypi-publish@v1.6.4
+    - uses: pypa/gh-action-pypi-publish@v1.8.5
       if: github.event_name == 'release' && github.event.action == 'published'
-      with:
-        password: ${{ secrets.pypi_password }}
```

### Comparing `uproot_browser-0.4.2/docs/make_logo.py` & `uproot_browser-0.5.0/docs/make_logo.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import PIL.Image
 import PIL.ImageDraw
 import PIL.ImageFilter
 import PIL.ImageFont
 
 LOGO = """\
-┬ ┬┌─┐┬─┐┌─┐┌─┐┌┬┐4 ┌┐ ┬─┐┌─┐┬ ┬┌─┐┌─┐┬─┐
+┬ ┬┌─┐┬─┐┌─┐┌─┐┌┬┐5 ┌┐ ┬─┐┌─┐┬ ┬┌─┐┌─┐┬─┐
 │ │├─┘├┬┘│ ││ │ │───├┴┐├┬┘│ ││││└─┐├┤ ├┬┘
 └─┘┴  ┴└─└─┘└─┘ ┴   └─┘┴└─└─┘└┴┘└─┘└─┘┴└─
 """
 
 image = PIL.Image.new("RGBA", (810, 120), color=(0, 0, 0, 0))
 
 draw = PIL.ImageDraw.Draw(image)
 
 font = PIL.ImageFont.truetype("Sauce Code Pro Medium Nerd Font Complete.ttf", 32)
 
 draw.text((10, 0), LOGO, font=font, fill=(128, 128, 128, 255))
 
-image.save("uproot-browser-logo.png")
+image.save("docs/_images/uproot-browser-logo.png")
```

### Comparing `uproot_browser-0.4.2/docs/_images/iterm.png` & `uproot_browser-0.5.0/docs/_images/iterm.png`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.4.2/src/uproot_browser/__main__.py` & `uproot_browser-0.5.0/src/uproot_browser/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 """
 This is the click-powered CLI.
 """
 
 from __future__ import annotations
 
-import asyncio
 import functools
 import os
 from pathlib import Path
 from typing import Any, Callable
 
 import click
-import rich
 import uproot
 
 from ._version import version as __version__
 
 CONTEXT_SETTINGS = {"help_option_names": ["-h", "--help"]}
 
 VERSION = __version__
@@ -93,36 +91,25 @@
         uproot_browser.plot.clf()
         uproot_browser.plot.plot(item)
         uproot_browser.plot.show()
 
 
 @main.command()
 @click.argument("filename")
-@click.option(
-    "--logging", is_flag=True, help="Write log information to the textual.log file."
-)
-def browse(filename: str, logging: bool) -> None:
+def browse(filename: str) -> None:
     """
     Display a TUI.
     """
-    import uproot_browser.tui  # pylint: disable=import-outside-toplevel
+    import uproot_browser.dirs  # pylint: disable=import-outside-toplevel
+    import uproot_browser.tui.browser  # pylint: disable=import-outside-toplevel
 
     fname = uproot_browser.dirs.filename(filename)
 
-    # Run the uproot-browser TUI
-    async def amain() -> list[Any]:
-        app = uproot_browser.tui.Browser(
-            title="uproot-browser",
-            path=Path(fname),
-            log="textual.log" if logging else None,
-        )
-        await app.process_messages()
-        return app.results
-
-    results = asyncio.run(amain())
+    app = uproot_browser.tui.browser.Browser(
+        path=Path(fname),
+    )
 
-    for result in results:
-        rich.print(result)
+    app.run()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `uproot_browser-0.4.2/src/uproot_browser/dirs.py` & `uproot_browser-0.5.0/src/uproot_browser/dirs.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,14 @@
 def selections(select: str) -> tuple[str, ...]:
     """
     Return the directory/tree portion of a colon-separated selection.
     """
     return tuple(select.split(":")[1:])
 
 
-def apply_selection(tree: Any, select: Iterable[str]) -> Iterable[Any]:
+def apply_selection(tree: Any, selection: Iterable[str]) -> Iterable[Any]:
     """
     Apply a colon-separated selection to an uproot tree. Slashes are handled by uproot.
     """
-    for sel in select:
+    for sel in selection:
         tree = tree[sel]
         yield tree
```

### Comparing `uproot_browser-0.4.2/src/uproot_browser/plot.py` & `uproot_browser-0.5.0/src/uproot_browser/plot.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.4.2/src/uproot_browser/plot_mpl.py` & `uproot_browser-0.5.0/src/uproot_browser/plot_mpl.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.4.2/src/uproot_browser/plot_view.py` & `uproot_browser-0.5.0/src/uproot_browser/tui/right_panel.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,115 +1,123 @@
 from __future__ import annotations
 
+import dataclasses
+from types import TracebackType
 from typing import Any
 
-import plotext as plt
-import rich.align
-import rich.box
-import rich.console
+import numpy as np
+import plotext as plt  # plots in text
 import rich.panel
-import rich.pretty
 import rich.text
+import rich.traceback
 import textual.widget
-import uproot
+import textual.widgets
 
-import uproot_browser.dirs
 import uproot_browser.plot
-from uproot_browser.exceptions import EmptyTreeError
-
-EMPTY = object()
 
 LOGO = """\
 Scikit-HEP
-┬ ┬┌─┐┬─┐┌─┐┌─┐┌┬┐4 ┌┐ ┬─┐┌─┐┬ ┬┌─┐┌─┐┬─┐
+┬ ┬┌─┐┬─┐┌─┐┌─┐┌┬┐5 ┌┐ ┬─┐┌─┐┬ ┬┌─┐┌─┐┬─┐
 │ │├─┘├┬┘│ ││ │ │───├┴┐├┬┘│ ││││└─┐├┤ ├┬┘
 └─┘┴  ┴└─└─┘└─┘ ┴   └─┘┴└─└─┘└┴┘└─┘└─┘┴└─
                 Powered by Textual & Hist"""
 
+LOGO_PANEL = rich.text.Text.from_ansi(LOGO, no_wrap=True)
+
 
-LOGO_PANEL = rich.panel.Panel(
-    rich.align.Align.center(
-        rich.text.Text.from_ansi(LOGO, no_wrap=True), vertical="middle"
-    ),
-    border_style="green",
-    box=rich.box.ROUNDED,
-)
+placeholder = np.random.rand(1000)
 
 
-def make_plot(item: Any, *size: int) -> Any:
+def make_plot(item: Any, theme: str, *size: int) -> Any:
     plt.clf()
     plt.plotsize(*size)
     uproot_browser.plot.plot(item)
+    plt.theme(theme)
     return plt.build()
 
 
-class Plot:
-    def __init__(self, item: Any) -> None:
-        self.item: Any = item
-        self.max_frames = 2
+# wrapper for plotext into a textual widget
+@dataclasses.dataclass
+class Plotext:
+    upfile: Any
+    selection: str
+    theme: str
 
     def __rich_console__(
         self, console: rich.console.Console, options: rich.console.ConsoleOptions
     ) -> rich.console.RenderResult:
+        *_, item = uproot_browser.dirs.apply_selection(
+            self.upfile, self.selection.split(":")
+        )
+
+        if item is None:
+            yield rich.text.Text()
+            return
         width = options.max_width or console.width
         height = options.height or console.height
-        try:
-            canvas = make_plot(self.item, width, height)
-            yield rich.text.Text.from_ansi(canvas)
-        except EmptyTreeError:
-            yield rich.panel.Panel(
-                rich.align.Align.center(
-                    f"[green]{self.item.name} is EMPTY",
-                    vertical="middle",
-                ),
-                border_style="red",
-                box=rich.box.ROUNDED,
-                width=width,
-                height=height,
-            )
-        except Exception:
-            tb = rich.traceback.Traceback(
-                extra_lines=1,
-                max_frames=self.max_frames,  # Can't be less than 4 frames
-                width=width,
-            )
-            tb.max_frames = self.max_frames
-            yield tb
+
+        canvas = make_plot(item, self.theme, width, height)
+        yield rich.text.Text.from_ansi(canvas)
 
 
 class PlotWidget(textual.widget.Widget):
-    def __init__(self, uproot_file: uproot.ReadOnlyFile) -> None:
-        super().__init__()
-        self.file = uproot_file
-        self.plot: rich.panel.Panel | Plot | None = LOGO_PANEL
-        self.plot_path: str | None = None
-
-    def set_plot(self, plot_path: str | None) -> None:
-        self.plot_path = plot_path
-        if plot_path is None:
-            self.plot = plot_path
-        else:
-            *_, item = uproot_browser.dirs.apply_selection(
-                self.file, plot_path.split(":")
-            )
-            self.plot = Plot(item)
+    _item: Plotext | None
 
-    async def update(self) -> None:
+    @property
+    def item(self) -> Plotext | None:
+        return self._item
+
+    @item.setter
+    def item(self, value: Plotext) -> None:
+        self._item = value
         self.refresh()
 
+    def __init__(self, **kargs: Any):
+        super().__init__(**kargs)
+        self._item = None
+
+    def render(self) -> rich.console.RenderableType:
+        return self.item or ""
+
+
+class EmptyWidget(textual.widget.Widget):
+    # if the plot is empty
+
+    def render(self) -> rich.console.RenderableType:
+        return rich.text.Text("Plot is Empty")
+
+
+class LogoWidget(textual.widget.Widget):
     def render(self) -> rich.console.RenderableType:
-        if self.plot is None:
-            return rich.panel.Panel(
-                rich.align.Align.center(
-                    rich.pretty.Pretty(
-                        "No plot selected!", no_wrap=True, overflow="ellipsis"
-                    ),
-                    vertical="middle",
-                ),
-                border_style="red",
-                box=rich.box.ROUNDED,
-            )
+        return LOGO_PANEL
+
+
+@dataclasses.dataclass
+class Error:
+    exc: tuple[type[BaseException], BaseException, TracebackType]
+
+    def __rich_console__(
+        self, console: rich.console.Console, options: rich.console.ConsoleOptions
+    ) -> rich.console.RenderResult:
+        width = options.max_width or console.width
+
+        yield rich.traceback.Traceback.from_exception(*self.exc, width=width)
+
 
-        if isinstance(self.plot, rich.panel.Panel):
-            return self.plot
+class ErrorWidget(textual.widgets.TextLog):
+    _exc: Error | None
 
-        return rich.panel.Panel(self.plot)
+    @property
+    def exc(self) -> Error | None:
+        return self._exc
+
+    @exc.setter
+    def exc(self, value: Error) -> None:
+        self._exc = value
+        self.clear()
+        self.write(self._exc)
+        # self.refresh()
+
+    def __init__(self, **kargs: Any):
+        super().__init__(**kargs)
+        self.write("No Exception set!")
+        self._exc = None
```

### Comparing `uproot_browser-0.4.2/src/uproot_browser/tree.py` & `uproot_browser-0.5.0/src/uproot_browser/tree.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,179 +2,219 @@
 Display tools for TTrees.
 """
 
 from __future__ import annotations
 
 import dataclasses
 import functools
+import sys
 from pathlib import Path
-from typing import Any, Dict
+from typing import Any
 
 import uproot
+import uproot.reading
 from rich.console import Console
 from rich.markup import escape
 from rich.text import Text
 from rich.tree import Tree
 
+if sys.version_info < (3, 8):
+    from typing_extensions import TypedDict
+else:
+    from typing import TypedDict
+
 console = Console()
 
-__all__ = ("make_tree", "process_item", "print_tree", "UprootItem", "console")
+__all__ = (
+    "make_tree",
+    "process_item",
+    "print_tree",
+    "UprootEntry",
+    "console",
+    "MetaDict",
+)
 
 
 def __dir__() -> tuple[str, ...]:
     return __all__
 
 
+class MetaDictRequired(TypedDict, total=True):
+    label_text: Text
+    label_icon: str
+
+
+class MetaDict(MetaDictRequired, total=False):
+    guide_style: str
+
+
 @dataclasses.dataclass
-class UprootItem:
+class UprootEntry:
     path: str
     item: Any
 
     @property
     def is_dir(self) -> bool:
-        # also uproot.TBranch Element with len(TBranch.branches) > 0
-        return (
-            isinstance(self.item, uproot.reading.ReadOnlyDirectory)
-            or isinstance(self.item, uproot.behaviors.TBranch.HasBranches)
-            and len(self.item.branches) > 0
-        )
+        if isinstance(self.item, uproot.reading.ReadOnlyDirectory):
+            return True
+        if isinstance(self.item, uproot.behaviors.TBranch.HasBranches):
+            return len(self.item.branches) > 0
+        return False
 
-    def meta(self) -> dict[str, Any]:
+    def meta(self) -> MetaDict:
         return process_item(self.item)
 
     def label(self) -> Text:
-        return process_item(self.item)["label"]  # type: ignore[no-any-return]
+        meta = self.meta()
+        return Text.assemble(meta["label_icon"], meta["label_text"])
+
+    def tree_args(self) -> dict[str, Any]:
+        d: dict[str, Text | str] = {"label": self.label()}
+        if "guide_style" in self.meta():
+            d["guide_style"] = self.meta()["guide_style"]
+        return d
 
     @property
-    def children(self) -> list[UprootItem]:
+    def children(self) -> list[UprootEntry]:
         if not self.is_dir:
             return []
         if isinstance(self.item, uproot.reading.ReadOnlyDirectory):
             items = {
                 key.split(";")[0]
                 for key in self.item.keys()  # noqa: SIM118
                 if "/" not in key
             }
+        elif isinstance(self.item, uproot.behaviors.TBranch.HasBranches):
+            items = {item.name for item in self.item.branches}
         else:
             items = {obj.name.split(";")[0] for obj in self.item.branches}
         return [
-            UprootItem(f"{self.path}/{key}", self.item[key]) for key in sorted(items)
+            UprootEntry(f"{self.path}/{key}", self.item[key]) for key in sorted(items)
         ]
 
 
-def make_tree(node: UprootItem, *, tree: Tree | None = None) -> Tree:
+def make_tree(node: UprootEntry, *, tree: Tree | None = None) -> Tree:
     """
     Given an object, build a rich.tree.Tree output.
     """
 
-    tree = Tree(**node.meta()) if tree is None else tree.add(**node.meta())
+    tree = Tree(**node.tree_args()) if tree is None else tree.add(**node.tree_args())
 
     for child in node.children:
         make_tree(child, tree=tree)
 
     return tree
 
 
 @functools.singledispatch
-def process_item(uproot_object: Any) -> Dict[str, Any]:
+def process_item(uproot_object: Any) -> MetaDict:
     """
     Given an unknown object, return a rich.tree.Tree output. Specialize for known objects.
     """
     name = getattr(uproot_object, "name", "<unnamed>")
     classname = getattr(uproot_object, "classname", uproot_object.__class__.__name__)
-    label = Text.assemble(
-        "❓ ",
+    label_text = Text.assemble(
         (f"{name} ", "bold"),
         (classname, "italic"),
     )
-    return {"label": label}
+    return MetaDict(label_icon="❓ ", label_text=label_text)
 
 
 @process_item.register
 def _process_item_tfile(
     uproot_object: uproot.reading.ReadOnlyDirectory,
-) -> Dict[str, Any]:
+) -> MetaDict:
     """
     Given an TFile, return a rich.tree.Tree output.
     """
     path = Path(uproot_object.file_path)
 
     if uproot_object.path:
         # path is to a TDirectory on tree
         path_name = escape(uproot_object.path[0])
         link_text = f"file://{path}:/{path_name}"
     else:
         # path is the top of the tree: the file
         path_name = escape(path.name)
         link_text = f"file://{path}"
 
-    label = Text.from_markup(f":file_folder: [link {link_text}]{path_name}")
+    label_text = Text.from_markup(f"[link {link_text}]{path_name}")
 
-    return {
-        "label": label,
-        "guide_style": "bold bright_blue",
-    }
+    return MetaDict(
+        label_icon="📁 ",
+        label_text=label_text,
+        guide_style="bold bright_blue",
+    )
 
 
 @process_item.register
-def _process_item_ttree(uproot_object: uproot.TTree) -> Dict[str, Any]:
+def _process_item_ttree(uproot_object: uproot.TTree) -> MetaDict:
     """
     Given an tree, return a rich.tree.Tree output.
     """
-    label = Text.assemble(
-        "🌴 ",
+    label_text = Text.assemble(
         (f"{uproot_object.name} ", "bold"),
         f"({uproot_object.num_entries:g})",
     )
 
-    return {
-        "label": label,
-        "guide_style": "bold bright_green",
-    }
+    return MetaDict(
+        label_icon="🌴 ",
+        label_text=label_text,
+        guide_style="bold bright_green",
+    )
 
 
 @process_item.register
-def _process_item_tbranch(uproot_object: uproot.TBranch) -> Dict[str, Any]:
+def _process_item_tbranch(uproot_object: uproot.TBranch) -> MetaDict:
     """
     Given an branch, return a rich.tree.Tree output.
     """
 
     jagged = isinstance(
         uproot_object.interpretation, uproot.interpretation.jagged.AsJagged
     )
     icon = "🍃 " if jagged else "🍁 "
 
-    label = Text.assemble(
-        icon,
+    if len(uproot_object.branches):
+        icon = "🌿 "
+
+    label_text = Text.assemble(
         (f"{uproot_object.name} ", "bold"),
         (f"{uproot_object.typename}", "italic"),
     )
-    return {"label": label}
+
+    return MetaDict(
+        label_icon=icon,
+        label_text=label_text,
+        guide_style="bold bright_green",
+    )
 
 
 @process_item.register
-def _process_item_th(uproot_object: uproot.behaviors.TH1.Histogram) -> Dict[str, Any]:
+def _process_item_th(uproot_object: uproot.behaviors.TH1.Histogram) -> MetaDict:
     """
     Given an histogram, return a rich.tree.Tree output.
     """
     icon = "📊 " if uproot_object.kind == "COUNT" else "📈 "
     sizes = " × ".join(f"{len(ax)}" for ax in uproot_object.axes)
 
-    label = Text.assemble(
-        icon,
+    label_text = Text.assemble(
         (f"{uproot_object.name} ", "bold"),
         (f"{uproot_object.classname} ", "italic"),
         f"({sizes})",
     )
-    return {"label": label}
+    return MetaDict(
+        label_icon=icon,
+        label_text=label_text,
+    )
 
 
 # pylint: disable-next=redefined-outer-name
 def print_tree(entry: str, *, console: Console = console) -> None:
     """
     Prints a tree given a specification string. Currently, that must be a
     single filename. Colons are not allowed currently in the filename.
     """
 
     upfile = uproot.open(entry)
-    tree = make_tree(UprootItem("/", upfile))
+    tree = make_tree(UprootEntry("/", upfile))
     console.print(tree)
```

### Comparing `uproot_browser-0.4.2/src/uproot_browser/tree_view.py` & `uproot_browser-0.5.0/src/uproot_browser/tui/left_panel.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,111 +1,78 @@
 from __future__ import annotations
 
-from functools import lru_cache
 from pathlib import Path
+from typing import Any
 
-import rich.console
+import rich.panel
 import rich.repr
-import textual.events
+import rich.text
 import textual.message
-import textual.reactive
+import textual.widget
 import textual.widgets
+import textual.widgets.tree
 import uproot
-from textual._types import MessageTarget
+from rich.style import Style
 
-from .tree import UprootItem
+from ..tree import UprootEntry
 
 
 @rich.repr.auto
-class UprootClick(textual.message.Message, bubble=True):
-    def __init__(self, sender: MessageTarget, path: str) -> None:
+class UprootSelected(textual.message.Message, bubble=True):
+    def __init__(self, upfile: Any, path: str) -> None:
+        self.upfile = upfile
         self.path = path
-        super().__init__(sender)
+        super().__init__()
 
 
-class TreeView(textual.widgets.TreeControl[UprootItem]):
-    """A tree view for the uproot-browser"""
+class UprootTree(textual.widgets.Tree[UprootEntry]):
+    """currently just extending DirectoryTree, showing current path"""
 
-    def __init__(self, path: Path) -> None:
+    def __init__(self, path: Path, **args: Any) -> None:
         self.upfile = uproot.open(path)
-        data = UprootItem("/", self.upfile)
-        super().__init__(name=path.name, label=path.stem, data=data)
-        self.root.tree.guide_style = "black"
+        data = UprootEntry("/", self.upfile)
+        super().__init__(name=path.name, data=data, label=path.stem, **args)
 
-    has_focus: textual.reactive.Reactive[bool] = textual.reactive.Reactive(False)
-
-    def on_focus(self) -> None:
-        self.has_focus = True
-
-    def on_blur(self) -> None:
-        self.has_focus = False
-
-    async def watch_hover_node(self, hover_node: textual.widgets.NodeID) -> None:
-        for node in self.nodes.values():
-            node.tree.guide_style = "bold" if node.id == hover_node else ""
-        self.refresh(layout=True)
-
-    def render_node(
-        self, node: textual.widgets.TreeNode[UprootItem]
-    ) -> rich.console.RenderableType:
-        return render_tree_label(
-            node,
-            node.data.is_dir,
-            node.expanded,
-            node.is_cursor,
-            node.id == self.hover_node,
-            self.has_focus,
-        )
-
-    async def on_mount(
+    def render_label(
         self,
-        event: textual.events.Mount,  # noqa: ARG002
-    ) -> None:
-        await self.load_directory(self.root)
-
-    async def load_directory(self, node: textual.widgets.TreeNode[UprootItem]) -> None:
-        children = node.data.children
-        for child in children:
-            await node.add(child.path, child)
-        node.loaded = True
-        await node.expand()
+        node: textual.widgets.tree.TreeNode[UprootEntry],
+        base_style: Style,
+        style: Style,  # ,
+    ) -> rich.text.Text:
+        assert node.data
+        meta = node.data.meta()
+        label_icon = rich.text.Text(meta["label_icon"])
+        label_icon.stylize(base_style)
+
+        label = rich.text.Text.assemble(label_icon, meta["label_text"])
+        label.stylize(style)
+        return label
+
+    def on_mount(self) -> None:
+        self.load_directory(self.root)
+
+    def load_directory(self, node: textual.widgets.tree.TreeNode[UprootEntry]) -> None:
+        assert node.data
+        if not node.children:
+            children = node.data.children
+            for child in children:
+                node.add(child.path, child)
+        node.expand()
         self.refresh(layout=True)
 
-    async def handle_tree_click(
-        self, message: textual.widgets.TreeClick[UprootItem]
+    def on_tree_node_selected(
+        self, event: textual.widgets.Tree.NodeSelected[UprootEntry]
     ) -> None:
-        item = message.node.data
+        event.stop()
+        item = event.node.data
+        assert item
         if not item.is_dir:
-            await self.emit(UprootClick(self, item.path))
-        else:
-            if not message.node.loaded:
-                await self.load_directory(message.node)
-                await message.node.expand()
-            else:
-                await message.node.toggle()
-
-
-@lru_cache(maxsize=1024 * 32)
-def render_tree_label(
-    node: textual.widgets.TreeNode[UprootItem],
-    is_dir: bool,
-    expanded: bool,
-    is_cursor: bool,
-    is_hover: bool,
-    has_focus: bool,
-) -> rich.console.RenderableType:
-    meta = {
-        "@click": f"click_label({node.id})",
-        "tree_node": node.id,
-        "cursor": node.is_cursor,
-    }
-    icon_label = node.data.meta()["label"]
-    icon_label.apply_meta(meta)
-
-    if is_hover:
-        icon_label.stylize("underline")
-    if is_cursor and has_focus:
-        icon_label.stylize("reverse")
-    if is_dir:
-        icon_label.stylize("green4" if expanded else "spring_green3")
+            self.post_message(UprootSelected(self.upfile, item.path))
 
-    return icon_label  # type: ignore[no-any-return]
+    def on_tree_node_expanded(
+        self, event: textual.widgets.Tree.NodeSelected[UprootEntry]
+    ) -> None:
+        event.stop()
+        item = event.node.data
+        assert item
+        if item.is_dir:
+            self.load_directory(event.node)
```

### Comparing `uproot_browser-0.4.2/tests/test_printouts.py` & `uproot_browser-0.5.0/tests/test_printouts.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
 from uproot_browser.tree import print_tree
 
 OUT1 = """\
 📁 uproot-Event.root
 ┣━━ ❓ <unnamed> TProcessID
 ┣━━ 🌴 T (1000)
-┃   ┗━━ 🍁 event Event
-┃       ┣━━ 🍁 TObject (group of fUniqueID:uint32_t, fBits:uint32_t)
+┃   ┗━━ 🌿 event Event
+┃       ┣━━ 🌿 TObject (group of fUniqueID:uint32_t, fBits:uint32_t)
 ┃       ┃   ┣━━ 🍁 fBits uint32_t
 ┃       ┃   ┗━━ 🍁 fUniqueID uint32_t
 ┃       ┣━━ 🍁 fClosestDistance unknown[]
 ┃       ┣━━ 🍁 fEventName char*
-┃       ┣━━ 🍁 fEvtHdr EventHeader
+┃       ┣━━ 🌿 fEvtHdr EventHeader
 ┃       ┃   ┣━━ 🍁 fEvtHdr.fDate int32_t
 ┃       ┃   ┣━━ 🍁 fEvtHdr.fEvtNum int32_t
 ┃       ┃   ┗━━ 🍁 fEvtHdr.fRun int32_t
 ┃       ┣━━ 🍁 fFlag uint32_t
 ┃       ┣━━ 🍁 fH TH1F
 ┃       ┣━━ 🍁 fHighPt TRefArray*
 ┃       ┣━━ 🍁 fIsValid bool
@@ -30,15 +30,15 @@
 ┃       ┣━━ 🍁 fMatrix[4][4] float[4][4]
 ┃       ┣━━ 🍁 fMeasures[10] int32_t[10]
 ┃       ┣━━ 🍁 fMuons TRefArray*
 ┃       ┣━━ 🍁 fNseg int32_t
 ┃       ┣━━ 🍁 fNtrack int32_t
 ┃       ┣━━ 🍁 fNvertex uint32_t
 ┃       ┣━━ 🍁 fTemperature float
-┃       ┣━━ 🍁 fTracks TClonesArray*
+┃       ┣━━ 🌿 fTracks TClonesArray*
 ┃       ┃   ┣━━ 🍃 fTracks.fBits uint32_t[]
 ┃       ┃   ┣━━ 🍃 fTracks.fBx Float16_t[]
 ┃       ┃   ┣━━ 🍃 fTracks.fBy Float16_t[]
 ┃       ┃   ┣━━ 🍃 fTracks.fCharge Double32_t[]
 ┃       ┃   ┣━━ 🍃 fTracks.fMass2 Float16_t[]
 ┃       ┃   ┣━━ 🍃 fTracks.fMeanCharge float[]
 ┃       ┃   ┣━━ 🍃 fTracks.fNpoint int32_t[]
@@ -59,16 +59,16 @@
 ┃       ┃   ┣━━ 🍃 fTracks.fVertex[3] Double32_t[][3]
 ┃       ┃   ┣━━ 🍃 fTracks.fXfirst Float16_t[]
 ┃       ┃   ┣━━ 🍃 fTracks.fXlast Float16_t[]
 ┃       ┃   ┣━━ 🍃 fTracks.fYfirst Float16_t[]
 ┃       ┃   ┣━━ 🍃 fTracks.fYlast Float16_t[]
 ┃       ┃   ┣━━ 🍃 fTracks.fZfirst Float16_t[]
 ┃       ┃   ┗━━ 🍃 fTracks.fZlast Float16_t[]
-┃       ┣━━ 🍁 fTriggerBits TBits
-┃       ┃   ┣━━ 🍁 fTriggerBits.TObject (group of fTriggerBits.fUniqueID:uint32_t, fTriggerBits.fBits:uint32_t)
+┃       ┣━━ 🌿 fTriggerBits TBits
+┃       ┃   ┣━━ 🌿 fTriggerBits.TObject (group of fTriggerBits.fUniqueID:uint32_t, fTriggerBits.fBits:uint32_t)
 ┃       ┃   ┃   ┣━━ 🍁 fTriggerBits.fBits uint32_t
 ┃       ┃   ┃   ┗━━ 🍁 fTriggerBits.fUniqueID uint32_t
 ┃       ┃   ┣━━ 🍃 fTriggerBits.fAllBits uint8_t[]
 ┃       ┃   ┣━━ 🍁 fTriggerBits.fNbits uint32_t
 ┃       ┃   ┗━━ 🍁 fTriggerBits.fNbytes uint32_t
 ┃       ┣━━ 🍁 fType[20] int8_t[20]
 ┃       ┗━━ 🍁 fWebHistogram TRef
```

### Comparing `uproot_browser-0.4.2/.gitignore` & `uproot_browser-0.5.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 celerybeat.pid
 
 # SageMath parsed files
 *.sage.py
 
 # Environments
 .env
-.venv
+.venv*
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
 
 # Spyder project settings
```

### Comparing `uproot_browser-0.4.2/LICENSE` & `uproot_browser-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.4.2/README.md` & `uproot_browser-0.5.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -99,74 +99,74 @@
 **`tree` command:**
 
 ```bash
 uproot-browser tree ../scikit-hep-testdata/src/skhep_testdata/data/uproot-Event.root
 📁 uproot-Event.root
 ┣━━ ❓ <unnamed> TProcessID
 ┣━━ 🌴 T (1000)
-┃   ┣━━ 🍁 event Event
-┃   ┣━━ 🍁 TObject (group of fUniqueID:uint32_t, fBits:uint8_t)
-┃   ┣━━ 🍁 fBits uint8_t
-┃   ┣━━ 🍁 fUniqueID uint32_t
-┃   ┣━━ 🍁 fClosestDistance unknown[]
-┃   ┣━━ 🍁 fEventName char*
-┃   ┣━━ 🍁 fEvtHdr EventHeader
-┃   ┣━━ 🍁 fEvtHdr.fDate int32_t
-┃   ┣━━ 🍁 fEvtHdr.fEvtNum int32_t
-┃   ┣━━ 🍁 fEvtHdr.fRun int32_t
-┃   ┣━━ 🍁 fFlag uint32_t
-┃   ┣━━ 🍁 fH TH1F
-┃   ┣━━ 🍁 fHighPt TRefArray*
-┃   ┣━━ 🍁 fIsValid bool
-┃   ┣━━ 🍁 fLastTrack TRef
-┃   ┣━━ 🍁 fMatrix[4][4] float[4][4]
-┃   ┣━━ 🍁 fMeasures[10] int32_t[10]
-┃   ┣━━ 🍁 fMuons TRefArray*
-┃   ┣━━ 🍁 fNseg int32_t
-┃   ┣━━ 🍁 fNtrack int32_t
-┃   ┣━━ 🍁 fNvertex uint32_t
-┃   ┣━━ 🍁 fTemperature float
-┃   ┣━━ 🍁 fTracks TClonesArray*
-┃   ┣━━ 🍃 fTracks.fBits uint8_t[]
-┃   ┣━━ 🍃 fTracks.fBx Float16_t[]
-┃   ┣━━ 🍃 fTracks.fBy Float16_t[]
-┃   ┣━━ 🍃 fTracks.fCharge Double32_t[]
-┃   ┣━━ 🍃 fTracks.fMass2 Float16_t[]
-┃   ┣━━ 🍃 fTracks.fMeanCharge float[]
-┃   ┣━━ 🍃 fTracks.fNpoint int32_t[]
-┃   ┣━━ 🍃 fTracks.fNsp uint32_t[]
-┃   ┣━━ 🍁 fTracks.fPointValue unknown[][]
-┃   ┣━━ 🍃 fTracks.fPx float[]
-┃   ┣━━ 🍃 fTracks.fPy float[]
-┃   ┣━━ 🍃 fTracks.fPz float[]
-┃   ┣━━ 🍃 fTracks.fRandom float[]
-┃   ┣━━ 🍃 fTracks.fTArray[3] float[][3]
-┃   ┣━━ 🍁 fTracks.fTriggerBits.fAllBits uint8_t[][]
-┃   ┣━━ 🍃 fTracks.fTriggerBits.fBits uint8_t[]
-┃   ┣━━ 🍃 fTracks.fTriggerBits.fNbits uint32_t[]
-┃   ┣━━ 🍃 fTracks.fTriggerBits.fNbytes uint32_t[]
-┃   ┣━━ 🍃 fTracks.fTriggerBits.fUniqueID uint32_t[]
-┃   ┣━━ 🍃 fTracks.fUniqueID uint32_t[]
-┃   ┣━━ 🍃 fTracks.fValid int16_t[]
-┃   ┣━━ 🍃 fTracks.fVertex[3] Double32_t[][3]
-┃   ┣━━ 🍃 fTracks.fXfirst Float16_t[]
-┃   ┣━━ 🍃 fTracks.fXlast Float16_t[]
-┃   ┣━━ 🍃 fTracks.fYfirst Float16_t[]
-┃   ┣━━ 🍃 fTracks.fYlast Float16_t[]
-┃   ┣━━ 🍃 fTracks.fZfirst Float16_t[]
-┃   ┣━━ 🍃 fTracks.fZlast Float16_t[]
-┃   ┣━━ 🍁 fTriggerBits TBits
-┃   ┣━━ 🍁 fTriggerBits.TObject (group of fTriggerBits.fUniqueID:uint32_t, fTriggerBits.fBits:uint8_t)
-┃   ┣━━ 🍁 fTriggerBits.fBits uint8_t
-┃   ┣━━ 🍁 fTriggerBits.fUniqueID uint32_t
-┃   ┣━━ 🍃 fTriggerBits.fAllBits uint8_t[]
-┃   ┣━━ 🍁 fTriggerBits.fNbits uint32_t
-┃   ┣━━ 🍁 fTriggerBits.fNbytes uint32_t
-┃   ┣━━ 🍁 fType[20] int8_t[20]
-┃   ┗━━ 🍁 fWebHistogram TRef
+┃   ┗━━ 🌿 event Event
+┃       ┣━━ 🌿 TObject (group of fUniqueID:uint32_t, fBits:uint32_t)
+┃       ┃   ┣━━ 🍁 fBits uint32_t
+┃       ┃   ┗━━ 🍁 fUniqueID uint32_t
+┃       ┣━━ 🍁 fClosestDistance unknown[]
+┃       ┣━━ 🍁 fEventName char*
+┃       ┣━━ 🌿 fEvtHdr EventHeader
+┃       ┃   ┣━━ 🍁 fEvtHdr.fDate int32_t
+┃       ┃   ┣━━ 🍁 fEvtHdr.fEvtNum int32_t
+┃       ┃   ┗━━ 🍁 fEvtHdr.fRun int32_t
+┃       ┣━━ 🍁 fFlag uint32_t
+┃       ┣━━ 🍁 fH TH1F
+┃       ┣━━ 🍁 fHighPt TRefArray*
+┃       ┣━━ 🍁 fIsValid bool
+┃       ┣━━ 🍁 fLastTrack TRef
+┃       ┣━━ 🍁 fMatrix[4][4] float[4][4]
+┃       ┣━━ 🍁 fMeasures[10] int32_t[10]
+┃       ┣━━ 🍁 fMuons TRefArray*
+┃       ┣━━ 🍁 fNseg int32_t
+┃       ┣━━ 🍁 fNtrack int32_t
+┃       ┣━━ 🍁 fNvertex uint32_t
+┃       ┣━━ 🍁 fTemperature float
+┃       ┣━━ 🌿 fTracks TClonesArray*
+┃       ┃   ┣━━ 🍃 fTracks.fBits uint32_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fBx Float16_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fBy Float16_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fCharge Double32_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fMass2 Float16_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fMeanCharge float[]
+┃       ┃   ┣━━ 🍃 fTracks.fNpoint int32_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fNsp uint32_t[]
+┃       ┃   ┣━━ 🍁 fTracks.fPointValue unknown[][]
+┃       ┃   ┣━━ 🍃 fTracks.fPx float[]
+┃       ┃   ┣━━ 🍃 fTracks.fPy float[]
+┃       ┃   ┣━━ 🍃 fTracks.fPz float[]
+┃       ┃   ┣━━ 🍃 fTracks.fRandom float[]
+┃       ┃   ┣━━ 🍃 fTracks.fTArray[3] float[][3]
+┃       ┃   ┣━━ 🍁 fTracks.fTriggerBits.fAllBits uint8_t[][]
+┃       ┃   ┣━━ 🍃 fTracks.fTriggerBits.fBits uint32_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fTriggerBits.fNbits uint32_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fTriggerBits.fNbytes uint32_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fTriggerBits.fUniqueID uint32_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fUniqueID uint32_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fValid int16_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fVertex[3] Double32_t[][3]
+┃       ┃   ┣━━ 🍃 fTracks.fXfirst Float16_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fXlast Float16_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fYfirst Float16_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fYlast Float16_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fZfirst Float16_t[]
+┃       ┃   ┗━━ 🍃 fTracks.fZlast Float16_t[]
+┃       ┣━━ 🌿 fTriggerBits TBits
+┃       ┃   ┣━━ 🌿 fTriggerBits.TObject (group of fTriggerBits.fUniqueID:uint32_t, fTriggerBits.fBits:uint32_t)
+┃       ┃   ┃   ┣━━ 🍁 fTriggerBits.fBits uint32_t
+┃       ┃   ┃   ┗━━ 🍁 fTriggerBits.fUniqueID uint32_t
+┃       ┃   ┣━━ 🍃 fTriggerBits.fAllBits uint8_t[]
+┃       ┃   ┣━━ 🍁 fTriggerBits.fNbits uint32_t
+┃       ┃   ┗━━ 🍁 fTriggerBits.fNbytes uint32_t
+┃       ┣━━ 🍁 fType[20] int8_t[20]
+┃       ┗━━ 🍁 fWebHistogram TRef
 ┣━━ 📊 hstat TH1F (100)
 ┗━━ 📊 htime TH1F (10)
 ```
 
 ## Development
 
 [![pre-commit.ci status][pre-commit-badge]][pre-commit-link]
```

### Comparing `uproot_browser-0.4.2/pyproject.toml` & `uproot_browser-0.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -27,29 +27,30 @@
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
-  "Development Status :: 2 - Pre-Alpha",
+  "Development Status :: 4 - Beta",
   "Typing :: Typed",
 ]
 
 dynamic = ["version"]
 dependencies = [
   "awkward >=1",
   "click >=8",
   "lz4",
   "numpy >=1.13.3",
   "rich >=12.0.0",
   "uproot >=4.2.1",
   "plotext >=5.2.2",
   "hist >=2.4",
-  "textual >=0.1.17,<0.2.0",
+  "textual >=0.18.0",
+  'typing_extensions; python_version<"3.8"'
 ]
 
 [project.optional-dependencies]
 test = [
   "pytest >=6",
   "scikit-hep-testdata",
 ]
@@ -112,15 +113,16 @@
   "design",
   "invalid-name",
   "line-too-long",
   "missing-class-docstring",
   "missing-function-docstring",
   "missing-module-docstring",
   "duplicate-code",
-  "unused-argument",  # Handed by Ruff
+  "unused-argument",  # Handled by Ruff
+  "wrong-import-position",  # Handled by Ruff
 ]
 
 [tool.ruff]
 select = [
   "E", "F", "W", # flake8
   "B", "B904",   # flake8-bugbear
   "I",           # isort
```

### Comparing `uproot_browser-0.4.2/PKG-INFO` & `uproot_browser-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uproot_browser
-Version: 0.4.2
+Version: 0.5.0
 Summary: Tools to inspect ROOT files with uproot
 Project-URL: homepage, https://github.com/scikit-hep/uproot-browser
 Project-URL: repository, https://github.com/scikit-hep/uproot-browser
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 Maintainer-email: The Scikit-HEP admins <scikit-hep-admins@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -32,15 +32,15 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -54,15 +54,16 @@
 Requires-Dist: awkward>=1
 Requires-Dist: click>=8
 Requires-Dist: hist>=2.4
 Requires-Dist: lz4
 Requires-Dist: numpy>=1.13.3
 Requires-Dist: plotext>=5.2.2
 Requires-Dist: rich>=12.0.0
-Requires-Dist: textual<0.2.0,>=0.1.17
+Requires-Dist: textual>=0.18.0
+Requires-Dist: typing-extensions; python_version < '3.8'
 Requires-Dist: uproot>=4.2.1
 Provides-Extra: dev
 Requires-Dist: ipython>=6; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
 Requires-Dist: scikit-hep-testdata; extra == 'dev'
 Provides-Extra: iterm
 Requires-Dist: itermplot==0.5; extra == 'iterm'
@@ -174,74 +175,74 @@
 **`tree` command:**
 
 ```bash
 uproot-browser tree ../scikit-hep-testdata/src/skhep_testdata/data/uproot-Event.root
 📁 uproot-Event.root
 ┣━━ ❓ <unnamed> TProcessID
 ┣━━ 🌴 T (1000)
-┃   ┣━━ 🍁 event Event
-┃   ┣━━ 🍁 TObject (group of fUniqueID:uint32_t, fBits:uint8_t)
-┃   ┣━━ 🍁 fBits uint8_t
-┃   ┣━━ 🍁 fUniqueID uint32_t
-┃   ┣━━ 🍁 fClosestDistance unknown[]
-┃   ┣━━ 🍁 fEventName char*
-┃   ┣━━ 🍁 fEvtHdr EventHeader
-┃   ┣━━ 🍁 fEvtHdr.fDate int32_t
-┃   ┣━━ 🍁 fEvtHdr.fEvtNum int32_t
-┃   ┣━━ 🍁 fEvtHdr.fRun int32_t
-┃   ┣━━ 🍁 fFlag uint32_t
-┃   ┣━━ 🍁 fH TH1F
-┃   ┣━━ 🍁 fHighPt TRefArray*
-┃   ┣━━ 🍁 fIsValid bool
-┃   ┣━━ 🍁 fLastTrack TRef
-┃   ┣━━ 🍁 fMatrix[4][4] float[4][4]
-┃   ┣━━ 🍁 fMeasures[10] int32_t[10]
-┃   ┣━━ 🍁 fMuons TRefArray*
-┃   ┣━━ 🍁 fNseg int32_t
-┃   ┣━━ 🍁 fNtrack int32_t
-┃   ┣━━ 🍁 fNvertex uint32_t
-┃   ┣━━ 🍁 fTemperature float
-┃   ┣━━ 🍁 fTracks TClonesArray*
-┃   ┣━━ 🍃 fTracks.fBits uint8_t[]
-┃   ┣━━ 🍃 fTracks.fBx Float16_t[]
-┃   ┣━━ 🍃 fTracks.fBy Float16_t[]
-┃   ┣━━ 🍃 fTracks.fCharge Double32_t[]
-┃   ┣━━ 🍃 fTracks.fMass2 Float16_t[]
-┃   ┣━━ 🍃 fTracks.fMeanCharge float[]
-┃   ┣━━ 🍃 fTracks.fNpoint int32_t[]
-┃   ┣━━ 🍃 fTracks.fNsp uint32_t[]
-┃   ┣━━ 🍁 fTracks.fPointValue unknown[][]
-┃   ┣━━ 🍃 fTracks.fPx float[]
-┃   ┣━━ 🍃 fTracks.fPy float[]
-┃   ┣━━ 🍃 fTracks.fPz float[]
-┃   ┣━━ 🍃 fTracks.fRandom float[]
-┃   ┣━━ 🍃 fTracks.fTArray[3] float[][3]
-┃   ┣━━ 🍁 fTracks.fTriggerBits.fAllBits uint8_t[][]
-┃   ┣━━ 🍃 fTracks.fTriggerBits.fBits uint8_t[]
-┃   ┣━━ 🍃 fTracks.fTriggerBits.fNbits uint32_t[]
-┃   ┣━━ 🍃 fTracks.fTriggerBits.fNbytes uint32_t[]
-┃   ┣━━ 🍃 fTracks.fTriggerBits.fUniqueID uint32_t[]
-┃   ┣━━ 🍃 fTracks.fUniqueID uint32_t[]
-┃   ┣━━ 🍃 fTracks.fValid int16_t[]
-┃   ┣━━ 🍃 fTracks.fVertex[3] Double32_t[][3]
-┃   ┣━━ 🍃 fTracks.fXfirst Float16_t[]
-┃   ┣━━ 🍃 fTracks.fXlast Float16_t[]
-┃   ┣━━ 🍃 fTracks.fYfirst Float16_t[]
-┃   ┣━━ 🍃 fTracks.fYlast Float16_t[]
-┃   ┣━━ 🍃 fTracks.fZfirst Float16_t[]
-┃   ┣━━ 🍃 fTracks.fZlast Float16_t[]
-┃   ┣━━ 🍁 fTriggerBits TBits
-┃   ┣━━ 🍁 fTriggerBits.TObject (group of fTriggerBits.fUniqueID:uint32_t, fTriggerBits.fBits:uint8_t)
-┃   ┣━━ 🍁 fTriggerBits.fBits uint8_t
-┃   ┣━━ 🍁 fTriggerBits.fUniqueID uint32_t
-┃   ┣━━ 🍃 fTriggerBits.fAllBits uint8_t[]
-┃   ┣━━ 🍁 fTriggerBits.fNbits uint32_t
-┃   ┣━━ 🍁 fTriggerBits.fNbytes uint32_t
-┃   ┣━━ 🍁 fType[20] int8_t[20]
-┃   ┗━━ 🍁 fWebHistogram TRef
+┃   ┗━━ 🌿 event Event
+┃       ┣━━ 🌿 TObject (group of fUniqueID:uint32_t, fBits:uint32_t)
+┃       ┃   ┣━━ 🍁 fBits uint32_t
+┃       ┃   ┗━━ 🍁 fUniqueID uint32_t
+┃       ┣━━ 🍁 fClosestDistance unknown[]
+┃       ┣━━ 🍁 fEventName char*
+┃       ┣━━ 🌿 fEvtHdr EventHeader
+┃       ┃   ┣━━ 🍁 fEvtHdr.fDate int32_t
+┃       ┃   ┣━━ 🍁 fEvtHdr.fEvtNum int32_t
+┃       ┃   ┗━━ 🍁 fEvtHdr.fRun int32_t
+┃       ┣━━ 🍁 fFlag uint32_t
+┃       ┣━━ 🍁 fH TH1F
+┃       ┣━━ 🍁 fHighPt TRefArray*
+┃       ┣━━ 🍁 fIsValid bool
+┃       ┣━━ 🍁 fLastTrack TRef
+┃       ┣━━ 🍁 fMatrix[4][4] float[4][4]
+┃       ┣━━ 🍁 fMeasures[10] int32_t[10]
+┃       ┣━━ 🍁 fMuons TRefArray*
+┃       ┣━━ 🍁 fNseg int32_t
+┃       ┣━━ 🍁 fNtrack int32_t
+┃       ┣━━ 🍁 fNvertex uint32_t
+┃       ┣━━ 🍁 fTemperature float
+┃       ┣━━ 🌿 fTracks TClonesArray*
+┃       ┃   ┣━━ 🍃 fTracks.fBits uint32_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fBx Float16_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fBy Float16_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fCharge Double32_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fMass2 Float16_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fMeanCharge float[]
+┃       ┃   ┣━━ 🍃 fTracks.fNpoint int32_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fNsp uint32_t[]
+┃       ┃   ┣━━ 🍁 fTracks.fPointValue unknown[][]
+┃       ┃   ┣━━ 🍃 fTracks.fPx float[]
+┃       ┃   ┣━━ 🍃 fTracks.fPy float[]
+┃       ┃   ┣━━ 🍃 fTracks.fPz float[]
+┃       ┃   ┣━━ 🍃 fTracks.fRandom float[]
+┃       ┃   ┣━━ 🍃 fTracks.fTArray[3] float[][3]
+┃       ┃   ┣━━ 🍁 fTracks.fTriggerBits.fAllBits uint8_t[][]
+┃       ┃   ┣━━ 🍃 fTracks.fTriggerBits.fBits uint32_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fTriggerBits.fNbits uint32_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fTriggerBits.fNbytes uint32_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fTriggerBits.fUniqueID uint32_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fUniqueID uint32_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fValid int16_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fVertex[3] Double32_t[][3]
+┃       ┃   ┣━━ 🍃 fTracks.fXfirst Float16_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fXlast Float16_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fYfirst Float16_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fYlast Float16_t[]
+┃       ┃   ┣━━ 🍃 fTracks.fZfirst Float16_t[]
+┃       ┃   ┗━━ 🍃 fTracks.fZlast Float16_t[]
+┃       ┣━━ 🌿 fTriggerBits TBits
+┃       ┃   ┣━━ 🌿 fTriggerBits.TObject (group of fTriggerBits.fUniqueID:uint32_t, fTriggerBits.fBits:uint32_t)
+┃       ┃   ┃   ┣━━ 🍁 fTriggerBits.fBits uint32_t
+┃       ┃   ┃   ┗━━ 🍁 fTriggerBits.fUniqueID uint32_t
+┃       ┃   ┣━━ 🍃 fTriggerBits.fAllBits uint8_t[]
+┃       ┃   ┣━━ 🍁 fTriggerBits.fNbits uint32_t
+┃       ┃   ┗━━ 🍁 fTriggerBits.fNbytes uint32_t
+┃       ┣━━ 🍁 fType[20] int8_t[20]
+┃       ┗━━ 🍁 fWebHistogram TRef
 ┣━━ 📊 hstat TH1F (100)
 ┗━━ 📊 htime TH1F (10)
 ```
 
 ## Development
 
 [![pre-commit.ci status][pre-commit-badge]][pre-commit-link]
```

