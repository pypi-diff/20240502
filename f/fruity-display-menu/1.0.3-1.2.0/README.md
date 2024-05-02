# Comparing `tmp/fruity_display_menu-1.0.3.tar.gz` & `tmp/fruity_display_menu-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fruity_display_menu-1.0.3.tar", last modified: Tue Nov 30 01:29:20 2021, max compression
+gzip compressed data, was "fruity_display_menu-1.2.0.tar", last modified: Thu May  2 20:38:56 2024, max compression
```

## Comparing `fruity_display_menu-1.0.3.tar` & `fruity_display_menu-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2021-11-30 01:29:20.233506 fruity_display_menu-1.0.3/
--rw-rw-rw-   0        0        0    17098 2021-11-26 17:59:40.000000 fruity_display_menu-1.0.3/LICENSE.md
--rw-rw-rw-   0        0        0     1951 2021-11-30 01:29:20.232506 fruity_display_menu-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1509 2021-11-26 22:08:12.000000 fruity_display_menu-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2021-11-30 01:29:20.227505 fruity_display_menu-1.0.3/fruity_display_menu.egg-info/
--rw-rw-rw-   0        0        0     1951 2021-11-30 01:29:20.000000 fruity_display_menu-1.0.3/fruity_display_menu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      467 2021-11-30 01:29:20.000000 fruity_display_menu-1.0.3/fruity_display_menu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-30 01:29:20.000000 fruity_display_menu-1.0.3/fruity_display_menu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2021-11-30 01:29:20.000000 fruity_display_menu-1.0.3/fruity_display_menu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2021-11-30 01:29:20.000000 fruity_display_menu-1.0.3/fruity_display_menu.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-11-30 01:29:20.229506 fruity_display_menu-1.0.3/fruity_menu/
--rw-rw-rw-   0        0        0       21 2021-11-30 01:28:36.000000 fruity_display_menu-1.0.3/fruity_menu/__init__.py
--rw-rw-rw-   0        0        0     1184 2021-10-29 16:50:53.000000 fruity_display_menu-1.0.3/fruity_menu/abstract.py
--rw-rw-rw-   0        0        0     5369 2021-11-30 00:44:53.000000 fruity_display_menu-1.0.3/fruity_menu/adjust.py
--rw-rw-rw-   0        0        0    11137 2021-11-30 01:22:05.000000 fruity_display_menu-1.0.3/fruity_menu/menu.py
--rw-rw-rw-   0        0        0     1876 2021-11-01 16:31:31.000000 fruity_display_menu-1.0.3/fruity_menu/options.py
--rw-rw-rw-   0        0        0       42 2021-11-30 01:29:20.233506 fruity_display_menu-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      897 2021-11-30 01:14:49.000000 fruity_display_menu-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2021-11-30 01:29:20.232506 fruity_display_menu-1.0.3/test/
--rw-rw-rw-   0        0        0      367 2021-11-01 02:15:50.000000 fruity_display_menu-1.0.3/test/test_adjust.py
--rw-rw-rw-   0        0        0     3890 2021-11-01 03:02:35.000000 fruity_display_menu-1.0.3/test/test_adjust_bool.py
--rw-rw-rw-   0        0        0     2573 2021-11-30 01:00:30.000000 fruity_display_menu-1.0.3/test/test_adjust_number.py
--rw-rw-rw-   0        0        0    14740 2021-11-26 18:04:40.000000 fruity_display_menu-1.0.3/test/test_menu.py
--rw-rw-rw-   0        0        0     1994 2021-11-01 16:37:24.000000 fruity_display_menu-1.0.3/test/test_options.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:38:56.535163 fruity_display_menu-1.2.0/
+-rw-rw-rw-   0        0        0    17098 2023-01-11 16:41:22.000000 fruity_display_menu-1.2.0/LICENSE.md
+-rw-rw-rw-   0        0        0     8770 2024-05-02 20:38:56.534658 fruity_display_menu-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8199 2024-05-02 20:01:28.000000 fruity_display_menu-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 20:38:56.533658 fruity_display_menu-1.2.0/fruity_display_menu.egg-info/
+-rw-rw-rw-   0        0        0     8770 2024-05-02 20:38:56.000000 fruity_display_menu-1.2.0/fruity_display_menu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      467 2024-05-02 20:38:56.000000 fruity_display_menu-1.2.0/fruity_display_menu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 20:38:56.000000 fruity_display_menu-1.2.0/fruity_display_menu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2024-05-02 20:38:56.000000 fruity_display_menu-1.2.0/fruity_display_menu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-02 20:38:56.000000 fruity_display_menu-1.2.0/fruity_display_menu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 20:38:56.530654 fruity_display_menu-1.2.0/fruity_menu/
+-rw-rw-rw-   0        0        0       21 2024-05-02 20:38:42.000000 fruity_display_menu-1.2.0/fruity_menu/__init__.py
+-rw-rw-rw-   0        0        0     1184 2023-01-11 16:41:22.000000 fruity_display_menu-1.2.0/fruity_menu/abstract.py
+-rw-rw-rw-   0        0        0     5369 2024-05-02 20:01:28.000000 fruity_display_menu-1.2.0/fruity_menu/adjust.py
+-rw-rw-rw-   0        0        0    11909 2024-05-02 20:01:28.000000 fruity_display_menu-1.2.0/fruity_menu/menu.py
+-rw-rw-rw-   0        0        0     1876 2024-05-02 20:01:28.000000 fruity_display_menu-1.2.0/fruity_menu/options.py
+-rw-rw-rw-   0        0        0       42 2024-05-02 20:38:56.535163 fruity_display_menu-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-01-11 16:41:22.000000 fruity_display_menu-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:38:56.533658 fruity_display_menu-1.2.0/test/
+-rw-rw-rw-   0        0        0      367 2023-01-11 16:41:22.000000 fruity_display_menu-1.2.0/test/test_adjust.py
+-rw-rw-rw-   0        0        0     3890 2023-01-11 16:41:22.000000 fruity_display_menu-1.2.0/test/test_adjust_bool.py
+-rw-rw-rw-   0        0        0     2573 2023-01-11 16:41:22.000000 fruity_display_menu-1.2.0/test/test_adjust_number.py
+-rw-rw-rw-   0        0        0    14742 2023-01-11 16:41:22.000000 fruity_display_menu-1.2.0/test/test_menu.py
+-rw-rw-rw-   0        0        0     1994 2023-01-11 16:41:22.000000 fruity_display_menu-1.2.0/test/test_options.py
```

### Comparing `fruity_display_menu-1.0.3/LICENSE.md` & `fruity_display_menu-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fruity_display_menu-1.0.3/fruity_menu/abstract.py` & `fruity_display_menu-1.2.0/fruity_menu/abstract.py`

 * *Files identical despite different names*

### Comparing `fruity_display_menu-1.0.3/fruity_menu/adjust.py` & `fruity_display_menu-1.2.0/fruity_menu/adjust.py`

 * *Files identical despite different names*

### Comparing `fruity_display_menu-1.0.3/fruity_menu/menu.py` & `fruity_display_menu-1.2.0/fruity_menu/menu.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from math import ceil, floor
 from displayio import Display, Group
+from os import getcwd
 import terminalio
+from time import time
 from adafruit_display_text.label import Label
+from adafruit_bitmapsaver import save_pixels
 
 from fruity_menu.adjust import AdjustMenu, BoolMenu, NumberMenu
 from fruity_menu.abstract import AbstractMenu
 from fruity_menu.options import ActionButton, SubmenuButton, ValueButton
 
 OPT_HIGHLIGHT_TEXT_COLOR = 0x0000FF
 """RGB color code to use for text in selected items"""
@@ -79,14 +82,20 @@
     X-coordinate for rendering menu
     """
 
     _y: int = 0
     """
     Y-coordinate for rendering menu
     """
+    
+    _save_debug_screenshots: bool = False
+    """
+    If True, then a screenshot will be saved every time the menu is redrawn.
+    This will seriously slow down the device and may quickly fill it up--use at your own risk!
+    """
 
     def __init__(self, display: Display, height, width, show_menu_title = True, title: str = 'Menu'):
         """
         Create a Menu for the given display.
         """
         self._display = display
         if (self._display is not None):
@@ -224,14 +233,24 @@
             # main and submenus can show themselves, but adjustmenus have to *be* shown
             if (isinstance(self._activated_submenu, AdjustMenu)):
                 grp = self._activated_submenu.build_displayio_group()
                 self._display.show(grp)
                 return grp
             else:
                 return self._activated_submenu.show_menu()
+            
+    def screenshot(self, hint: str) -> None:
+        """IF this menu has screenshots enables, this function takes a screenshot and saves it."""
+        if not self._save_debug_screenshots:
+            return
+        
+        name = hint + '-' + str(time())
+        save_pixels(name, self._display)
+        print('Saving screenshot to', name)
+        print('CWD:', getcwd())
 
     def click(self) -> bool:
         """Clicks the currently selected item and returns whether this menu is still open (True) or closed (False)"""
         # Exec submenu if open
         if (self._activated_submenu != None):
             # AdjustMenus have to be reloaded by their parent menu
             if (isinstance(self._activated_submenu, AdjustMenu)):
@@ -240,14 +259,15 @@
                     self._submenu_is_closing()
                 return True
             else:
                 return self._activated_submenu.click()
         else:
             # otherwise click this menu
             selected = self._options[self._selection]
+            self.screenshot(self._title)
             return selected.click()
             
 
     def scroll(self, delta: int) -> int:
         """
         Update menu's selected position using the given delta and allowing circular scrolling.
         The menu is not graphically updated.
```

### Comparing `fruity_display_menu-1.0.3/fruity_menu/options.py` & `fruity_display_menu-1.2.0/fruity_menu/options.py`

 * *Files identical despite different names*

### Comparing `fruity_display_menu-1.0.3/setup.py` & `fruity_display_menu-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `fruity_display_menu-1.0.3/test/test_adjust_bool.py` & `fruity_display_menu-1.2.0/test/test_adjust_bool.py`

 * *Files identical despite different names*

### Comparing `fruity_display_menu-1.0.3/test/test_adjust_number.py` & `fruity_display_menu-1.2.0/test/test_adjust_number.py`

 * *Files identical despite different names*

### Comparing `fruity_display_menu-1.0.3/test/test_menu.py` & `fruity_display_menu-1.2.0/test/test_menu.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         self.menu._activated_submenu = mock_submenu
         self.assertTrue(isinstance(self.menu.show_menu(), Group), 'Show_menu() did not return the displayio group it used')
 
     def test_showMenu_noSubmenu(self):
         self.assertTrue(isinstance(self.menu.show_menu(), Group), 'Show_menu() did not return the displayio group it used')
 
     def test_showMenu_hasAdjustMenu(self):
-        mock_submenu = Mock(AdjustMenu('', HEIGHT, WIDTH), get_displayio_group=TRUE_ACTION)
+        mock_submenu = Mock(AdjustMenu('', HEIGHT, WIDTH), build_displayio_group=TRUE_ACTION)
         self.menu._activated_submenu = mock_submenu
         self.assertEqual(True, self.menu.show_menu(), 'Show_menu() did not return the displayio group it used')
 
     def test_click_clicksSubmenu(self):
         planted_return_value = True
         submenu = Menu(get_mock_display(), HEIGHT, WIDTH)
         submenu.click = Mock(return_value=planted_return_value)
```

### Comparing `fruity_display_menu-1.0.3/test/test_options.py` & `fruity_display_menu-1.2.0/test/test_options.py`

 * *Files identical despite different names*

