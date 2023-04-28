# Comparing `tmp/calendar_widget-1.0.7.tar.gz` & `tmp/calendar_widget-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calendar_widget-1.0.7.tar", last modified: Thu Apr 27 17:16:31 2023, max compression
+gzip compressed data, was "calendar_widget-1.0.8.tar", last modified: Fri Apr 28 17:00:47 2023, max compression
```

## Comparing `calendar_widget-1.0.7.tar` & `calendar_widget-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 17:16:31.260429 calendar_widget-1.0.7/
--rw-rw-rw-   0        0        0    26526 2023-04-14 15:16:21.000000 calendar_widget-1.0.7/LICENSE.md
--rw-rw-rw-   0        0        0    14037 2023-04-27 17:16:31.260429 calendar_widget-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    13144 2023-04-27 17:15:12.000000 calendar_widget-1.0.7/README.md
--rw-rw-rw-   0        0        0      763 2023-04-27 17:15:39.000000 calendar_widget-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 17:16:31.260429 calendar_widget-1.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-27 17:16:31.119794 calendar_widget-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-27 17:16:31.213553 calendar_widget-1.0.7/src/calendar_widget/
--rw-rw-rw-   0        0        0   129221 2023-04-27 16:34:52.000000 calendar_widget-1.0.7/src/calendar_widget/Calendar_Widget.py
--rw-rw-rw-   0        0        0       37 2023-04-15 01:39:22.000000 calendar_widget-1.0.7/src/calendar_widget/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 17:16:31.244803 calendar_widget-1.0.7/src/calendar_widget.egg-info/
--rw-rw-rw-   0        0        0    14037 2023-04-27 17:16:31.000000 calendar_widget-1.0.7/src/calendar_widget.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-04-27 17:16:31.000000 calendar_widget-1.0.7/src/calendar_widget.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 17:16:31.000000 calendar_widget-1.0.7/src/calendar_widget.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-27 17:16:31.000000 calendar_widget-1.0.7/src/calendar_widget.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-27 17:16:31.244803 calendar_widget-1.0.7/tests/
--rw-rw-rw-   0        0        0      821 2023-04-27 16:36:43.000000 calendar_widget-1.0.7/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-04-28 17:00:47.641586 calendar_widget-1.0.8/
+-rw-rw-rw-   0        0        0    26526 2023-04-14 15:16:21.000000 calendar_widget-1.0.8/LICENSE.md
+-rw-rw-rw-   0        0        0    13646 2023-04-28 17:00:47.641586 calendar_widget-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    12753 2023-04-28 16:58:13.000000 calendar_widget-1.0.8/README.md
+-rw-rw-rw-   0        0        0      763 2023-04-28 16:59:53.000000 calendar_widget-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-28 17:00:47.641586 calendar_widget-1.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 17:00:47.546959 calendar_widget-1.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 17:00:47.609467 calendar_widget-1.0.8/src/calendar_widget/
+-rw-rw-rw-   0        0        0   129387 2023-04-28 16:58:24.000000 calendar_widget-1.0.8/src/calendar_widget/Calendar_Widget.py
+-rw-rw-rw-   0        0        0       37 2023-04-15 01:39:22.000000 calendar_widget-1.0.8/src/calendar_widget/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 17:00:47.640534 calendar_widget-1.0.8/src/calendar_widget.egg-info/
+-rw-rw-rw-   0        0        0    13646 2023-04-28 17:00:47.000000 calendar_widget-1.0.8/src/calendar_widget.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-04-28 17:00:47.000000 calendar_widget-1.0.8/src/calendar_widget.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 17:00:47.000000 calendar_widget-1.0.8/src/calendar_widget.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-28 17:00:47.000000 calendar_widget-1.0.8/src/calendar_widget.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 17:00:47.641586 calendar_widget-1.0.8/tests/
+-rw-rw-rw-   0        0        0      461 2023-04-28 16:58:42.000000 calendar_widget-1.0.8/tests/test.py
```

### Comparing `calendar_widget-1.0.7/LICENSE.md` & `calendar_widget-1.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `calendar_widget-1.0.7/PKG-INFO` & `calendar_widget-1.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calendar_widget
-Version: 1.0.7
+Version: 1.0.8
 Summary: Calendar widget for use with python tkinter
 Author-email: Spartanlasergun <bns360@live.com>
 Project-URL: Homepage, https://github.com/Spartanlasergun/calendar_widget
 Project-URL: Bug Tracker, https://github.com/Spartanlasergun/calendar_widget/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -102,15 +102,14 @@
 # define the main window into which the widget will be placed
 root = tkinter.Tk()
 root.geometry('600x600')  # the geometry function defines the size of the tkinter window
                           # - in this case, we are using a window that is 600px by 600px
 
 # create the calendar widget
 Calendar = Calendar(root, # specify the tkinter window into which the widget will be placed
-	size = 250, # set the size of the calendar widget to 250px
 	pos_x = 0, # set the x position of the calendar widget within the tkinter window
 	pos_y = 0, # set the y position of the calendar widget within the tkinter window
 	background = 'lightblue', # set the background of the calendar to light blue
 	)
 
 # Note: images of the type 'png', 'gif', 'ppm', and 'pgm' can be set as the background.
 # However, these images will not scale with the size of the calendar.
@@ -130,15 +129,14 @@
 ```python
 # the 'Calendar_Click' function retrives the date selected on the Calendar by the user, and prints the date to the console
 def Calendar_Click():
 	print(Calendar.getdate())
 
 # create the calendar widget
 Calendar = Calendar(root,
-	size = 250,
 	pos_x = 0,
 	pos_y = 0, 
 	background = 'lightblue', 
 	command = Calendar_Click  # link the 'Calendar_Click' function to the widget
 	)
 ```
 
@@ -148,55 +146,57 @@
 
 # Widget Parameters - functionality and styling
 
 The table below specifies opitons availiable for styling and other operations associated with the calendar widget
 
 | options | description |
 | ------- | ----------- |
-| size= | Sets the width of the widget in pixels. The default width is 300px. <br> Example: ``` Calendar = Calendar(root, size=350, ...) ``` |
-| pos_x= | Sets the x coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. <br> Example: ``` Calendar = Calendar(root, size=350, pos_x=0, ...) ``` |
-| pos_y= | Sets the y coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. <br> Example: ``` Calendar = Calendar(root, size=350, pos_y=0, ...) ``` |
-| style= | Set the style="Dark" for the dark theme. If no styling is specified the Calendar will inherit its default white theme. <br> Example: ``` Calendar = Calendar(root, size=350, style='Dark', ...) ``` |
-| command= | A function to be called when the widget is clicked. <br> Example: ``` Calendar = Calendar(root, command=my_function, ...) ``` |
-| background= | Sets the background of the Calendar to a valid tkinter colour or image (png, gif, ppm, pgm). <br> Example: ``` Calendar = Calendar(root, background='sky.png', ...) ``` |
-| img_pos_x= | Set the x coordinate of the background image if specified (by default, this is the top left corner). <br> Example: ``` Calendar = Calendar(root, background='sky.png', img_pos_x=0, ...) ``` |
-| img_pos_y= | Set the y coordinate of the background image if specified (by default, this is the top left corner). <br> Example: ``` Calendar = Calendar(root, background='sky.png', img_pos_y=0, ...) ``` |
-| img_anchor= | Set the anchor of the background image if specified (by default, this is set to 'nw' - the top left corner). <br> Example: ``` Calendar = Calendar(root, background='sky.png', img_pos_x=0, img_pos_y=0, img_anchor='ne', ...) ``` |
-| arrow_box_border= | Sets the border colour of the box containing the arrows for selecting previous and following months. <br> Example: ``` Calendar = Calendar(root, size=250, arrow_box_border='blue', ...) ``` |
-| arrow_box_fill= | Sets the background of the box containing the arrows for selecting previous and following months. <br> Example: ``` Calendar = Calendar(root, size=300, arrow_box_fill='red', ...) ``` |
-| arrow_box_width= | Sets the line width of the box containing the arrows for selecting previous and following months. <br> Example: ``` Calendar = Calendar(root, size=350, arrow_box_width=3, ...) ``` |
-| date_box_fill= | Sets the colour inside of the boxes that make up the monthly calendar grid. <br> Example: ``` Calendar = Calendar(root, size=300, date_box_fill='purple', ...) ``` |
-| date_box_width= | Sets the width of the line used to create the grid for the monthly calendar. <br> Example: ``` Calendar = Calendar(root, size=350, date_box_width=5, ...) ``` |
-| date_boxes_outline= | Sets the colour of the box outline for the boxes that make up the monthly claendar grid. <br> Example: ``` Calendar = Calendar(root, size=350, date_boxes_outline='lime', ...) ``` |
-| arrow_outline= | Sets the colour for the outline of the polygon (i.e - triangle) that represents the calendar arrows. <br> Example: ``` Calendar = Calendar(root, size=350, arrow_outline='lightblue' ...) ``` |
-| arrow_fill= | Sets the colour of the calendar arrows. <br> Example: ``` Calendar = Calendar(root, size=350, arrow_fill='navy', ...) ``` |
-| arrow_thickness= | Sets the thickness of the calendar arrows. <br> Example: ``` Calendar = Calendar(root, size=350, arrow_thickness=5, ...) ``` |
-| arrow_active= | Sets the colour for the active highlight when the mouse hovers over the calendar arrows. <br> Example: ``` Calendar = Calendar(root, size=350, arrow_active='magenta', ...) ``` |
-| weekday_border= | Sets the colour for the outline of the boxes that hold the weekday headings. <br> Example: ``` Calendar = Calendar(root, size=300, weekday_border='blue', ...) ``` |
-| weekday_fill= | Sets the colour for the background of the boxes that hold the weekday headings. <br> Example: ``` Calendar = Calendar(root, size=250, weekday_fill='gray', ...) ``` |
-| weekday_width= | Sets the width of the boxes that hold the weekday headings. <br> Example: ``` Calendar = Calendar(root, size=250, weekday_width=3, ...) ``` |
-| weekday_font_fill= | Sets the colour of the text associated with the weekday headings. <br> Example: ``` Calendar = Calendar(root, size=250, weekday_font_fill='red' ...) ``` |
-| weekday_font_family= | Sets the type of font used to create the weekday headings. (Accepts any of the valid native tkinter fonts). <br> Example: ``` Calendar = Calendar(root, size=250, weekday_font_family='Georgia', ...) ``` |
-| weekday_font_weight= | Sets the weight of the font used to create the weekday headings. Valid options are 'normal' or 'bold'. <br> Example: ``` Calendar = Calendar(root, size=250, weekday_font_family='bold' ...) ``` |
-| weekday_font_slant= | Sets the slant of the font used to create the weekday headings. Valid options are 'roman' or 'italic'. <br> Example: ``` Calendar = Calendar(root, size=250, weekday_font_slant='italic', ...) ``` |
-| weekday_font_underline= | Sets the underline of the font used to creates the weekday heading. Valid options are True or False. <br> Example: ``` Calendar = Calendar(root, size=250, weekday_font_underline=True, ...) ``` |
-| weekday_font_size= | Sets the font size of the weekday headings. Note: this overrides the default size and scaling of the font. <br> Example: ``` Calendar = Calendar(root, size=250, weekday_font_size=10, ...) ``` |
-| calendar_date_title= | Sets the colour of the text associated with the calendar title (ex: Aug 2020). <br> Example: ``` Calendar = Calendar(root, size=250, calendar_date_title='red', ...) ``` |
-| date_heading_font_family= | Sets the font type for the Calendar date heading. (Accepts any of the valid native tkinter fonts). <br> Example: ``` Calendar = Calendar(root, size=250, date_heading_font_family='Helvetica', ...) ``` |
-| date_heading_font_weight= | Sets the weight of the font used to create the Calendar date heading. Valid options are 'normal' or 'bold'. <br> Example: ``` Calendar = Calendar(root, size=250, date_heading_font_weight='bold', ...) ``` |
-| date_heading_font_slant= | Sets the slant of the font used to create the Calendar date heading. Valid options are 'roman' or 'italic'. <br> Example: ``` Calendar = Calendar(root, size=250, date_heading_font_slant='italic', ...) ``` |
-| date_heading_font_underline= | Sets the underline of the font used to create the Calendar date heading. Valid options are True or False. <br> Example: ``` Calendar = Calendar(root, size=250, date_heading_font_underline=True, ...) ``` |
-| date_heading_font_size= | Sets the font size used to create the Calendar heading. Note: This overrides the default size and scaling of the font. <br> Example: ``` Calendar = Calendar(root, size=250, date_heading_font_size=15 ...) ``` |
-| date_text_fill= | Sets the colour of the text numbers associated with the month dates. <br> Example: ``` Calendar = Calendar(root, size=250, date_text_fill='green', ...) ``` |
-| date_text_font_family= | Sets the font type used to create the month dates. (Accepts any of the valid native tkinter fonts). <br> Example: ``` Calendar = Calendar(root, size=250, date_text_font_family='Georgia', ...) ``` |
-| date_text_font_weight= | Sets the weight of the font used to create the month dates. Valid options are 'normal' or 'bold'. <br> Example: ``` Calendar = Calendar(root, size=250, date_text_font_weight='bold', ...) ``` |
-| date_text_font_slant= | Sets the slant of the font used to create the month dates. Valid options are 'roman' or 'italic'. <br> Example: ``` Calendar = Calendar(root, size=250, date_text_font_slant='italic', ...) ``` |
-| date_text_font_underline= | Sets the underline of the font used to create the month dates. Valid options are True or False. <br> Example: ``` Calendar = Calendar(root, size=250, date_text_font_underline=True, ...) ``` |
-| date_text_font_size= | Sets the font size of the dates on the Calendar month grid. Note: this overrides the default size and scaling of the font. <br> Example: ``` Calendar = Calendar(root, size=250, date_text_font_size=10, ...) ``` |
-| trail_box_fill= | Sets the colour of the background of the date boxes that trail into the previous and following months. <br> Example: ``` Calendar = Calendar(root, size=250, trail_box_fill='lime', ...) ``` |
-| trail_text_fill= | Sets the colour of the text numbers associated with the trailing date boxes. <br> Example: ``` Calendar = Calendar(root, size=250, trail_text_fill='blue' ...) ``` |
+| width= | Sets the width of the widget in pixels. The default width is 300px. <br> Example: ``` Calendar = Calendar(root, width=350) ``` |
+| height= | Sets the height of the widget in pixels. The default height is 200px. <br> Example: ``` Calendar = Calendar(root, height=200) ``` |
+| padding= | Sets the internal padding of the calendar widget. The default padding is set to 10px. <br> Example: ``` Calendar = Calendar(root, padding=15) ```
+| pos_x= | Sets the x coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. <br> Example: ``` Calendar = Calendar(root, pos_x=0) ``` |
+| pos_y= | Sets the y coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. <br> Example: ``` Calendar = Calendar(root, pos_y=0) ``` |
+| style= | Set the style="Dark" for the dark theme. If no styling is specified the Calendar will inherit its default white theme. <br> Example: ``` Calendar = Calendar(root, style='Dark') ``` |
+| command= | A function to be called when the widget is clicked. <br> Example: ``` Calendar = Calendar(root, command=my_function) ``` |
+| background= | Sets the background of the Calendar to a valid tkinter colour or image (png, gif, ppm, pgm). <br> Example: ``` Calendar = Calendar(root, background='sky.png') ``` |
+| img_pos_x= | Set the x coordinate of the background image if specified (by default, this is the top left corner). <br> Example: ``` Calendar = Calendar(root, background='sky.png', img_pos_x=0) ``` |
+| img_pos_y= | Set the y coordinate of the background image if specified (by default, this is the top left corner). <br> Example: ``` Calendar = Calendar(root, background='sky.png', img_pos_y=0) ``` |
+| img_anchor= | Set the anchor of the background image if specified (by default, this is set to 'nw' - the top left corner). <br> Example: ``` Calendar = Calendar(root, background='sky.png', img_pos_x=0, img_pos_y=0, img_anchor='ne') ``` |
+| arrow_box_border= | Sets the border colour of the box containing the arrows for selecting previous and following months. <br> Example: ``` Calendar = Calendar(root, arrow_box_border='blue') ``` |
+| arrow_box_fill= | Sets the background of the box containing the arrows for selecting previous and following months. <br> Example: ``` Calendar = Calendar(root, arrow_box_fill='red') ``` |
+| arrow_box_width= | Sets the line width of the box containing the arrows for selecting previous and following months. <br> Example: ``` Calendar = Calendar(root, arrow_box_width=3) ``` |
+| date_box_fill= | Sets the colour inside of the boxes that make up the monthly calendar grid. <br> Example: ``` Calendar = Calendar(root, date_box_fill='purple') ``` |
+| date_box_width= | Sets the width of the line used to create the grid for the monthly calendar. <br> Example: ``` Calendar = Calendar(root, date_box_width=5) ``` |
+| date_boxes_outline= | Sets the colour of the box outline for the boxes that make up the monthly claendar grid. <br> Example: ``` Calendar = Calendar(root, date_boxes_outline='lime') ``` |
+| arrow_outline= | Sets the colour for the outline of the polygon (i.e - triangle) that represents the calendar arrows. <br> Example: ``` Calendar = Calendar(root, arrow_outline='lightblue') ``` |
+| arrow_fill= | Sets the colour of the calendar arrows. <br> Example: ``` Calendar = Calendar(root, arrow_fill='navy') ``` |
+| arrow_thickness= | Sets the thickness of the calendar arrows. <br> Example: ``` Calendar = Calendar(root, arrow_thickness=5) ``` |
+| arrow_active= | Sets the colour for the active highlight when the mouse hovers over the calendar arrows. <br> Example: ``` Calendar = Calendar(root, arrow_active='magenta') ``` |
+| weekday_border= | Sets the colour for the outline of the boxes that hold the weekday headings. <br> Example: ``` Calendar = Calendar(root, weekday_border='blue') ``` |
+| weekday_fill= | Sets the colour for the background of the boxes that hold the weekday headings. <br> Example: ``` Calendar = Calendar(root, weekday_fill='gray') ``` |
+| weekday_width= | Sets the width of the boxes that hold the weekday headings. <br> Example: ``` Calendar = Calendar(root, weekday_width=3) ``` |
+| weekday_font_fill= | Sets the colour of the text associated with the weekday headings. <br> Example: ``` Calendar = Calendar(root, weekday_font_fill='red') ``` |
+| weekday_font_family= | Sets the type of font used to create the weekday headings. (Accepts any of the valid native tkinter fonts). <br> Example: ``` Calendar = Calendar(root, weekday_font_family='Georgia') ``` |
+| weekday_font_weight= | Sets the weight of the font used to create the weekday headings. Valid options are 'normal' or 'bold'. <br> Example: ``` Calendar = Calendar(root, weekday_font_family='bold') ``` |
+| weekday_font_slant= | Sets the slant of the font used to create the weekday headings. Valid options are 'roman' or 'italic'. <br> Example: ``` Calendar = Calendar(root, weekday_font_slant='italic') ``` |
+| weekday_font_underline= | Sets the underline of the font used to creates the weekday heading. Valid options are True or False. <br> Example: ``` Calendar = Calendar(root, weekday_font_underline=True) ``` |
+| weekday_font_size= | Sets the font size of the weekday headings. Note: this overrides the default size and scaling of the font. <br> Example: ``` Calendar = Calendar(root, weekday_font_size=10) ``` |
+| calendar_date_title= | Sets the colour of the text associated with the calendar title (ex: Aug 2020). <br> Example: ``` Calendar = Calendar(root, calendar_date_title='red') ``` |
+| date_heading_font_family= | Sets the font type for the Calendar date heading. (Accepts any of the valid native tkinter fonts). <br> Example: ``` Calendar = Calendar(root, date_heading_font_family='Helvetica') ``` |
+| date_heading_font_weight= | Sets the weight of the font used to create the Calendar date heading. Valid options are 'normal' or 'bold'. <br> Example: ``` Calendar = Calendar(root, date_heading_font_weight='bold') ``` |
+| date_heading_font_slant= | Sets the slant of the font used to create the Calendar date heading. Valid options are 'roman' or 'italic'. <br> Example: ``` Calendar = Calendar(root, date_heading_font_slant='italic') ``` |
+| date_heading_font_underline= | Sets the underline of the font used to create the Calendar date heading. Valid options are True or False. <br> Example: ``` Calendar = Calendar(root, date_heading_font_underline=True) ``` |
+| date_heading_font_size= | Sets the font size used to create the Calendar heading. Note: This overrides the default size and scaling of the font. <br> Example: ``` Calendar = Calendar(root, date_heading_font_size=15) ``` |
+| date_text_fill= | Sets the colour of the text numbers associated with the month dates. <br> Example: ``` Calendar = Calendar(root, date_text_fill='green') ``` |
+| date_text_font_family= | Sets the font type used to create the month dates. (Accepts any of the valid native tkinter fonts). <br> Example: ``` Calendar = Calendar(root, date_text_font_family='Georgia') ``` |
+| date_text_font_weight= | Sets the weight of the font used to create the month dates. Valid options are 'normal' or 'bold'. <br> Example: ``` Calendar = Calendar(root, date_text_font_weight='bold') ``` |
+| date_text_font_slant= | Sets the slant of the font used to create the month dates. Valid options are 'roman' or 'italic'. <br> Example: ``` Calendar = Calendar(root, date_text_font_slant='italic') ``` |
+| date_text_font_underline= | Sets the underline of the font used to create the month dates. Valid options are True or False. <br> Example: ``` Calendar = Calendar(root, date_text_font_underline=True) ``` |
+| date_text_font_size= | Sets the font size of the dates on the Calendar month grid. Note: this overrides the default size and scaling of the font. <br> Example: ``` Calendar = Calendar(root, date_text_font_size=10) ``` |
+| trail_box_fill= | Sets the colour of the background of the date boxes that trail into the previous and following months. <br> Example: ``` Calendar = Calendar(root, trail_box_fill='lime') ``` |
+| trail_text_fill= | Sets the colour of the text numbers associated with the trailing date boxes. <br> Example: ``` Calendar = Calendar(root, trail_text_fill='blue') ``` |
 | current_date_highlight= | Toggles the current date highlight on/off. This parameter accepts a True or False value. Example: ``` Calendar = Calendar(root, current_date_highlight=False) ``` |
-| date_highlight= | Sets the colour of the permanent date highlight associated with the current date retrieved from the OS. <br> Example: ``` Calendar = Calendar(root, size=250, date_highlight='red', ...) ``` |
-| text_highlight_fill= | Sets the colour of the text associated with the permanent date highlight. <br> Example: ``` Calendar = Calendar(root, size=250, text_highlight_fill='pink' ...) ``` |
-| user_highlight_colour= | Sets the colour of the highlight that is created when the user clicks on a month date. <br> Example: ``` Calendar = Calendar(root, size=250, user_highlight_colour='magenta', ...) ``` |
-| user_highlight_text= | Sets the colour of the text associated with the user highlight. <br> Example: ``` Calendar = Calendar(root, size=250, user_highlight_text='blue' ...) ``` |
+| date_highlight= | Sets the colour of the permanent date highlight associated with the current date retrieved from the OS. <br> Example: ``` Calendar = Calendar(root, date_highlight='red') ``` |
+| text_highlight_fill= | Sets the colour of the text associated with the permanent date highlight. <br> Example: ``` Calendar = Calendar(root, text_highlight_fill='pink') ``` |
+| user_highlight_colour= | Sets the colour of the highlight that is created when the user clicks on a month date. <br> Example: ``` Calendar = Calendar(root, user_highlight_colour='magenta') ``` |
+| user_highlight_text= | Sets the colour of the text associated with the user highlight. <br> Example: ``` Calendar = Calendar(root, user_highlight_text='blue') ``` |
```

### Comparing `calendar_widget-1.0.7/README.md` & `calendar_widget-1.0.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -86,15 +86,14 @@
 # define the main window into which the widget will be placed
 root = tkinter.Tk()
 root.geometry('600x600')  # the geometry function defines the size of the tkinter window
                           # - in this case, we are using a window that is 600px by 600px
 
 # create the calendar widget
 Calendar = Calendar(root, # specify the tkinter window into which the widget will be placed
-	size = 250, # set the size of the calendar widget to 250px
 	pos_x = 0, # set the x position of the calendar widget within the tkinter window
 	pos_y = 0, # set the y position of the calendar widget within the tkinter window
 	background = 'lightblue', # set the background of the calendar to light blue
 	)
 
 # Note: images of the type 'png', 'gif', 'ppm', and 'pgm' can be set as the background.
 # However, these images will not scale with the size of the calendar.
@@ -114,15 +113,14 @@
 ```python
 # the 'Calendar_Click' function retrives the date selected on the Calendar by the user, and prints the date to the console
 def Calendar_Click():
 	print(Calendar.getdate())
 
 # create the calendar widget
 Calendar = Calendar(root,
-	size = 250,
 	pos_x = 0,
 	pos_y = 0, 
 	background = 'lightblue', 
 	command = Calendar_Click  # link the 'Calendar_Click' function to the widget
 	)
 ```
 
@@ -132,55 +130,57 @@
 
 # Widget Parameters - functionality and styling
 
 The table below specifies opitons availiable for styling and other operations associated with the calendar widget
 
 | options | description |
 | ------- | ----------- |
-| size= | Sets the width of the widget in pixels. The default width is 300px. <br> Example: ``` Calendar = Calendar(root, size=350, ...) ``` |
-| pos_x= | Sets the x coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. <br> Example: ``` Calendar = Calendar(root, size=350, pos_x=0, ...) ``` |
-| pos_y= | Sets the y coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. <br> Example: ``` Calendar = Calendar(root, size=350, pos_y=0, ...) ``` |
-| style= | Set the style="Dark" for the dark theme. If no styling is specified the Calendar will inherit its default white theme. <br> Example: ``` Calendar = Calendar(root, size=350, style='Dark', ...) ``` |
-| command= | A function to be called when the widget is clicked. <br> Example: ``` Calendar = Calendar(root, command=my_function, ...) ``` |
-| background= | Sets the background of the Calendar to a valid tkinter colour or image (png, gif, ppm, pgm). <br> Example: ``` Calendar = Calendar(root, background='sky.png', ...) ``` |
-| img_pos_x= | Set the x coordinate of the background image if specified (by default, this is the top left corner). <br> Example: ``` Calendar = Calendar(root, background='sky.png', img_pos_x=0, ...) ``` |
-| img_pos_y= | Set the y coordinate of the background image if specified (by default, this is the top left corner). <br> Example: ``` Calendar = Calendar(root, background='sky.png', img_pos_y=0, ...) ``` |
-| img_anchor= | Set the anchor of the background image if specified (by default, this is set to 'nw' - the top left corner). <br> Example: ``` Calendar = Calendar(root, background='sky.png', img_pos_x=0, img_pos_y=0, img_anchor='ne', ...) ``` |
-| arrow_box_border= | Sets the border colour of the box containing the arrows for selecting previous and following months. <br> Example: ``` Calendar = Calendar(root, size=250, arrow_box_border='blue', ...) ``` |
-| arrow_box_fill= | Sets the background of the box containing the arrows for selecting previous and following months. <br> Example: ``` Calendar = Calendar(root, size=300, arrow_box_fill='red', ...) ``` |
-| arrow_box_width= | Sets the line width of the box containing the arrows for selecting previous and following months. <br> Example: ``` Calendar = Calendar(root, size=350, arrow_box_width=3, ...) ``` |
-| date_box_fill= | Sets the colour inside of the boxes that make up the monthly calendar grid. <br> Example: ``` Calendar = Calendar(root, size=300, date_box_fill='purple', ...) ``` |
-| date_box_width= | Sets the width of the line used to create the grid for the monthly calendar. <br> Example: ``` Calendar = Calendar(root, size=350, date_box_width=5, ...) ``` |
-| date_boxes_outline= | Sets the colour of the box outline for the boxes that make up the monthly claendar grid. <br> Example: ``` Calendar = Calendar(root, size=350, date_boxes_outline='lime', ...) ``` |
-| arrow_outline= | Sets the colour for the outline of the polygon (i.e - triangle) that represents the calendar arrows. <br> Example: ``` Calendar = Calendar(root, size=350, arrow_outline='lightblue' ...) ``` |
-| arrow_fill= | Sets the colour of the calendar arrows. <br> Example: ``` Calendar = Calendar(root, size=350, arrow_fill='navy', ...) ``` |
-| arrow_thickness= | Sets the thickness of the calendar arrows. <br> Example: ``` Calendar = Calendar(root, size=350, arrow_thickness=5, ...) ``` |
-| arrow_active= | Sets the colour for the active highlight when the mouse hovers over the calendar arrows. <br> Example: ``` Calendar = Calendar(root, size=350, arrow_active='magenta', ...) ``` |
-| weekday_border= | Sets the colour for the outline of the boxes that hold the weekday headings. <br> Example: ``` Calendar = Calendar(root, size=300, weekday_border='blue', ...) ``` |
-| weekday_fill= | Sets the colour for the background of the boxes that hold the weekday headings. <br> Example: ``` Calendar = Calendar(root, size=250, weekday_fill='gray', ...) ``` |
-| weekday_width= | Sets the width of the boxes that hold the weekday headings. <br> Example: ``` Calendar = Calendar(root, size=250, weekday_width=3, ...) ``` |
-| weekday_font_fill= | Sets the colour of the text associated with the weekday headings. <br> Example: ``` Calendar = Calendar(root, size=250, weekday_font_fill='red' ...) ``` |
-| weekday_font_family= | Sets the type of font used to create the weekday headings. (Accepts any of the valid native tkinter fonts). <br> Example: ``` Calendar = Calendar(root, size=250, weekday_font_family='Georgia', ...) ``` |
-| weekday_font_weight= | Sets the weight of the font used to create the weekday headings. Valid options are 'normal' or 'bold'. <br> Example: ``` Calendar = Calendar(root, size=250, weekday_font_family='bold' ...) ``` |
-| weekday_font_slant= | Sets the slant of the font used to create the weekday headings. Valid options are 'roman' or 'italic'. <br> Example: ``` Calendar = Calendar(root, size=250, weekday_font_slant='italic', ...) ``` |
-| weekday_font_underline= | Sets the underline of the font used to creates the weekday heading. Valid options are True or False. <br> Example: ``` Calendar = Calendar(root, size=250, weekday_font_underline=True, ...) ``` |
-| weekday_font_size= | Sets the font size of the weekday headings. Note: this overrides the default size and scaling of the font. <br> Example: ``` Calendar = Calendar(root, size=250, weekday_font_size=10, ...) ``` |
-| calendar_date_title= | Sets the colour of the text associated with the calendar title (ex: Aug 2020). <br> Example: ``` Calendar = Calendar(root, size=250, calendar_date_title='red', ...) ``` |
-| date_heading_font_family= | Sets the font type for the Calendar date heading. (Accepts any of the valid native tkinter fonts). <br> Example: ``` Calendar = Calendar(root, size=250, date_heading_font_family='Helvetica', ...) ``` |
-| date_heading_font_weight= | Sets the weight of the font used to create the Calendar date heading. Valid options are 'normal' or 'bold'. <br> Example: ``` Calendar = Calendar(root, size=250, date_heading_font_weight='bold', ...) ``` |
-| date_heading_font_slant= | Sets the slant of the font used to create the Calendar date heading. Valid options are 'roman' or 'italic'. <br> Example: ``` Calendar = Calendar(root, size=250, date_heading_font_slant='italic', ...) ``` |
-| date_heading_font_underline= | Sets the underline of the font used to create the Calendar date heading. Valid options are True or False. <br> Example: ``` Calendar = Calendar(root, size=250, date_heading_font_underline=True, ...) ``` |
-| date_heading_font_size= | Sets the font size used to create the Calendar heading. Note: This overrides the default size and scaling of the font. <br> Example: ``` Calendar = Calendar(root, size=250, date_heading_font_size=15 ...) ``` |
-| date_text_fill= | Sets the colour of the text numbers associated with the month dates. <br> Example: ``` Calendar = Calendar(root, size=250, date_text_fill='green', ...) ``` |
-| date_text_font_family= | Sets the font type used to create the month dates. (Accepts any of the valid native tkinter fonts). <br> Example: ``` Calendar = Calendar(root, size=250, date_text_font_family='Georgia', ...) ``` |
-| date_text_font_weight= | Sets the weight of the font used to create the month dates. Valid options are 'normal' or 'bold'. <br> Example: ``` Calendar = Calendar(root, size=250, date_text_font_weight='bold', ...) ``` |
-| date_text_font_slant= | Sets the slant of the font used to create the month dates. Valid options are 'roman' or 'italic'. <br> Example: ``` Calendar = Calendar(root, size=250, date_text_font_slant='italic', ...) ``` |
-| date_text_font_underline= | Sets the underline of the font used to create the month dates. Valid options are True or False. <br> Example: ``` Calendar = Calendar(root, size=250, date_text_font_underline=True, ...) ``` |
-| date_text_font_size= | Sets the font size of the dates on the Calendar month grid. Note: this overrides the default size and scaling of the font. <br> Example: ``` Calendar = Calendar(root, size=250, date_text_font_size=10, ...) ``` |
-| trail_box_fill= | Sets the colour of the background of the date boxes that trail into the previous and following months. <br> Example: ``` Calendar = Calendar(root, size=250, trail_box_fill='lime', ...) ``` |
-| trail_text_fill= | Sets the colour of the text numbers associated with the trailing date boxes. <br> Example: ``` Calendar = Calendar(root, size=250, trail_text_fill='blue' ...) ``` |
+| width= | Sets the width of the widget in pixels. The default width is 300px. <br> Example: ``` Calendar = Calendar(root, width=350) ``` |
+| height= | Sets the height of the widget in pixels. The default height is 200px. <br> Example: ``` Calendar = Calendar(root, height=200) ``` |
+| padding= | Sets the internal padding of the calendar widget. The default padding is set to 10px. <br> Example: ``` Calendar = Calendar(root, padding=15) ```
+| pos_x= | Sets the x coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. <br> Example: ``` Calendar = Calendar(root, pos_x=0) ``` |
+| pos_y= | Sets the y coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. <br> Example: ``` Calendar = Calendar(root, pos_y=0) ``` |
+| style= | Set the style="Dark" for the dark theme. If no styling is specified the Calendar will inherit its default white theme. <br> Example: ``` Calendar = Calendar(root, style='Dark') ``` |
+| command= | A function to be called when the widget is clicked. <br> Example: ``` Calendar = Calendar(root, command=my_function) ``` |
+| background= | Sets the background of the Calendar to a valid tkinter colour or image (png, gif, ppm, pgm). <br> Example: ``` Calendar = Calendar(root, background='sky.png') ``` |
+| img_pos_x= | Set the x coordinate of the background image if specified (by default, this is the top left corner). <br> Example: ``` Calendar = Calendar(root, background='sky.png', img_pos_x=0) ``` |
+| img_pos_y= | Set the y coordinate of the background image if specified (by default, this is the top left corner). <br> Example: ``` Calendar = Calendar(root, background='sky.png', img_pos_y=0) ``` |
+| img_anchor= | Set the anchor of the background image if specified (by default, this is set to 'nw' - the top left corner). <br> Example: ``` Calendar = Calendar(root, background='sky.png', img_pos_x=0, img_pos_y=0, img_anchor='ne') ``` |
+| arrow_box_border= | Sets the border colour of the box containing the arrows for selecting previous and following months. <br> Example: ``` Calendar = Calendar(root, arrow_box_border='blue') ``` |
+| arrow_box_fill= | Sets the background of the box containing the arrows for selecting previous and following months. <br> Example: ``` Calendar = Calendar(root, arrow_box_fill='red') ``` |
+| arrow_box_width= | Sets the line width of the box containing the arrows for selecting previous and following months. <br> Example: ``` Calendar = Calendar(root, arrow_box_width=3) ``` |
+| date_box_fill= | Sets the colour inside of the boxes that make up the monthly calendar grid. <br> Example: ``` Calendar = Calendar(root, date_box_fill='purple') ``` |
+| date_box_width= | Sets the width of the line used to create the grid for the monthly calendar. <br> Example: ``` Calendar = Calendar(root, date_box_width=5) ``` |
+| date_boxes_outline= | Sets the colour of the box outline for the boxes that make up the monthly claendar grid. <br> Example: ``` Calendar = Calendar(root, date_boxes_outline='lime') ``` |
+| arrow_outline= | Sets the colour for the outline of the polygon (i.e - triangle) that represents the calendar arrows. <br> Example: ``` Calendar = Calendar(root, arrow_outline='lightblue') ``` |
+| arrow_fill= | Sets the colour of the calendar arrows. <br> Example: ``` Calendar = Calendar(root, arrow_fill='navy') ``` |
+| arrow_thickness= | Sets the thickness of the calendar arrows. <br> Example: ``` Calendar = Calendar(root, arrow_thickness=5) ``` |
+| arrow_active= | Sets the colour for the active highlight when the mouse hovers over the calendar arrows. <br> Example: ``` Calendar = Calendar(root, arrow_active='magenta') ``` |
+| weekday_border= | Sets the colour for the outline of the boxes that hold the weekday headings. <br> Example: ``` Calendar = Calendar(root, weekday_border='blue') ``` |
+| weekday_fill= | Sets the colour for the background of the boxes that hold the weekday headings. <br> Example: ``` Calendar = Calendar(root, weekday_fill='gray') ``` |
+| weekday_width= | Sets the width of the boxes that hold the weekday headings. <br> Example: ``` Calendar = Calendar(root, weekday_width=3) ``` |
+| weekday_font_fill= | Sets the colour of the text associated with the weekday headings. <br> Example: ``` Calendar = Calendar(root, weekday_font_fill='red') ``` |
+| weekday_font_family= | Sets the type of font used to create the weekday headings. (Accepts any of the valid native tkinter fonts). <br> Example: ``` Calendar = Calendar(root, weekday_font_family='Georgia') ``` |
+| weekday_font_weight= | Sets the weight of the font used to create the weekday headings. Valid options are 'normal' or 'bold'. <br> Example: ``` Calendar = Calendar(root, weekday_font_family='bold') ``` |
+| weekday_font_slant= | Sets the slant of the font used to create the weekday headings. Valid options are 'roman' or 'italic'. <br> Example: ``` Calendar = Calendar(root, weekday_font_slant='italic') ``` |
+| weekday_font_underline= | Sets the underline of the font used to creates the weekday heading. Valid options are True or False. <br> Example: ``` Calendar = Calendar(root, weekday_font_underline=True) ``` |
+| weekday_font_size= | Sets the font size of the weekday headings. Note: this overrides the default size and scaling of the font. <br> Example: ``` Calendar = Calendar(root, weekday_font_size=10) ``` |
+| calendar_date_title= | Sets the colour of the text associated with the calendar title (ex: Aug 2020). <br> Example: ``` Calendar = Calendar(root, calendar_date_title='red') ``` |
+| date_heading_font_family= | Sets the font type for the Calendar date heading. (Accepts any of the valid native tkinter fonts). <br> Example: ``` Calendar = Calendar(root, date_heading_font_family='Helvetica') ``` |
+| date_heading_font_weight= | Sets the weight of the font used to create the Calendar date heading. Valid options are 'normal' or 'bold'. <br> Example: ``` Calendar = Calendar(root, date_heading_font_weight='bold') ``` |
+| date_heading_font_slant= | Sets the slant of the font used to create the Calendar date heading. Valid options are 'roman' or 'italic'. <br> Example: ``` Calendar = Calendar(root, date_heading_font_slant='italic') ``` |
+| date_heading_font_underline= | Sets the underline of the font used to create the Calendar date heading. Valid options are True or False. <br> Example: ``` Calendar = Calendar(root, date_heading_font_underline=True) ``` |
+| date_heading_font_size= | Sets the font size used to create the Calendar heading. Note: This overrides the default size and scaling of the font. <br> Example: ``` Calendar = Calendar(root, date_heading_font_size=15) ``` |
+| date_text_fill= | Sets the colour of the text numbers associated with the month dates. <br> Example: ``` Calendar = Calendar(root, date_text_fill='green') ``` |
+| date_text_font_family= | Sets the font type used to create the month dates. (Accepts any of the valid native tkinter fonts). <br> Example: ``` Calendar = Calendar(root, date_text_font_family='Georgia') ``` |
+| date_text_font_weight= | Sets the weight of the font used to create the month dates. Valid options are 'normal' or 'bold'. <br> Example: ``` Calendar = Calendar(root, date_text_font_weight='bold') ``` |
+| date_text_font_slant= | Sets the slant of the font used to create the month dates. Valid options are 'roman' or 'italic'. <br> Example: ``` Calendar = Calendar(root, date_text_font_slant='italic') ``` |
+| date_text_font_underline= | Sets the underline of the font used to create the month dates. Valid options are True or False. <br> Example: ``` Calendar = Calendar(root, date_text_font_underline=True) ``` |
+| date_text_font_size= | Sets the font size of the dates on the Calendar month grid. Note: this overrides the default size and scaling of the font. <br> Example: ``` Calendar = Calendar(root, date_text_font_size=10) ``` |
+| trail_box_fill= | Sets the colour of the background of the date boxes that trail into the previous and following months. <br> Example: ``` Calendar = Calendar(root, trail_box_fill='lime') ``` |
+| trail_text_fill= | Sets the colour of the text numbers associated with the trailing date boxes. <br> Example: ``` Calendar = Calendar(root, trail_text_fill='blue') ``` |
 | current_date_highlight= | Toggles the current date highlight on/off. This parameter accepts a True or False value. Example: ``` Calendar = Calendar(root, current_date_highlight=False) ``` |
-| date_highlight= | Sets the colour of the permanent date highlight associated with the current date retrieved from the OS. <br> Example: ``` Calendar = Calendar(root, size=250, date_highlight='red', ...) ``` |
-| text_highlight_fill= | Sets the colour of the text associated with the permanent date highlight. <br> Example: ``` Calendar = Calendar(root, size=250, text_highlight_fill='pink' ...) ``` |
-| user_highlight_colour= | Sets the colour of the highlight that is created when the user clicks on a month date. <br> Example: ``` Calendar = Calendar(root, size=250, user_highlight_colour='magenta', ...) ``` |
-| user_highlight_text= | Sets the colour of the text associated with the user highlight. <br> Example: ``` Calendar = Calendar(root, size=250, user_highlight_text='blue' ...) ``` |
+| date_highlight= | Sets the colour of the permanent date highlight associated with the current date retrieved from the OS. <br> Example: ``` Calendar = Calendar(root, date_highlight='red') ``` |
+| text_highlight_fill= | Sets the colour of the text associated with the permanent date highlight. <br> Example: ``` Calendar = Calendar(root, text_highlight_fill='pink') ``` |
+| user_highlight_colour= | Sets the colour of the highlight that is created when the user clicks on a month date. <br> Example: ``` Calendar = Calendar(root, user_highlight_colour='magenta') ``` |
+| user_highlight_text= | Sets the colour of the text associated with the user highlight. <br> Example: ``` Calendar = Calendar(root, user_highlight_text='blue') ``` |
```

### Comparing `calendar_widget-1.0.7/pyproject.toml` & `calendar_widget-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "calendar_widget"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="Spartanlasergun", email="bns360@live.com" },
 ]
 description = "Calendar widget for use with python tkinter"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `calendar_widget-1.0.7/src/calendar_widget/Calendar_Widget.py` & `calendar_widget-1.0.8/src/calendar_widget/Calendar_Widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,17 @@
     # The init function parameters describe the information that dictates the size, position and styling associated with
     # the calendar object. Comments associated with the usage of each parameter is given within the __init__ function
     # where they are first defined and used.
     def __init__(self, 
             window_name, 
             pos_x=None, 
             pos_y=None, 
-            size=300, 
+            width=300,
+            height=200,
+            padding=10,
             style=None, 
             command="no command",
             background="default.gif",
             arrow_box_border="black",
             arrow_box_fill="white",
             arrow_box_width=1,
             date_box_fill="white",
@@ -100,18 +102,17 @@
             self.date_text_fill = "white"
             self.trail_box_fill = "gray20"
             self.trail_text_fill = "gray60"
             self.date_highlight = "lime"
             self.text_highlight_fill = "black"
 
 
-        # The default width of the calendar object is set at 300 pixels. The depth and the padding are both factors of
-        # the width.
-        depth = (0.666 * size)
-        padding = int(size * 0.03333)
+        # The default width of the calendar object is set at 300 pixels. The default height is set to 200 pixels.
+        size = width     # The widget was originally created with size as the only modifiable parameter.
+        depth = height   # The reassignment fixes some of these design flaws, though it is a bit redundant.
 
 
         # check if a image file is specified for the background
         img = None
         if background != None:
             if (background.endswith('.png')) or (background.endswith('.gif')) or (background.endswith('.ppm')) or (background.endswith('.pgm')):
                 if background == "default.gif":
```

### Comparing `calendar_widget-1.0.7/src/calendar_widget.egg-info/PKG-INFO` & `calendar_widget-1.0.8/src/calendar_widget.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calendar-widget
-Version: 1.0.7
+Version: 1.0.8
 Summary: Calendar widget for use with python tkinter
 Author-email: Spartanlasergun <bns360@live.com>
 Project-URL: Homepage, https://github.com/Spartanlasergun/calendar_widget
 Project-URL: Bug Tracker, https://github.com/Spartanlasergun/calendar_widget/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -102,15 +102,14 @@
 # define the main window into which the widget will be placed
 root = tkinter.Tk()
 root.geometry('600x600')  # the geometry function defines the size of the tkinter window
                           # - in this case, we are using a window that is 600px by 600px
 
 # create the calendar widget
 Calendar = Calendar(root, # specify the tkinter window into which the widget will be placed
-	size = 250, # set the size of the calendar widget to 250px
 	pos_x = 0, # set the x position of the calendar widget within the tkinter window
 	pos_y = 0, # set the y position of the calendar widget within the tkinter window
 	background = 'lightblue', # set the background of the calendar to light blue
 	)
 
 # Note: images of the type 'png', 'gif', 'ppm', and 'pgm' can be set as the background.
 # However, these images will not scale with the size of the calendar.
@@ -130,15 +129,14 @@
 ```python
 # the 'Calendar_Click' function retrives the date selected on the Calendar by the user, and prints the date to the console
 def Calendar_Click():
 	print(Calendar.getdate())
 
 # create the calendar widget
 Calendar = Calendar(root,
-	size = 250,
 	pos_x = 0,
 	pos_y = 0, 
 	background = 'lightblue', 
 	command = Calendar_Click  # link the 'Calendar_Click' function to the widget
 	)
 ```
 
@@ -148,55 +146,57 @@
 
 # Widget Parameters - functionality and styling
 
 The table below specifies opitons availiable for styling and other operations associated with the calendar widget
 
 | options | description |
 | ------- | ----------- |
-| size= | Sets the width of the widget in pixels. The default width is 300px. <br> Example: ``` Calendar = Calendar(root, size=350, ...) ``` |
-| pos_x= | Sets the x coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. <br> Example: ``` Calendar = Calendar(root, size=350, pos_x=0, ...) ``` |
-| pos_y= | Sets the y coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. <br> Example: ``` Calendar = Calendar(root, size=350, pos_y=0, ...) ``` |
-| style= | Set the style="Dark" for the dark theme. If no styling is specified the Calendar will inherit its default white theme. <br> Example: ``` Calendar = Calendar(root, size=350, style='Dark', ...) ``` |
-| command= | A function to be called when the widget is clicked. <br> Example: ``` Calendar = Calendar(root, command=my_function, ...) ``` |
-| background= | Sets the background of the Calendar to a valid tkinter colour or image (png, gif, ppm, pgm). <br> Example: ``` Calendar = Calendar(root, background='sky.png', ...) ``` |
-| img_pos_x= | Set the x coordinate of the background image if specified (by default, this is the top left corner). <br> Example: ``` Calendar = Calendar(root, background='sky.png', img_pos_x=0, ...) ``` |
-| img_pos_y= | Set the y coordinate of the background image if specified (by default, this is the top left corner). <br> Example: ``` Calendar = Calendar(root, background='sky.png', img_pos_y=0, ...) ``` |
-| img_anchor= | Set the anchor of the background image if specified (by default, this is set to 'nw' - the top left corner). <br> Example: ``` Calendar = Calendar(root, background='sky.png', img_pos_x=0, img_pos_y=0, img_anchor='ne', ...) ``` |
-| arrow_box_border= | Sets the border colour of the box containing the arrows for selecting previous and following months. <br> Example: ``` Calendar = Calendar(root, size=250, arrow_box_border='blue', ...) ``` |
-| arrow_box_fill= | Sets the background of the box containing the arrows for selecting previous and following months. <br> Example: ``` Calendar = Calendar(root, size=300, arrow_box_fill='red', ...) ``` |
-| arrow_box_width= | Sets the line width of the box containing the arrows for selecting previous and following months. <br> Example: ``` Calendar = Calendar(root, size=350, arrow_box_width=3, ...) ``` |
-| date_box_fill= | Sets the colour inside of the boxes that make up the monthly calendar grid. <br> Example: ``` Calendar = Calendar(root, size=300, date_box_fill='purple', ...) ``` |
-| date_box_width= | Sets the width of the line used to create the grid for the monthly calendar. <br> Example: ``` Calendar = Calendar(root, size=350, date_box_width=5, ...) ``` |
-| date_boxes_outline= | Sets the colour of the box outline for the boxes that make up the monthly claendar grid. <br> Example: ``` Calendar = Calendar(root, size=350, date_boxes_outline='lime', ...) ``` |
-| arrow_outline= | Sets the colour for the outline of the polygon (i.e - triangle) that represents the calendar arrows. <br> Example: ``` Calendar = Calendar(root, size=350, arrow_outline='lightblue' ...) ``` |
-| arrow_fill= | Sets the colour of the calendar arrows. <br> Example: ``` Calendar = Calendar(root, size=350, arrow_fill='navy', ...) ``` |
-| arrow_thickness= | Sets the thickness of the calendar arrows. <br> Example: ``` Calendar = Calendar(root, size=350, arrow_thickness=5, ...) ``` |
-| arrow_active= | Sets the colour for the active highlight when the mouse hovers over the calendar arrows. <br> Example: ``` Calendar = Calendar(root, size=350, arrow_active='magenta', ...) ``` |
-| weekday_border= | Sets the colour for the outline of the boxes that hold the weekday headings. <br> Example: ``` Calendar = Calendar(root, size=300, weekday_border='blue', ...) ``` |
-| weekday_fill= | Sets the colour for the background of the boxes that hold the weekday headings. <br> Example: ``` Calendar = Calendar(root, size=250, weekday_fill='gray', ...) ``` |
-| weekday_width= | Sets the width of the boxes that hold the weekday headings. <br> Example: ``` Calendar = Calendar(root, size=250, weekday_width=3, ...) ``` |
-| weekday_font_fill= | Sets the colour of the text associated with the weekday headings. <br> Example: ``` Calendar = Calendar(root, size=250, weekday_font_fill='red' ...) ``` |
-| weekday_font_family= | Sets the type of font used to create the weekday headings. (Accepts any of the valid native tkinter fonts). <br> Example: ``` Calendar = Calendar(root, size=250, weekday_font_family='Georgia', ...) ``` |
-| weekday_font_weight= | Sets the weight of the font used to create the weekday headings. Valid options are 'normal' or 'bold'. <br> Example: ``` Calendar = Calendar(root, size=250, weekday_font_family='bold' ...) ``` |
-| weekday_font_slant= | Sets the slant of the font used to create the weekday headings. Valid options are 'roman' or 'italic'. <br> Example: ``` Calendar = Calendar(root, size=250, weekday_font_slant='italic', ...) ``` |
-| weekday_font_underline= | Sets the underline of the font used to creates the weekday heading. Valid options are True or False. <br> Example: ``` Calendar = Calendar(root, size=250, weekday_font_underline=True, ...) ``` |
-| weekday_font_size= | Sets the font size of the weekday headings. Note: this overrides the default size and scaling of the font. <br> Example: ``` Calendar = Calendar(root, size=250, weekday_font_size=10, ...) ``` |
-| calendar_date_title= | Sets the colour of the text associated with the calendar title (ex: Aug 2020). <br> Example: ``` Calendar = Calendar(root, size=250, calendar_date_title='red', ...) ``` |
-| date_heading_font_family= | Sets the font type for the Calendar date heading. (Accepts any of the valid native tkinter fonts). <br> Example: ``` Calendar = Calendar(root, size=250, date_heading_font_family='Helvetica', ...) ``` |
-| date_heading_font_weight= | Sets the weight of the font used to create the Calendar date heading. Valid options are 'normal' or 'bold'. <br> Example: ``` Calendar = Calendar(root, size=250, date_heading_font_weight='bold', ...) ``` |
-| date_heading_font_slant= | Sets the slant of the font used to create the Calendar date heading. Valid options are 'roman' or 'italic'. <br> Example: ``` Calendar = Calendar(root, size=250, date_heading_font_slant='italic', ...) ``` |
-| date_heading_font_underline= | Sets the underline of the font used to create the Calendar date heading. Valid options are True or False. <br> Example: ``` Calendar = Calendar(root, size=250, date_heading_font_underline=True, ...) ``` |
-| date_heading_font_size= | Sets the font size used to create the Calendar heading. Note: This overrides the default size and scaling of the font. <br> Example: ``` Calendar = Calendar(root, size=250, date_heading_font_size=15 ...) ``` |
-| date_text_fill= | Sets the colour of the text numbers associated with the month dates. <br> Example: ``` Calendar = Calendar(root, size=250, date_text_fill='green', ...) ``` |
-| date_text_font_family= | Sets the font type used to create the month dates. (Accepts any of the valid native tkinter fonts). <br> Example: ``` Calendar = Calendar(root, size=250, date_text_font_family='Georgia', ...) ``` |
-| date_text_font_weight= | Sets the weight of the font used to create the month dates. Valid options are 'normal' or 'bold'. <br> Example: ``` Calendar = Calendar(root, size=250, date_text_font_weight='bold', ...) ``` |
-| date_text_font_slant= | Sets the slant of the font used to create the month dates. Valid options are 'roman' or 'italic'. <br> Example: ``` Calendar = Calendar(root, size=250, date_text_font_slant='italic', ...) ``` |
-| date_text_font_underline= | Sets the underline of the font used to create the month dates. Valid options are True or False. <br> Example: ``` Calendar = Calendar(root, size=250, date_text_font_underline=True, ...) ``` |
-| date_text_font_size= | Sets the font size of the dates on the Calendar month grid. Note: this overrides the default size and scaling of the font. <br> Example: ``` Calendar = Calendar(root, size=250, date_text_font_size=10, ...) ``` |
-| trail_box_fill= | Sets the colour of the background of the date boxes that trail into the previous and following months. <br> Example: ``` Calendar = Calendar(root, size=250, trail_box_fill='lime', ...) ``` |
-| trail_text_fill= | Sets the colour of the text numbers associated with the trailing date boxes. <br> Example: ``` Calendar = Calendar(root, size=250, trail_text_fill='blue' ...) ``` |
+| width= | Sets the width of the widget in pixels. The default width is 300px. <br> Example: ``` Calendar = Calendar(root, width=350) ``` |
+| height= | Sets the height of the widget in pixels. The default height is 200px. <br> Example: ``` Calendar = Calendar(root, height=200) ``` |
+| padding= | Sets the internal padding of the calendar widget. The default padding is set to 10px. <br> Example: ``` Calendar = Calendar(root, padding=15) ```
+| pos_x= | Sets the x coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. <br> Example: ``` Calendar = Calendar(root, pos_x=0) ``` |
+| pos_y= | Sets the y coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. <br> Example: ``` Calendar = Calendar(root, pos_y=0) ``` |
+| style= | Set the style="Dark" for the dark theme. If no styling is specified the Calendar will inherit its default white theme. <br> Example: ``` Calendar = Calendar(root, style='Dark') ``` |
+| command= | A function to be called when the widget is clicked. <br> Example: ``` Calendar = Calendar(root, command=my_function) ``` |
+| background= | Sets the background of the Calendar to a valid tkinter colour or image (png, gif, ppm, pgm). <br> Example: ``` Calendar = Calendar(root, background='sky.png') ``` |
+| img_pos_x= | Set the x coordinate of the background image if specified (by default, this is the top left corner). <br> Example: ``` Calendar = Calendar(root, background='sky.png', img_pos_x=0) ``` |
+| img_pos_y= | Set the y coordinate of the background image if specified (by default, this is the top left corner). <br> Example: ``` Calendar = Calendar(root, background='sky.png', img_pos_y=0) ``` |
+| img_anchor= | Set the anchor of the background image if specified (by default, this is set to 'nw' - the top left corner). <br> Example: ``` Calendar = Calendar(root, background='sky.png', img_pos_x=0, img_pos_y=0, img_anchor='ne') ``` |
+| arrow_box_border= | Sets the border colour of the box containing the arrows for selecting previous and following months. <br> Example: ``` Calendar = Calendar(root, arrow_box_border='blue') ``` |
+| arrow_box_fill= | Sets the background of the box containing the arrows for selecting previous and following months. <br> Example: ``` Calendar = Calendar(root, arrow_box_fill='red') ``` |
+| arrow_box_width= | Sets the line width of the box containing the arrows for selecting previous and following months. <br> Example: ``` Calendar = Calendar(root, arrow_box_width=3) ``` |
+| date_box_fill= | Sets the colour inside of the boxes that make up the monthly calendar grid. <br> Example: ``` Calendar = Calendar(root, date_box_fill='purple') ``` |
+| date_box_width= | Sets the width of the line used to create the grid for the monthly calendar. <br> Example: ``` Calendar = Calendar(root, date_box_width=5) ``` |
+| date_boxes_outline= | Sets the colour of the box outline for the boxes that make up the monthly claendar grid. <br> Example: ``` Calendar = Calendar(root, date_boxes_outline='lime') ``` |
+| arrow_outline= | Sets the colour for the outline of the polygon (i.e - triangle) that represents the calendar arrows. <br> Example: ``` Calendar = Calendar(root, arrow_outline='lightblue') ``` |
+| arrow_fill= | Sets the colour of the calendar arrows. <br> Example: ``` Calendar = Calendar(root, arrow_fill='navy') ``` |
+| arrow_thickness= | Sets the thickness of the calendar arrows. <br> Example: ``` Calendar = Calendar(root, arrow_thickness=5) ``` |
+| arrow_active= | Sets the colour for the active highlight when the mouse hovers over the calendar arrows. <br> Example: ``` Calendar = Calendar(root, arrow_active='magenta') ``` |
+| weekday_border= | Sets the colour for the outline of the boxes that hold the weekday headings. <br> Example: ``` Calendar = Calendar(root, weekday_border='blue') ``` |
+| weekday_fill= | Sets the colour for the background of the boxes that hold the weekday headings. <br> Example: ``` Calendar = Calendar(root, weekday_fill='gray') ``` |
+| weekday_width= | Sets the width of the boxes that hold the weekday headings. <br> Example: ``` Calendar = Calendar(root, weekday_width=3) ``` |
+| weekday_font_fill= | Sets the colour of the text associated with the weekday headings. <br> Example: ``` Calendar = Calendar(root, weekday_font_fill='red') ``` |
+| weekday_font_family= | Sets the type of font used to create the weekday headings. (Accepts any of the valid native tkinter fonts). <br> Example: ``` Calendar = Calendar(root, weekday_font_family='Georgia') ``` |
+| weekday_font_weight= | Sets the weight of the font used to create the weekday headings. Valid options are 'normal' or 'bold'. <br> Example: ``` Calendar = Calendar(root, weekday_font_family='bold') ``` |
+| weekday_font_slant= | Sets the slant of the font used to create the weekday headings. Valid options are 'roman' or 'italic'. <br> Example: ``` Calendar = Calendar(root, weekday_font_slant='italic') ``` |
+| weekday_font_underline= | Sets the underline of the font used to creates the weekday heading. Valid options are True or False. <br> Example: ``` Calendar = Calendar(root, weekday_font_underline=True) ``` |
+| weekday_font_size= | Sets the font size of the weekday headings. Note: this overrides the default size and scaling of the font. <br> Example: ``` Calendar = Calendar(root, weekday_font_size=10) ``` |
+| calendar_date_title= | Sets the colour of the text associated with the calendar title (ex: Aug 2020). <br> Example: ``` Calendar = Calendar(root, calendar_date_title='red') ``` |
+| date_heading_font_family= | Sets the font type for the Calendar date heading. (Accepts any of the valid native tkinter fonts). <br> Example: ``` Calendar = Calendar(root, date_heading_font_family='Helvetica') ``` |
+| date_heading_font_weight= | Sets the weight of the font used to create the Calendar date heading. Valid options are 'normal' or 'bold'. <br> Example: ``` Calendar = Calendar(root, date_heading_font_weight='bold') ``` |
+| date_heading_font_slant= | Sets the slant of the font used to create the Calendar date heading. Valid options are 'roman' or 'italic'. <br> Example: ``` Calendar = Calendar(root, date_heading_font_slant='italic') ``` |
+| date_heading_font_underline= | Sets the underline of the font used to create the Calendar date heading. Valid options are True or False. <br> Example: ``` Calendar = Calendar(root, date_heading_font_underline=True) ``` |
+| date_heading_font_size= | Sets the font size used to create the Calendar heading. Note: This overrides the default size and scaling of the font. <br> Example: ``` Calendar = Calendar(root, date_heading_font_size=15) ``` |
+| date_text_fill= | Sets the colour of the text numbers associated with the month dates. <br> Example: ``` Calendar = Calendar(root, date_text_fill='green') ``` |
+| date_text_font_family= | Sets the font type used to create the month dates. (Accepts any of the valid native tkinter fonts). <br> Example: ``` Calendar = Calendar(root, date_text_font_family='Georgia') ``` |
+| date_text_font_weight= | Sets the weight of the font used to create the month dates. Valid options are 'normal' or 'bold'. <br> Example: ``` Calendar = Calendar(root, date_text_font_weight='bold') ``` |
+| date_text_font_slant= | Sets the slant of the font used to create the month dates. Valid options are 'roman' or 'italic'. <br> Example: ``` Calendar = Calendar(root, date_text_font_slant='italic') ``` |
+| date_text_font_underline= | Sets the underline of the font used to create the month dates. Valid options are True or False. <br> Example: ``` Calendar = Calendar(root, date_text_font_underline=True) ``` |
+| date_text_font_size= | Sets the font size of the dates on the Calendar month grid. Note: this overrides the default size and scaling of the font. <br> Example: ``` Calendar = Calendar(root, date_text_font_size=10) ``` |
+| trail_box_fill= | Sets the colour of the background of the date boxes that trail into the previous and following months. <br> Example: ``` Calendar = Calendar(root, trail_box_fill='lime') ``` |
+| trail_text_fill= | Sets the colour of the text numbers associated with the trailing date boxes. <br> Example: ``` Calendar = Calendar(root, trail_text_fill='blue') ``` |
 | current_date_highlight= | Toggles the current date highlight on/off. This parameter accepts a True or False value. Example: ``` Calendar = Calendar(root, current_date_highlight=False) ``` |
-| date_highlight= | Sets the colour of the permanent date highlight associated with the current date retrieved from the OS. <br> Example: ``` Calendar = Calendar(root, size=250, date_highlight='red', ...) ``` |
-| text_highlight_fill= | Sets the colour of the text associated with the permanent date highlight. <br> Example: ``` Calendar = Calendar(root, size=250, text_highlight_fill='pink' ...) ``` |
-| user_highlight_colour= | Sets the colour of the highlight that is created when the user clicks on a month date. <br> Example: ``` Calendar = Calendar(root, size=250, user_highlight_colour='magenta', ...) ``` |
-| user_highlight_text= | Sets the colour of the text associated with the user highlight. <br> Example: ``` Calendar = Calendar(root, size=250, user_highlight_text='blue' ...) ``` |
+| date_highlight= | Sets the colour of the permanent date highlight associated with the current date retrieved from the OS. <br> Example: ``` Calendar = Calendar(root, date_highlight='red') ``` |
+| text_highlight_fill= | Sets the colour of the text associated with the permanent date highlight. <br> Example: ``` Calendar = Calendar(root, text_highlight_fill='pink') ``` |
+| user_highlight_colour= | Sets the colour of the highlight that is created when the user clicks on a month date. <br> Example: ``` Calendar = Calendar(root, user_highlight_colour='magenta') ``` |
+| user_highlight_text= | Sets the colour of the text associated with the user highlight. <br> Example: ``` Calendar = Calendar(root, user_highlight_text='blue') ``` |
```

