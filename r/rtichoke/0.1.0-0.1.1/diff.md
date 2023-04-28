# Comparing `tmp/rtichoke-0.1.0-py3-none-any.whl.zip` & `tmp/rtichoke-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,25 @@
-Zip file size: 10720 bytes, number of entries: 15
--rw-r--r--  2.0 fat      172 b- defN 80-Jan-01 00:00 rtichoke/__init__.py
--rw-r--r--  2.0 fat     9841 b- defN 80-Jan-01 00:00 rtichoke/calibration/calibration.py
--rw-r--r--  2.0 fat      915 b- defN 80-Jan-01 00:00 rtichoke/discrimination/gains.py
--rw-r--r--  2.0 fat      913 b- defN 80-Jan-01 00:00 rtichoke/discrimination/lift.py
--rw-r--r--  2.0 fat      847 b- defN 80-Jan-01 00:00 rtichoke/discrimination/precision_recall.py
--rw-r--r--  2.0 fat     1235 b- defN 80-Jan-01 00:00 rtichoke/discrimination/roc.py
--rw-r--r--  2.0 fat     6410 b- defN 80-Jan-01 00:00 rtichoke/helpers/exported_functions.py
--rw-r--r--  2.0 fat     3265 b- defN 80-Jan-01 00:00 rtichoke/helpers/plotly_helper_functions.py
--rw-r--r--  2.0 fat     2709 b- defN 80-Jan-01 00:00 rtichoke/helpers/send_post_request_to_r_rtichoke.py
--rw-r--r--  2.0 fat      700 b- defN 80-Jan-01 00:00 rtichoke/performance_data/performance_data.py
+Zip file size: 14878 bytes, number of entries: 23
+-rw-r--r--  2.0 fat     1045 b- defN 80-Jan-01 00:00 rtichoke/__init__.py
+-rw-r--r--  2.0 fat       38 b- defN 80-Jan-01 00:00 rtichoke/calibration/__init__.py
+-rw-r--r--  2.0 fat    10705 b- defN 80-Jan-01 00:00 rtichoke/calibration/calibration.py
+-rw-r--r--  2.0 fat       41 b- defN 80-Jan-01 00:00 rtichoke/discrimination/__init__.py
+-rw-r--r--  2.0 fat     2253 b- defN 80-Jan-01 00:00 rtichoke/discrimination/gains.py
+-rw-r--r--  2.0 fat     2246 b- defN 80-Jan-01 00:00 rtichoke/discrimination/lift.py
+-rw-r--r--  2.0 fat     2330 b- defN 80-Jan-01 00:00 rtichoke/discrimination/precision_recall.py
+-rw-r--r--  2.0 fat     2241 b- defN 80-Jan-01 00:00 rtichoke/discrimination/roc.py
+-rw-r--r--  2.0 fat       34 b- defN 80-Jan-01 00:00 rtichoke/helpers/__init__.py
+-rw-r--r--  2.0 fat     7763 b- defN 80-Jan-01 00:00 rtichoke/helpers/exported_functions.py
+-rw-r--r--  2.0 fat     3105 b- defN 80-Jan-01 00:00 rtichoke/helpers/plotly_helper_functions.py
+-rw-r--r--  2.0 fat     5736 b- defN 80-Jan-01 00:00 rtichoke/helpers/send_post_request_to_r_rtichoke.py
+-rw-r--r--  2.0 fat       43 b- defN 80-Jan-01 00:00 rtichoke/performance_data/__init__.py
+-rw-r--r--  2.0 fat     1323 b- defN 80-Jan-01 00:00 rtichoke/performance_data/performance_data.py
 -rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 rtichoke/rtichoke.py
--rw-r--r--  2.0 fat     1093 b- defN 80-Jan-01 00:00 rtichoke-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 fat     1186 b- defN 80-Jan-01 00:00 rtichoke-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 rtichoke-0.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 fat     1305 b- defN 16-Jan-01 00:00 rtichoke-0.1.0.dist-info/RECORD
-15 files, 30679 bytes uncompressed, 8530 bytes compressed:  72.2%
+-rw-r--r--  2.0 fat       41 b- defN 80-Jan-01 00:00 rtichoke/summary_report/__init__.py
+-rw-r--r--  2.0 fat      676 b- defN 80-Jan-01 00:00 rtichoke/summary_report/summary_report.py
+-rw-r--r--  2.0 fat       42 b- defN 80-Jan-01 00:00 rtichoke/utility/__init__.py
+-rw-r--r--  2.0 fat     3293 b- defN 80-Jan-01 00:00 rtichoke/utility/decision.py
+-rw-r--r--  2.0 fat     1093 b- defN 80-Jan-01 00:00 rtichoke-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 fat      755 b- defN 80-Jan-01 00:00 rtichoke-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 rtichoke-0.1.1.dist-info/WHEEL
+?rw-r--r--  2.0 fat     2017 b- defN 16-Jan-01 00:00 rtichoke-0.1.1.dist-info/RECORD
+23 files, 46908 bytes uncompressed, 11552 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -1,46 +1,70 @@
 Filename: rtichoke/__init__.py
 Comment: 
 
+Filename: rtichoke/calibration/__init__.py
+Comment: 
+
 Filename: rtichoke/calibration/calibration.py
 Comment: 
 
+Filename: rtichoke/discrimination/__init__.py
+Comment: 
+
 Filename: rtichoke/discrimination/gains.py
 Comment: 
 
 Filename: rtichoke/discrimination/lift.py
 Comment: 
 
 Filename: rtichoke/discrimination/precision_recall.py
 Comment: 
 
 Filename: rtichoke/discrimination/roc.py
 Comment: 
 
+Filename: rtichoke/helpers/__init__.py
+Comment: 
+
 Filename: rtichoke/helpers/exported_functions.py
 Comment: 
 
 Filename: rtichoke/helpers/plotly_helper_functions.py
 Comment: 
 
 Filename: rtichoke/helpers/send_post_request_to_r_rtichoke.py
 Comment: 
 
+Filename: rtichoke/performance_data/__init__.py
+Comment: 
+
 Filename: rtichoke/performance_data/performance_data.py
 Comment: 
 
 Filename: rtichoke/rtichoke.py
 Comment: 
 
-Filename: rtichoke-0.1.0.dist-info/LICENSE
+Filename: rtichoke/summary_report/__init__.py
+Comment: 
+
+Filename: rtichoke/summary_report/summary_report.py
+Comment: 
+
+Filename: rtichoke/utility/__init__.py
+Comment: 
+
+Filename: rtichoke/utility/decision.py
+Comment: 
+
+Filename: rtichoke-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: rtichoke-0.1.0.dist-info/METADATA
+Filename: rtichoke-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: rtichoke-0.1.0.dist-info/WHEEL
+Filename: rtichoke-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: rtichoke-0.1.0.dist-info/RECORD
+Filename: rtichoke-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rtichoke/__init__.py

```diff
@@ -1,4 +1,27 @@
-# read version from installed package
+"""rtichoke is a package for interactive vizualization of performance metrics
+"""
+
 from importlib.metadata import version
+
 __version__ = version("rtichoke")
+
 from rtichoke.discrimination.roc import create_roc_curve
+from rtichoke.discrimination.roc import plot_roc_curve
+
+from rtichoke.discrimination.lift import create_lift_curve
+from rtichoke.discrimination.lift import plot_lift_curve
+
+from rtichoke.discrimination.precision_recall import create_precision_recall_curve
+from rtichoke.discrimination.precision_recall import plot_precision_recall_curve
+
+from rtichoke.discrimination.gains import create_gains_curve
+from rtichoke.discrimination.gains import plot_gains_curve
+
+from rtichoke.calibration.calibration import create_calibration_curve
+
+from rtichoke.utility.decision import create_decision_curve
+from rtichoke.utility.decision import plot_decision_curve
+
+from rtichoke.performance_data.performance_data import prepare_performance_data
+
+from rtichoke.summary_report.summary_report import create_summary_report
```

## rtichoke/calibration/calibration.py

```diff
@@ -1,57 +1,76 @@
-from rtichoke.rtichoke_curves.send_post_request_to_r_rtichoke import (
-    send_requests_to_rtichoke_r,
-)
-import plotly.express as px
+"""
+A module for Calibration Curves
+"""
+
+from typing import Any, Dict, List, Optional
 import pandas as pd
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
+from plotly.graph_objs._figure import Figure
+from rtichoke.helpers.send_post_request_to_r_rtichoke import send_requests_to_rtichoke_r
 
 
 def create_calibration_curve(
-    probs,
-    reals,
-    type="discrete",
-    size=None,
-    color_values=[
-        "#1b9e77",
-        "#d95f02",
-        "#7570b3",
-        "#e7298a",
-        "#07004D",
-        "#E6AB02",
-        "#FE5F55",
-        "#54494B",
-        "#006E90",
-        "#BC96E6",
-        "#52050A",
-        "#1F271B",
-        "#BE7C4D",
-        "#63768D",
-        "#08A045",
-        "#320A28",
-        "#82FF9E",
-        "#2176FF",
-        "#D1603D",
-        "#585123",
-    ],
-    url_api="http://localhost:4242/",
-):
-    r = send_requests_to_rtichoke_r(
+    probs: Dict[str, List[float]],
+    reals: Dict[str, List[int]],
+    calibration_type: str = "discrete",
+    size: Optional[int] = None,
+    color_values: List[str] = None,
+    url_api: str = "http://localhost:4242/",
+) -> Figure:
+    """Creates Calibration Curve
+
+    Args:
+        probs (Dict[str, List[float]]): _description_
+        reals (Dict[str, List[int]]): _description_
+        calibration_type (str, optional): _description_. Defaults to "discrete".
+        size (Optional[int], optional): _description_. Defaults to None.
+        color_values (List[str], optional): _description_. Defaults to None.
+        url_api (_type_, optional): _description_. Defaults to "http://localhost:4242/".
+
+    Returns:
+        Figure: _description_
+    """
+    if color_values is None:
+        color_values = [
+            "#1b9e77",
+            "#d95f02",
+            "#7570b3",
+            "#e7298a",
+            "#07004D",
+            "#E6AB02",
+            "#FE5F55",
+            "#54494B",
+            "#006E90",
+            "#BC96E6",
+            "#52050A",
+            "#1F271B",
+            "#BE7C4D",
+            "#63768D",
+            "#08A045",
+            "#320A28",
+            "#82FF9E",
+            "#2176FF",
+            "#D1603D",
+            "#585123",
+        ]
+
+    rtichoke_response = send_requests_to_rtichoke_r(
         dictionary_to_send={
             "probs": probs,
             "reals": reals,
             "size": size,
             "color_values ": color_values,
         },
         url_api=url_api,
         endpoint="create_calibration_curve_list",
     )
 
-    calibration_curve_list = r.json()
+    calibration_curve_list = rtichoke_response.json()
 
     calibration_curve_list["deciles_dat"] = pd.DataFrame.from_dict(
         calibration_curve_list["deciles_dat"]
     )
     calibration_curve_list["smooth_dat"] = pd.DataFrame.from_dict(
         calibration_curve_list["smooth_dat"]
     )
@@ -59,48 +78,32 @@
         calibration_curve_list["reference_data"]
     )
     calibration_curve_list["histogram_for_calibration"] = pd.DataFrame.from_dict(
         calibration_curve_list["histogram_for_calibration"]
     )
 
     calibration_curve = create_plotly_curve_from_calibration_curve_list(
-        calibration_curve_list=calibration_curve_list, type=type
+        calibration_curve_list=calibration_curve_list, calibration_type=calibration_type
     )
 
     return calibration_curve
 
 
 def create_plotly_curve_from_calibration_curve_list(
-    calibration_curve_list,
-    type="discrete",
-    size=None,
-    color_values=[
-        "#1b9e77",
-        "#d95f02",
-        "#7570b3",
-        "#e7298a",
-        "#07004D",
-        "#E6AB02",
-        "#FE5F55",
-        "#54494B",
-        "#006E90",
-        "#BC96E6",
-        "#52050A",
-        "#1F271B",
-        "#BE7C4D",
-        "#63768D",
-        "#08A045",
-        "#320A28",
-        "#82FF9E",
-        "#2176FF",
-        "#D1603D",
-        "#585123",
-    ],
-):
-
+    calibration_curve_list: Dict[str, Any], calibration_type: str = "discrete"
+) -> Figure:
+    """Create plotly curve from calibration curve list
+
+    Args:
+        calibration_curve_list (Dict[str, Any]): _description_
+        calibration_type (str, optional): _description_. Defaults to "discrete".
+
+    Returns:
+        Figure: _description_
+    """
     calibration_curve = make_subplots(
         rows=2, cols=1, shared_xaxes=True, x_title="Predicted", row_heights=[0.8, 0.2]
     )
 
     calibration_curve.update_layout(
         {
             "xaxis": {"showgrid": False},
@@ -123,33 +126,33 @@
         go.Scatter(
             x=calibration_curve_list["reference_data"]["x"].values.tolist(),
             y=calibration_curve_list["reference_data"]["y"].values.tolist(),
             hovertext=calibration_curve_list["reference_data"]["text"].values.tolist(),
             name="Perfectly Calibrated",
             legendgroup="Perfectly Calibrated",
             hoverinfo="text",
-            line=dict(
-                width=2,
-                dash="dot",
-                color=calibration_curve_list["group_colors_vec"]["reference_line"][0],
-            ),
+            line={
+                "width": 2,
+                "dash": "dot",
+                "color": calibration_curve_list["group_colors_vec"]["reference_line"][
+                    0
+                ],
+            },
             showlegend=False,
         ),
         row=1,
         col=1,
     )
 
-    if type == "discrete":
-
+    if calibration_type == "discrete":
         for reference_group in list(calibration_curve_list["group_colors_vec"].keys()):
             if any(
                 calibration_curve_list["deciles_dat"]["reference_group"]
                 == reference_group
             ):
-
                 calibration_curve.add_trace(
                     go.Scatter(
                         x=calibration_curve_list["deciles_dat"]["x"][
                             calibration_curve_list["deciles_dat"]["reference_group"]
                             == reference_group
                         ].values.tolist(),
                         y=calibration_curve_list["deciles_dat"]["y"][
@@ -160,33 +163,31 @@
                             calibration_curve_list["deciles_dat"]["reference_group"]
                             == reference_group
                         ].values.tolist(),
                         name=reference_group,
                         legendgroup=reference_group,
                         hoverinfo="text",
                         mode="lines+markers",
-                        marker=dict(
-                            size=10,
-                            color=calibration_curve_list["group_colors_vec"][
+                        marker={
+                            "size": 10,
+                            "color": calibration_curve_list["group_colors_vec"][
                                 reference_group
                             ][0],
-                        ),
+                        },
                     ),
                     row=1,
                     col=1,
                 )
 
-    if type == "smooth":
-
+    if calibration_type == "smooth":
         for reference_group in list(calibration_curve_list["group_colors_vec"].keys()):
             if any(
                 calibration_curve_list["smooth_dat"]["reference_group"]
                 == reference_group
             ):
-
                 calibration_curve.add_trace(
                     go.Scatter(
                         x=calibration_curve_list["smooth_dat"]["x"][
                             calibration_curve_list["smooth_dat"]["reference_group"]
                             == reference_group
                         ].values.tolist(),
                         y=calibration_curve_list["smooth_dat"]["y"][
@@ -197,31 +198,30 @@
                             calibration_curve_list["smooth_dat"]["reference_group"]
                             == reference_group
                         ].values.tolist(),
                         name=reference_group,
                         legendgroup=reference_group,
                         hoverinfo="text",
                         mode="lines",
-                        marker=dict(
-                            size=10,
-                            color=calibration_curve_list["group_colors_vec"][
+                        marker={
+                            "size": 10,
+                            "color": calibration_curve_list["group_colors_vec"][
                                 reference_group
                             ][0],
-                        ),
+                        },
                     ),
                     row=1,
                     col=1,
                 )
 
     for reference_group in list(calibration_curve_list["group_colors_vec"].keys()):
         if any(
             calibration_curve_list["histogram_for_calibration"]["reference_group"]
             == reference_group
         ):
-
             calibration_curve.add_trace(
                 go.Bar(
                     x=calibration_curve_list["histogram_for_calibration"]["mids"][
                         calibration_curve_list["histogram_for_calibration"][
                             "reference_group"
                         ]
                         == reference_group
```

## rtichoke/discrimination/gains.py

```diff
@@ -1,19 +1,71 @@
-import requests
-import pandas as pd
-from rtichoke.rtichoke_curves.exported_functions import create_plotly_curve
-from rtichoke.rtichoke_curves.send_post_request_to_r_rtichoke import create_rtichoke_curve
-
-
-def create_gains_curve(probs, reals, by = 0.01, stratified_by = "probability_threshold", size= None, color_values = ["#1b9e77", "#d95f02", "#7570b3", "#e7298a", "#07004D", "#E6AB02",
-                "#FE5F55", "#54494B", "#006E90", "#BC96E6", "#52050A", "#1F271B", "#BE7C4D",
-                "#63768D", "#08A045", "#320A28", "#82FF9E", "#2176FF", "#D1603D", "#585123"] ,url_api = "http://localhost:4242/"):
-        fig = create_rtichoke_curve(
-            probs, 
-            reals, 
-            by = by,
-            stratified_by = stratified_by,
-            size = size,
-            color_values = color_values,
-            url_api = url_api,
-            curve = "gains")
-        return fig
+"""
+A module for Gains Curves
+"""
+from typing import Dict, List, Optional
+from pandas.core.frame import DataFrame
+from plotly.graph_objs._figure import Figure
+from rtichoke.helpers.send_post_request_to_r_rtichoke import create_rtichoke_curve
+from rtichoke.helpers.send_post_request_to_r_rtichoke import plot_rtichoke_curve
+
+
+def create_gains_curve(
+    probs: Dict[str, List[float]],
+    reals: Dict[str, List[int]],
+    by: float = 0.01,
+    stratified_by: str = "probability_threshold",
+    size: Optional[int] = None,
+    color_values: List[str] = None,
+    url_api: str = "http://localhost:4242/",
+) -> Figure:
+    """Create Gains Curve
+
+    Args:
+        probs (Dict[str, List[float]]): _description_
+        reals (Dict[str, List[int]]): _description_
+        by (float, optional): _description_. Defaults to 0.01.
+        stratified_by (str, optional): _description_. Defaults to "probability_threshold".
+        size (Optional[int], optional): _description_. Defaults to None.
+        color_values (List[str], optional): _description_. Defaults to None.
+        url_api (_type_, optional): _description_. Defaults to "http://localhost:4242/".
+
+    Returns:
+        Figure: _description_
+    """
+    fig = create_rtichoke_curve(
+        probs,
+        reals,
+        by=by,
+        stratified_by=stratified_by,
+        size=size,
+        color_values=color_values,
+        url_api=url_api,
+        curve="gains",
+    )
+    return fig
+
+
+def plot_gains_curve(
+    performance_data: DataFrame,
+    size: Optional[int] = None,
+    color_values: List[str] = None,
+    url_api: str = "http://localhost:4242/",
+) -> Figure:
+    """Plot Gains Curve
+
+    Args:
+        performance_data (DataFrame): _description_
+        size (Optional[int], optional): _description_. Defaults to None.
+        color_values (List[str], optional): _description_. Defaults to None.
+        url_api (_type_, optional): _description_. Defaults to "http://localhost:4242/".
+
+    Returns:
+        Figure: _description_
+    """
+    fig = plot_rtichoke_curve(
+        performance_data,
+        size=size,
+        color_values=color_values,
+        url_api=url_api,
+        curve="gains",
+    )
+    return fig
```

## rtichoke/discrimination/lift.py

```diff
@@ -1,19 +1,71 @@
-import requests
-import pandas as pd
-from rtichoke.rtichoke_curves.exported_functions import create_plotly_curve
-from rtichoke.rtichoke_curves.send_post_request_to_r_rtichoke import create_rtichoke_curve
-
-
-def create_lift_curve(probs, reals, by = 0.01, stratified_by = "probability_threshold", size= None, color_values = ["#1b9e77", "#d95f02", "#7570b3", "#e7298a", "#07004D", "#E6AB02",
-                "#FE5F55", "#54494B", "#006E90", "#BC96E6", "#52050A", "#1F271B", "#BE7C4D",
-                "#63768D", "#08A045", "#320A28", "#82FF9E", "#2176FF", "#D1603D", "#585123"] ,url_api = "http://localhost:4242/"):
-        fig = create_rtichoke_curve(
-            probs, 
-            reals, 
-            by = by,
-            stratified_by = stratified_by,
-            size = size,
-            color_values = color_values,
-            url_api = url_api,
-            curve = "lift")
-        return fig
+"""
+A module for Lift Curves
+"""
+from typing import Dict, List, Optional
+from plotly.graph_objs._figure import Figure
+from pandas.core.frame import DataFrame
+from rtichoke.helpers.send_post_request_to_r_rtichoke import create_rtichoke_curve
+from rtichoke.helpers.send_post_request_to_r_rtichoke import plot_rtichoke_curve
+
+
+def create_lift_curve(
+    probs: Dict[str, List[float]],
+    reals: Dict[str, List[int]],
+    by: float = 0.01,
+    stratified_by: str = "probability_threshold",
+    size: Optional[int] = None,
+    color_values: List[str] = None,
+    url_api: str = "http://localhost:4242/",
+) -> Figure:
+    """Create Lift Curve
+
+    Args:
+        probs (Dict[str, List[float]]): _description_
+        reals (Dict[str, List[int]]): _description_
+        by (float, optional): _description_. Defaults to 0.01.
+        stratified_by (str, optional): _description_. Defaults to "probability_threshold".
+        size (Optional[int], optional): _description_. Defaults to None.
+        color_values (List[str], optional): _description_. Defaults to None.
+        url_api (_type_, optional): _description_. Defaults to "http://localhost:4242/".
+
+    Returns:
+        Figure: _description_
+    """
+    fig = create_rtichoke_curve(
+        probs,
+        reals,
+        by=by,
+        stratified_by=stratified_by,
+        size=size,
+        color_values=color_values,
+        url_api=url_api,
+        curve="lift",
+    )
+    return fig
+
+
+def plot_lift_curve(
+    performance_data: DataFrame,
+    size: Optional[int] = None,
+    color_values: List[str] = None,
+    url_api: str = "http://localhost:4242/",
+) -> Figure:
+    """Plot Lift Curve
+
+    Args:
+        performance_data (DataFrame): _description_
+        size (Optional[int], optional): _description_. Defaults to None.
+        color_values (List[str], optional): _description_. Defaults to None.
+        url_api (_type_, optional): _description_. Defaults to "http://localhost:4242/".
+
+    Returns:
+        Figure: _description_
+    """
+    fig = plot_rtichoke_curve(
+        performance_data,
+        size=size,
+        color_values=color_values,
+        url_api=url_api,
+        curve="lift",
+    )
+    return fig
```

## rtichoke/discrimination/precision_recall.py

```diff
@@ -1,16 +1,71 @@
-import requests
-import pandas as pd
-from rtichoke.rtichoke_curves.exported_functions import create_plotly_curve
-from rtichoke.rtichoke_curves.send_post_request_to_r_rtichoke import create_rtichoke_curve
-
-
-def create_precision_recall_curve(probs, reals, by = 0.01, stratified_by = "probability_threshold", size= None, color_values = ["#1b9e77", "#d95f02", "#7570b3", "#e7298a", "#07004D", "#E6AB02",
-                "#FE5F55", "#54494B", "#006E90", "#BC96E6", "#52050A", "#1F271B", "#BE7C4D",
-                "#63768D", "#08A045", "#320A28", "#82FF9E", "#2176FF", "#D1603D", "#585123"] ,url_api = "http://localhost:4242/"):
-        fig = create_rtichoke_curve(
-            probs, 
-            reals, 
-            stratified_by = stratified_by,
-            url_api = url_api,
-            curve = "precision_recall")
-        return fig
+"""
+A module for Precision Recall Curves
+"""
+from typing import Dict, List, Optional
+from plotly.graph_objs._figure import Figure
+from pandas.core.frame import DataFrame
+from rtichoke.helpers.send_post_request_to_r_rtichoke import create_rtichoke_curve
+from rtichoke.helpers.send_post_request_to_r_rtichoke import plot_rtichoke_curve
+
+
+def create_precision_recall_curve(
+    probs: Dict[str, List[float]],
+    reals: Dict[str, List[int]],
+    by: float = 0.01,
+    stratified_by: str = "probability_threshold",
+    size: Optional[int] = None,
+    color_values: List[str] = None,
+    url_api: str = "http://localhost:4242/",
+) -> Figure:
+    """Create Precision Recall Curve
+
+    Args:
+        probs (Dict[str, List[float]]): _description_
+        reals (Dict[str, List[int]]): _description_
+        by (float, optional): _description_. Defaults to 0.01.
+        stratified_by (str, optional): _description_. Defaults to "probability_threshold".
+        size (Optional[int], optional): _description_. Defaults to None.
+        color_values (List[str], optional): _description_. Defaults to None.
+        url_api (_type_, optional): _description_. Defaults to "http://localhost:4242/".
+
+    Returns:
+        Figure: _description_
+    """
+    fig = create_rtichoke_curve(
+        probs,
+        reals,
+        by=by,
+        stratified_by=stratified_by,
+        size=size,
+        color_values=color_values,
+        url_api=url_api,
+        curve="precision recall",
+    )
+    return fig
+
+
+def plot_precision_recall_curve(
+    performance_data: DataFrame,
+    size: Optional[int] = None,
+    color_values: List[str] = None,
+    url_api: str = "http://localhost:4242/",
+) -> Figure:
+    """Plot Precision Recall Curve
+
+    Args:
+        performance_data (DataFrame): _description_
+        size (Optional[int], optional): _description_. Defaults to None.
+        color_values (List[str], optional): _description_. Defaults to None.
+        url_api (_type_, optional): _description_. Defaults to "http://localhost:4242/".
+
+    Returns:
+        Figure: _description_
+    """
+    fig = plot_rtichoke_curve(
+        performance_data,
+        size=size,
+        color_values=color_values,
+        url_api=url_api,
+        curve="precision recall",
+    )
+    return fig
```

## rtichoke/discrimination/roc.py

```diff
@@ -1,29 +1,72 @@
-import requests
-import pandas as pd
-from rtichoke.helpers.exported_functions import create_plotly_curve
+"""
+A module for ROC Curves
+"""
+
+from typing import Dict, List, Optional
+from plotly.graph_objs._figure import Figure
+from pandas.core.frame import DataFrame
 from rtichoke.helpers.send_post_request_to_r_rtichoke import create_rtichoke_curve
 from rtichoke.helpers.send_post_request_to_r_rtichoke import plot_rtichoke_curve
 
 
-def create_roc_curve(probs, reals, by = 0.01, stratified_by = "probability_threshold", size= None, color_values = ["#1b9e77", "#d95f02", "#7570b3", "#e7298a", "#07004D", "#E6AB02",
-                "#FE5F55", "#54494B", "#006E90", "#BC96E6", "#52050A", "#1F271B", "#BE7C4D",
-                "#63768D", "#08A045", "#320A28", "#82FF9E", "#2176FF", "#D1603D", "#585123"] ,url_api = "http://localhost:4242/"):
-        fig = create_rtichoke_curve(
-            probs, 
-            reals, 
-            by = by,
-            stratified_by = stratified_by,
-            size = size,
-            color_values = color_values,
-            url_api = url_api,
-            curve = "roc")
-        return fig
+def create_roc_curve(
+    probs: Dict[str, List[float]],
+    reals: Dict[str, List[int]],
+    by: float = 0.01,
+    stratified_by: str = "probability_threshold",
+    size: Optional[int] = None,
+    color_values: List[str] = None,
+    url_api: str = "http://localhost:4242/",
+) -> Figure:
+    """Create ROC Curve
+
+    Args:
+        probs (Dict[str, List[float]]): _description_
+        reals (Dict[str, List[int]]): _description_
+        by (float, optional): _description_. Defaults to 0.01.
+        stratified_by (str, optional): _description_. Defaults to "probability_threshold".
+        size (Optional[int], optional): _description_. Defaults to None.
+        color_values (List[str], optional): _description_. Defaults to None.
+        url_api (_type_, optional): _description_. Defaults to "http://localhost:4242/".
+
+    Returns:
+        Figure: _description_
+    """
+    fig = create_rtichoke_curve(
+        probs,
+        reals,
+        by=by,
+        stratified_by=stratified_by,
+        size=size,
+        color_values=color_values,
+        url_api=url_api,
+        curve="roc",
+    )
+    return fig
+
+
+def plot_roc_curve(
+    performance_data: DataFrame,
+    size: Optional[int] = None,
+    color_values: List[str] = None,
+    url_api: str = "http://localhost:4242/",
+) -> Figure:
+    """Plot ROC Curve
 
+    Args:
+        performance_data (DataFrame): _description_
+        size (Optional[int], optional): _description_. Defaults to None.
+        color_values (List[str], optional): _description_. Defaults to None.
+        url_api (_type_, optional): _description_. Defaults to "http://localhost:4242/".
 
-def plot_roc_curve(performance_data, size= None, url_api = "http://localhost:4242/"):
+    Returns:
+        Figure: _description_
+    """
     fig = plot_rtichoke_curve(
-            performance_data, 
-            size = size, 
-            url_api = url_api,
-            curve = "roc")
-    return fig
+        performance_data,
+        size=size,
+        color_values=color_values,
+        url_api=url_api,
+        curve="roc",
+    )
+    return fig
```

## rtichoke/helpers/exported_functions.py

```diff
@@ -1,153 +1,237 @@
+"""
+A module for Creating Plotly Curves from rtichoke curve dictionaries
+"""
+
 import plotly.graph_objects as go
-from plotly.subplots import make_subplots
 
-from rtichoke.rtichoke_curves.plotly_helper_functions import (
+from rtichoke.helpers.plotly_helper_functions import (
     create_non_interactive_curve,
     create_interactive_marker,
-    create_reference_lines_for_plotly
+    create_reference_lines_for_plotly,
 )
 
+# TODO: Fix zoom for plotly curves
+
+
 def create_plotly_curve(rtichoke_curve_dict):
     """
 
     Parameters
     ----------
     rtichoke_curve_dict :
-        
+
 
     Returns
     -------
 
     """
 
-    # reference_data, 
-    # performance_data_ready_for_curve, 
-    # group_colors_vec, 
+    # reference_data,
+    # performance_data_ready_for_curve,
+    # group_colors_vec,
     # axis_ranges
 
     reference_data_list = []
     non_interactive_curve = []
     interactive_marker = []
 
     curve_layout = {
-    "xaxis": {"showgrid": False,
-                },
-    "yaxis": {"showgrid": False},
-    "plot_bgcolor": "rgba(0, 0, 0, 0)", 
-    "showlegend": True, 
-     "legend": {
-        "orientation": "h",
-        "xanchor": "center",
-        "yanchor": "top",
-        "x": 0.5,
-        "y": 1.3
-      },
-    "height": rtichoke_curve_dict["size"][0][0],
-    "width": rtichoke_curve_dict["size"][0][0],
-    "updatemenus": [dict(type="buttons",
-                          buttons=[dict(label="Play",
-                                        method="animate",
-                                        visible = False,
-                                        args=[None, {"frame": {"duration": 500, "redraw": False}}])])]
-                                        }
+        "xaxis": {
+            "showgrid": False,
+        },
+        "yaxis": {"showgrid": False},
+        "plot_bgcolor": "rgba(0, 0, 0, 0)",
+        "showlegend": True,
+        "legend": {
+            "orientation": "h",
+            "xanchor": "center",
+            "yanchor": "top",
+            "x": 0.5,
+            "y": 1.3,
+        },
+        "height": rtichoke_curve_dict["size"][0][0],
+        "width": rtichoke_curve_dict["size"][0][0],
+        "updatemenus": [
+            {
+                "type": "buttons",
+                "buttons": [
+                    {
+                        "label": "Play",
+                        "method": "animate",
+                        "visible": False,
+                        "args": [None, {"frame": {"duration": 500, "redraw": False}}],
+                    }
+                ],
+            }
+        ],
+    }
 
     for reference_group in list(rtichoke_curve_dict["group_colors_vec"].keys()):
-
-        if (rtichoke_curve_dict["perf_dat_type"][0] not in ["several models", "several populations"]) :
+        if rtichoke_curve_dict["perf_dat_type"][0] not in [
+            "several models",
+            "several populations",
+        ]:
             interactive_marker_color = "#f6e3be"
-        else :
-            interactive_marker_color = rtichoke_curve_dict["group_colors_vec"][reference_group][0]
-        if not (rtichoke_curve_dict["reference_data"].empty) :
-            if any(rtichoke_curve_dict["reference_data"]["reference_group"] == reference_group):
+        else:
+            interactive_marker_color = rtichoke_curve_dict["group_colors_vec"][
+                reference_group
+            ][0]
+        if not rtichoke_curve_dict["reference_data"].empty:
+            if any(
+                rtichoke_curve_dict["reference_data"]["reference_group"]
+                == reference_group
+            ):
                 reference_data_list.append(
                     create_reference_lines_for_plotly(
-                    rtichoke_curve_dict["reference_data"][rtichoke_curve_dict["reference_data"]["reference_group"] == reference_group], 
-                    rtichoke_curve_dict["group_colors_vec"][reference_group][0],
-                    reference_group
-                ))
-        if any(rtichoke_curve_dict["performance_data_ready_for_curve"]["reference_group"] == reference_group):
+                        rtichoke_curve_dict["reference_data"][
+                            rtichoke_curve_dict["reference_data"]["reference_group"]
+                            == reference_group
+                        ],
+                        rtichoke_curve_dict["group_colors_vec"][reference_group][0],
+                    )
+                )
+        if any(
+            rtichoke_curve_dict["performance_data_ready_for_curve"]["reference_group"]
+            == reference_group
+        ):
             non_interactive_curve.append(
                 create_non_interactive_curve(
-                    rtichoke_curve_dict["performance_data_ready_for_curve"][rtichoke_curve_dict["performance_data_ready_for_curve"]["reference_group"] == reference_group], 
+                    rtichoke_curve_dict["performance_data_ready_for_curve"][
+                        rtichoke_curve_dict["performance_data_ready_for_curve"][
+                            "reference_group"
+                        ]
+                        == reference_group
+                    ],
                     rtichoke_curve_dict["group_colors_vec"][reference_group][0],
-                    reference_group
+                    reference_group,
                 )
             )
-        if any(rtichoke_curve_dict["performance_data_ready_for_curve"]["reference_group"] == reference_group):
+        if any(
+            rtichoke_curve_dict["performance_data_ready_for_curve"]["reference_group"]
+            == reference_group
+        ):
             interactive_marker.append(
                 create_interactive_marker(
-                    rtichoke_curve_dict["performance_data_for_interactive_marker"][rtichoke_curve_dict["performance_data_for_interactive_marker"]["reference_group"] == reference_group], 
+                    rtichoke_curve_dict["performance_data_for_interactive_marker"][
+                        rtichoke_curve_dict["performance_data_for_interactive_marker"][
+                            "reference_group"
+                        ]
+                        == reference_group
+                    ],
                     interactive_marker_color,
                     0,
-                    reference_group
+                    reference_group,
                 )
             )
 
     frames = []
 
     sliders_dict = {
-        'active': 0,
-        'yanchor': 'top',
-        'xanchor': 'left',
-        'currentvalue': {
-            'font': {'size': 20},
-            'prefix': rtichoke_curve_dict["animation_slider_prefix"][0],
-            'visible': True,
-            'xanchor': 'left'
+        "active": 0,
+        "yanchor": "top",
+        "xanchor": "left",
+        "currentvalue": {
+            "font": {"size": 20},
+            "prefix": rtichoke_curve_dict["animation_slider_prefix"][0],
+            "visible": True,
+            "xanchor": "left",
         },
-        'transition': {'duration': 300, 'easing': 'linear'},
-        'pad': {'b': 10, 't': 50},
-        'len': 0.9,
-        'x': 0.1,
-        'y': 0,
-        'steps': []
+        "transition": {"duration": 300, "easing": "linear"},
+        "pad": {"b": 10, "t": 50},
+        "len": 0.9,
+        "x": 0.1,
+        "y": 0,
+        "steps": [],
     }
 
-    for k in range(len(
-    rtichoke_curve_dict["performance_data_ready_for_curve"]["stratified_by"].unique()
-    )):
+    for k in range(
+        len(
+            rtichoke_curve_dict["performance_data_ready_for_curve"][
+                "stratified_by"
+            ].unique()
+        )
+    ):
         frame_data = reference_data_list + non_interactive_curve
         for reference_group in list(rtichoke_curve_dict["group_colors_vec"].keys()):
-            if (rtichoke_curve_dict["perf_dat_type"][0] not in ["several models", "several populations"]) :
+            if rtichoke_curve_dict["perf_dat_type"][0] not in [
+                "several models",
+                "several populations",
+            ]:
                 interactive_marker_color = "#f6e3be"
-            else :
-                interactive_marker_color = rtichoke_curve_dict["group_colors_vec"][reference_group][0]
+            else:
+                interactive_marker_color = rtichoke_curve_dict["group_colors_vec"][
+                    reference_group
+                ][0]
 
-            if any(rtichoke_curve_dict["performance_data_ready_for_curve"]["reference_group"] == reference_group):
+            if any(
+                rtichoke_curve_dict["performance_data_ready_for_curve"][
+                    "reference_group"
+                ]
+                == reference_group
+            ):
                 frame_data.append(
                     create_interactive_marker(
-                        rtichoke_curve_dict["performance_data_for_interactive_marker"][rtichoke_curve_dict["performance_data_for_interactive_marker"]["reference_group"] == reference_group], 
+                        rtichoke_curve_dict["performance_data_for_interactive_marker"][
+                            rtichoke_curve_dict[
+                                "performance_data_for_interactive_marker"
+                            ]["reference_group"]
+                            == reference_group
+                        ],
                         interactive_marker_color,
                         k,
-                        reference_group)
+                        reference_group,
                     )
-        frames.append(go.Frame(data=frame_data, name = str(k)))
-        slider_step = {'args': [
-            [k],
-            {'frame': {'duration': 300, 'redraw': False},
-            'mode': 'immediate'}
-        ],
-        'label': str(rtichoke_curve_dict["performance_data_ready_for_curve"]["stratified_by"].unique()[k]),
-        'method': 'animate'}
-        sliders_dict['steps'].append(slider_step)                                        
+                )
+        frames.append(go.Frame(data=frame_data, name=str(k)))
+        slider_step = {
+            "args": [
+                [k],
+                {"frame": {"duration": 300, "redraw": False}, "mode": "immediate"},
+            ],
+            "label": str(
+                rtichoke_curve_dict["performance_data_ready_for_curve"][
+                    "stratified_by"
+                ].unique()[k]
+            ),
+            "method": "animate",
+        }
+        sliders_dict["steps"].append(slider_step)
 
     curve_layout["sliders"] = [sliders_dict]
-    fig = go.Figure(data = reference_data_list + non_interactive_curve + interactive_marker, 
-                layout = curve_layout,
-                frames=frames)
-
-    fig.update_layout({
-          "legend": {
-          "orientation": "h",
-          "xanchor": "center",
-          "yanchor": "top",
-          "x": 0.5,
-          "y": 1.3,
-          "bgcolor": "rgba(0, 0, 0, 0)"},
-          "showlegend": rtichoke_curve_dict["perf_dat_type"][0] != "one model"})
-
-    fig.update_xaxes(zeroline=True, range = rtichoke_curve_dict["axes_ranges"]['xaxis'],
-    zerolinewidth=1, zerolinecolor='black', fixedrange=True, title=dict(text=rtichoke_curve_dict["axes_labels"]['xaxis'][0]))
-    fig.update_yaxes(zeroline=True, range = rtichoke_curve_dict["axes_ranges"]['yaxis'], 
-    zerolinewidth=1, zerolinecolor='black', fixedrange=True, title=dict(text=rtichoke_curve_dict["axes_labels"]['yaxis'][0]))
-    return fig
+    fig = go.Figure(
+        data=reference_data_list + non_interactive_curve + interactive_marker,
+        layout=curve_layout,
+        frames=frames,
+    )
+
+    fig.update_layout(
+        {
+            "legend": {
+                "orientation": "h",
+                "xanchor": "center",
+                "yanchor": "top",
+                "x": 0.5,
+                "y": 1.3,
+                "bgcolor": "rgba(0, 0, 0, 0)",
+            },
+            "showlegend": rtichoke_curve_dict["perf_dat_type"][0] != "one model",
+        }
+    )
+
+    fig.update_xaxes(
+        zeroline=True,
+        range=rtichoke_curve_dict["axes_ranges"]["xaxis"],
+        zerolinewidth=1,
+        zerolinecolor="black",
+        fixedrange=True,
+        title={"text": rtichoke_curve_dict["axes_labels"]["xaxis"][0]},
+    )
+    fig.update_yaxes(
+        zeroline=True,
+        range=rtichoke_curve_dict["axes_ranges"]["yaxis"],
+        zerolinewidth=1,
+        zerolinecolor="black",
+        fixedrange=True,
+        title={"text": rtichoke_curve_dict["axes_labels"]["yaxis"][0]},
+    )
+    return fig
```

## rtichoke/helpers/plotly_helper_functions.py

```diff
@@ -1,96 +1,114 @@
+"""
+A module for helpers related to plotly
+"""
+
 import plotly.graph_objects as go
 
-def create_non_interactive_curve(performance_data_ready_for_curve, reference_group_color, reference_group):
+
+def create_non_interactive_curve(
+    performance_data_ready_for_curve, reference_group_color, reference_group
+):
     """
 
     Parameters
     ----------
     performance_data_ready_for_curve :
-        
+
     reference_group_color :
-        
+
 
     Returns
     -------
 
     """
     performance_data_ready_for_curve = performance_data_ready_for_curve.dropna()
     # print("Print y values non interactive")
     # print(performance_data_ready_for_curve['y'].values)
     # print("Done Printing non interactive")
     print(reference_group)
     non_interactive_curve = go.Scatter(
-                x=performance_data_ready_for_curve["x"].values.tolist(),
-                y=performance_data_ready_for_curve["y"].values.tolist(),
-                mode="markers+lines",
-                hoverinfo="text",
-                hovertext=performance_data_ready_for_curve["text"].values.tolist(),
-                name = reference_group,
-                legendgroup = reference_group,
-                line=dict(width=2, color=reference_group_color))
+        x=performance_data_ready_for_curve["x"].values.tolist(),
+        y=performance_data_ready_for_curve["y"].values.tolist(),
+        mode="markers+lines",
+        hoverinfo="text",
+        hovertext=performance_data_ready_for_curve["text"].values.tolist(),
+        name=reference_group,
+        legendgroup=reference_group,
+        line={"width": 2, "color": reference_group_color},
+    )
     return non_interactive_curve
 
-def create_interactive_marker(performance_data_ready_for_curve, interactive_marker_color, k, reference_group):
+
+def create_interactive_marker(
+    performance_data_ready_for_curve, interactive_marker_color, k, reference_group
+):
     """
 
     Parameters
     ----------
     performance_data_ready_for_curve :
-        
+
     reference_group_color :
-        
+
     k :
-        
+
 
     Returns
     -------
 
     """
-    performance_data_ready_for_curve = performance_data_ready_for_curve.assign(column_name=performance_data_ready_for_curve.loc[:, "y"].fillna(-1))
-    
+    performance_data_ready_for_curve = performance_data_ready_for_curve.assign(
+        column_name=performance_data_ready_for_curve.loc[:, "y"].fillna(-1)
+    )
+
     # print("Print y values in k")
     # print(performance_data_ready_for_curve["x"].values.tolist()[k])
     # print("Done Printing")
 
     # print("Print y values")
     # print(performance_data_ready_for_curve['y'].values)
     # print("Done Printing")
 
     interactive_marker = go.Scatter(
-                x=[performance_data_ready_for_curve["x"].values.tolist()[k]],
-                y=[performance_data_ready_for_curve["y"].values.tolist()[k]],
-                mode="markers",
-                hoverinfo="text",
-                hovertext=[performance_data_ready_for_curve["text"].values.tolist()[k]],
-                name = reference_group,
-                legendgroup = reference_group,
-                showlegend=False,
-                marker=dict(size = 12, color=interactive_marker_color, line=dict(width=2, color = "black")))
+        x=[performance_data_ready_for_curve["x"].values.tolist()[k]],
+        y=[performance_data_ready_for_curve["y"].values.tolist()[k]],
+        mode="markers",
+        hoverinfo="text",
+        hovertext=[performance_data_ready_for_curve["text"].values.tolist()[k]],
+        name=reference_group,
+        legendgroup=reference_group,
+        showlegend=False,
+        marker={
+            "size": 12,
+            "color": interactive_marker_color,
+            "line": {"width": 2, "color": "black"},
+        },
+    )
     return interactive_marker
 
 
-
-def create_reference_lines_for_plotly(reference_data, reference_line_color, reference_group):
+def create_reference_lines_for_plotly(reference_data, reference_line_color):
     """Creates a plotly scatter object of the reference lines
 
     Parameters
     ----------
     reference_data :
-        
+
     reference_line_color :
-        
+
 
     Returns
     -------
 
     """
-    reference_lines = go.Scatter(x=reference_data["x"].values.tolist(), 
-                     y=reference_data["y"].values.tolist(),
-                     mode="lines",
-                     hoverinfo="text",
-                     hovertext=reference_data["text"].values.tolist(),
-                     name="reference_line",
-                     line=dict(width=2, color=reference_line_color, 
-                     dash = "dot"),
-                     showlegend=False)
+    reference_lines = go.Scatter(
+        x=reference_data["x"].values.tolist(),
+        y=reference_data["y"].values.tolist(),
+        mode="lines",
+        hoverinfo="text",
+        hovertext=reference_data["text"].values.tolist(),
+        name="reference_line",
+        line={"width": 2, "color": reference_line_color, "dash": "dot"},
+        showlegend=False,
+    )
     return reference_lines
```

## rtichoke/helpers/send_post_request_to_r_rtichoke.py

```diff
@@ -1,80 +1,195 @@
+"""
+A module for sending post requests to rtichoke r api
+"""
+
 import requests
 import pandas as pd
-from rtichoke.rtichoke_curves.exported_functions import create_plotly_curve
+from rtichoke.helpers.exported_functions import create_plotly_curve
+
+
+def send_requests_to_rtichoke_r(dictionary_to_send, url_api, endpoint):
+    """Send requests to rtichoke r
+
+    Args:
+        dictionary_to_send (_type_): _description_
+        url_api (_type_): _description_
+        endpoint (_type_): _description_
+
+    Returns:
+        _type_: _description_
+    """
+    rtichoke_response = requests.post(f"{url_api}{endpoint}", json=dictionary_to_send)
+
+    return rtichoke_response
 
-def send_requests_to_rtichoke_r(
-        dictionary_to_send,
-        url_api,
-        endpoint
-    ):
-
-    r = requests.post(
-        f"{url_api}{endpoint}",
-        json = dictionary_to_send
-        )
-    return r
 
 def create_rtichoke_curve(
-    probs, 
-    reals, 
-    by = 0.01,
-    stratified_by = "probability_threshold",
-    size=None,
-    color_values = ["#1b9e77", "#d95f02", "#7570b3", "#e7298a", "#07004D", "#E6AB02",
-    "#FE5F55", "#54494B", "#006E90", "#BC96E6", "#52050A", "#1F271B", "#BE7C4D",
-    "#63768D", "#08A045", "#320A28", "#82FF9E", "#2176FF", "#D1603D", "#585123"],
-    url_api = "http://localhost:4242/",
-    curve = "roc"):
-
-    r = send_requests_to_rtichoke_r(
-           dictionary_to_send = {
-                "probs": probs,
-                "reals": reals,
-                "by": by,
-                "stratified_by": stratified_by,
-                "size": size,
-                "color_values": color_values
-           },
-           url_api = url_api,
-           endpoint = f"create_{curve}_curve_list" 
-        )
-
-    rtichoke_curve_list = r.json()
-
-    rtichoke_curve_list["reference_data"] = pd.DataFrame.from_dict(rtichoke_curve_list["reference_data"]) 
-    rtichoke_curve_list["performance_data_ready_for_curve"] = pd.DataFrame.from_dict(rtichoke_curve_list["performance_data_ready_for_curve"]) 
-    rtichoke_curve_list["performance_data_for_interactive_marker"] = pd.DataFrame.from_dict(rtichoke_curve_list["performance_data_for_interactive_marker"]) 
+    probs,
+    reals,
+    by,
+    stratified_by,
+    size,
+    color_values=None,
+    url_api="http://localhost:4242/",
+    curve="roc",
+    min_p_threshold=0,
+    max_p_threshold=1,
+):
+    """Create rtichoke curve
+
+    Args:
+        probs (_type_): _description_
+        reals (_type_): _description_
+        by (_type_): _description_
+        stratified_by (_type_): _description_
+        size (_type_): _description_
+        color_values (_type_, optional): _description_. Defaults to None.
+        url_api (str, optional): _description_. Defaults to "http://localhost:4242/".
+        curve (str, optional): _description_. Defaults to "roc".
+        min_p_threshold (int, optional): _description_. Defaults to 0.
+        max_p_threshold (int, optional): _description_. Defaults to 1.
+
+    Returns:
+        _type_: _description_
+    """
+    if color_values is None:
+        color_values = [
+            "#1b9e77",
+            "#d95f02",
+            "#7570b3",
+            "#e7298a",
+            "#07004D",
+            "#E6AB02",
+            "#FE5F55",
+            "#54494B",
+            "#006E90",
+            "#BC96E6",
+            "#52050A",
+            "#1F271B",
+            "#BE7C4D",
+            "#63768D",
+            "#08A045",
+            "#320A28",
+            "#82FF9E",
+            "#2176FF",
+            "#D1603D",
+            "#585123",
+        ]
+
+    rtichoke_response = send_requests_to_rtichoke_r(
+        dictionary_to_send={
+            "probs": probs,
+            "reals": reals,
+            "curve": curve,
+            "by": by,
+            "stratified_by": stratified_by,
+            "size": size,
+            "color_values": color_values,
+            "min_p_threshold": min_p_threshold,
+            "max_p_threshold": max_p_threshold,
+        },
+        url_api=url_api,
+        endpoint="create_rtichoke_curve_list",
+    )
+
+    rtichoke_curve_list = rtichoke_response.json()
 
-    fig = create_plotly_curve(
-        rtichoke_curve_list
+    if rtichoke_curve_list["size"][0] is None:
+        rtichoke_curve_list["size"] = [[None]]
+
+    rtichoke_curve_list["reference_data"] = pd.DataFrame.from_dict(
+        rtichoke_curve_list["reference_data"]
+    )
+    rtichoke_curve_list["performance_data_ready_for_curve"] = pd.DataFrame.from_dict(
+        rtichoke_curve_list["performance_data_ready_for_curve"]
     )
+    rtichoke_curve_list[
+        "performance_data_for_interactive_marker"
+    ] = pd.DataFrame.from_dict(
+        rtichoke_curve_list["performance_data_for_interactive_marker"]
+    )
+
+    fig = create_plotly_curve(rtichoke_curve_list)
 
     return fig
 
+
 def plot_rtichoke_curve(
     performance_data,
-    size = None,
-    url_api = "http://localhost:4242/",
-    curve = "roc"):
-
-    r = send_requests_to_rtichoke_r(
-           dictionary_to_send = {
-            "performance_data": performance_data.to_json(orient = 'records'),
-            "size": size},
-           url_api = url_api,
-           endpoint = f"plot_{curve}_curve_list" 
-        )
-
-    rtichoke_curve_list = r.json()
+    size=None,
+    color_values=None,
+    url_api="http://localhost:4242/",
+    curve="roc",
+    min_p_threshold=0,
+    max_p_threshold=1,
+):
+    """plot rtichoke curve
+
+    Args:
+        performance_data (_type_): _description_
+        size (_type_, optional): _description_. Defaults to None.
+        color_values (_type_, optional): _description_. Defaults to None.
+        url_api (str, optional): _description_. Defaults to "http://localhost:4242/".
+        curve (str, optional): _description_. Defaults to "roc".
+        min_p_threshold (int, optional): _description_. Defaults to 0.
+        max_p_threshold (int, optional): _description_. Defaults to 1.
+
+    Returns:
+        _type_: _description_
+    """
+    if color_values is None:
+        color_values = [
+            "#1b9e77",
+            "#d95f02",
+            "#7570b3",
+            "#e7298a",
+            "#07004D",
+            "#E6AB02",
+            "#FE5F55",
+            "#54494B",
+            "#006E90",
+            "#BC96E6",
+            "#52050A",
+            "#1F271B",
+            "#BE7C4D",
+            "#63768D",
+            "#08A045",
+            "#320A28",
+            "#82FF9E",
+            "#2176FF",
+            "#D1603D",
+            "#585123",
+        ]
+    rtichoke_response = send_requests_to_rtichoke_r(
+        dictionary_to_send={
+            "performance_data": performance_data.to_json(orient="records"),
+            "curve": curve,
+            "size": size,
+            "color_values": color_values,
+            "min_p_threshold": min_p_threshold,
+            "max_p_threshold": max_p_threshold,
+        },
+        url_api=url_api,
+        endpoint="plot_rtichoke_curve_list",
+    )
 
-    rtichoke_curve_list["reference_data"] = pd.DataFrame.from_dict(rtichoke_curve_list["reference_data"]) 
-    rtichoke_curve_list["performance_data_ready_for_curve"] = pd.DataFrame.from_dict(rtichoke_curve_list["performance_data_ready_for_curve"]) 
-    rtichoke_curve_list["performance_data_for_interactive_marker"] = pd.DataFrame.from_dict(rtichoke_curve_list["performance_data_for_interactive_marker"]) 
+    rtichoke_curve_list = rtichoke_response.json()
 
-    print(rtichoke_curve_list)
+    if rtichoke_curve_list["size"][0] is None:
+        rtichoke_curve_list["size"] = [[None]]
 
-    fig = create_plotly_curve(
-        rtichoke_curve_list
+    rtichoke_curve_list["reference_data"] = pd.DataFrame.from_dict(
+        rtichoke_curve_list["reference_data"]
+    )
+    rtichoke_curve_list["performance_data_ready_for_curve"] = pd.DataFrame.from_dict(
+        rtichoke_curve_list["performance_data_ready_for_curve"]
+    )
+    rtichoke_curve_list[
+        "performance_data_for_interactive_marker"
+    ] = pd.DataFrame.from_dict(
+        rtichoke_curve_list["performance_data_for_interactive_marker"]
     )
 
-    return fig
+    fig = create_plotly_curve(rtichoke_curve_list)
+
+    return fig
```

## rtichoke/performance_data/performance_data.py

```diff
@@ -1,18 +1,41 @@
-import requests
+"""
+A module for Performance Data
+"""
+
+from typing import Dict, List
+from pandas.core.frame import DataFrame
 import pandas as pd
-from rtichoke.rtichoke_curves.send_post_request_to_r_rtichoke import send_requests_to_rtichoke_r
+from rtichoke.helpers.send_post_request_to_r_rtichoke import send_requests_to_rtichoke_r
+
+
+def prepare_performance_data(
+    probs: Dict[str, List[float]],
+    reals: Dict[str, List[int]],
+    stratified_by: str = "probability_threshold",
+    url_api: str = "http://localhost:4242/",
+) -> DataFrame:
+    """Prepare Performance Data
+
+    Args:
+        probs (Dict[str, List[float]]): _description_
+        reals (Dict[str, List[int]]): _description_
+        stratified_by (str, optional): _description_. Defaults to "probability_threshold".
+        url_api (_type_, optional): _description_. Defaults to "http://localhost:4242/".
 
-def prepare_performance_data(probs, reals, stratified_by = "probability_threshold", url_api = "http://localhost:4242/"):
-    
-    r = send_requests_to_rtichoke_r(
-           dictionary_to_send = {
-                "probs": probs,
-                "reals": reals,
-                "stratified_by": stratified_by
-           },
-           url_api = url_api,
-           endpoint = "prepare_performance_data" 
-        )
-    print(r.json()[0].keys())
-    performance_data = pd.DataFrame(r.json(), columns=list(r.json()[0].keys()))
-    return performance_data
+    Returns:
+        DataFrame: _description_
+    """
+    rtichoke_response = send_requests_to_rtichoke_r(
+        dictionary_to_send={
+            "probs": probs,
+            "reals": reals,
+            "stratified_by": stratified_by,
+        },
+        url_api=url_api,
+        endpoint="prepare_performance_data",
+    )
+    print(rtichoke_response.json()[0].keys())
+    performance_data = pd.DataFrame(
+        rtichoke_response.json(), columns=list(rtichoke_response.json()[0].keys())
+    )
+    return performance_data
```

## Comparing `rtichoke-0.1.0.dist-info/LICENSE` & `rtichoke-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

