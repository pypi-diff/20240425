# Comparing `tmp/reactionmenu-3.1.5.tar.gz` & `tmp/reactionmenu-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reactionmenu-3.1.5.tar", last modified: Wed Nov 29 14:50:41 2023, max compression
+gzip compressed data, was "reactionmenu-3.1.6.tar", last modified: Thu Apr 25 13:51:11 2024, max compression
```

## Comparing `reactionmenu-3.1.5.tar` & `reactionmenu-3.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jaggenneil   (501) staff       (20)        0 2023-11-29 14:50:41.186392 reactionmenu-3.1.5/
--rw-r--r--   0 jaggenneil   (501) staff       (20)     1101 2023-09-03 09:24:09.000000 reactionmenu-3.1.5/LICENSE
--rw-r--r--   0 jaggenneil   (501) staff       (20)    49865 2023-11-29 14:50:41.186185 reactionmenu-3.1.5/PKG-INFO
--rw-r--r--   0 jaggenneil   (501) staff       (20)    49457 2023-09-03 09:24:09.000000 reactionmenu-3.1.5/README.md
--rw-r--r--   0 jaggenneil   (501) staff       (20)     1756 2023-09-20 23:33:53.000000 reactionmenu-3.1.5/pyproject.toml
-drwxr-xr-x   0 jaggenneil   (501) staff       (20)        0 2023-11-29 14:50:41.184962 reactionmenu-3.1.5/reactionmenu/
--rw-r--r--   0 jaggenneil   (501) staff       (20)      591 2023-11-29 14:47:03.000000 reactionmenu-3.1.5/reactionmenu/__init__.py
--rw-r--r--   0 jaggenneil   (501) staff       (20)    62302 2023-09-03 09:24:09.000000 reactionmenu-3.1.5/reactionmenu/abc.py
--rw-r--r--   0 jaggenneil   (501) staff       (20)    22469 2023-09-03 09:24:09.000000 reactionmenu-3.1.5/reactionmenu/buttons.py
--rw-r--r--   0 jaggenneil   (501) staff       (20)    30786 2023-09-20 23:25:39.000000 reactionmenu-3.1.5/reactionmenu/core.py
--rw-r--r--   0 jaggenneil   (501) staff       (20)     2311 2023-09-03 09:24:09.000000 reactionmenu-3.1.5/reactionmenu/decorators.py
--rw-r--r--   0 jaggenneil   (501) staff       (20)     3747 2023-09-03 09:24:09.000000 reactionmenu-3.1.5/reactionmenu/errors.py
--rw-r--r--   0 jaggenneil   (501) staff       (20)    67218 2023-09-03 09:24:09.000000 reactionmenu-3.1.5/reactionmenu/views_menu.py
-drwxr-xr-x   0 jaggenneil   (501) staff       (20)        0 2023-11-29 14:50:41.185924 reactionmenu-3.1.5/reactionmenu.egg-info/
--rw-r--r--   0 jaggenneil   (501) staff       (20)    49865 2023-11-29 14:50:41.000000 reactionmenu-3.1.5/reactionmenu.egg-info/PKG-INFO
--rw-r--r--   0 jaggenneil   (501) staff       (20)      387 2023-11-29 14:50:41.000000 reactionmenu-3.1.5/reactionmenu.egg-info/SOURCES.txt
--rw-r--r--   0 jaggenneil   (501) staff       (20)        1 2023-11-29 14:50:41.000000 reactionmenu-3.1.5/reactionmenu.egg-info/dependency_links.txt
--rw-r--r--   0 jaggenneil   (501) staff       (20)       18 2023-11-29 14:50:41.000000 reactionmenu-3.1.5/reactionmenu.egg-info/requires.txt
--rw-r--r--   0 jaggenneil   (501) staff       (20)       13 2023-11-29 14:50:41.000000 reactionmenu-3.1.5/reactionmenu.egg-info/top_level.txt
--rw-r--r--   0 jaggenneil   (501) staff       (20)       38 2023-11-29 14:50:41.186437 reactionmenu-3.1.5/setup.cfg
--rw-r--r--   0 jaggenneil   (501) staff       (20)       71 2023-09-03 09:24:09.000000 reactionmenu-3.1.5/setup.py
+drwxr-xr-x   0 jaggenneil   (501) staff       (20)        0 2024-04-25 13:51:11.522335 reactionmenu-3.1.6/
+-rw-r--r--   0 jaggenneil   (501) staff       (20)     1097 2023-11-29 18:48:23.000000 reactionmenu-3.1.6/LICENSE
+-rw-r--r--   0 jaggenneil   (501) staff       (20)    50856 2024-04-25 13:51:11.522066 reactionmenu-3.1.6/PKG-INFO
+-rw-r--r--   0 jaggenneil   (501) staff       (20)    50450 2024-04-20 11:49:36.000000 reactionmenu-3.1.6/README.md
+-rw-r--r--   0 jaggenneil   (501) staff       (20)     1756 2024-04-20 12:38:19.000000 reactionmenu-3.1.6/pyproject.toml
+drwxr-xr-x   0 jaggenneil   (501) staff       (20)        0 2024-04-25 13:51:11.520222 reactionmenu-3.1.6/reactionmenu/
+-rw-r--r--   0 jaggenneil   (501) staff       (20)      591 2023-11-29 14:47:03.000000 reactionmenu-3.1.6/reactionmenu/__init__.py
+-rw-r--r--   0 jaggenneil   (501) staff       (20)    62636 2024-04-20 12:14:43.000000 reactionmenu-3.1.6/reactionmenu/abc.py
+-rw-r--r--   0 jaggenneil   (501) staff       (20)    22465 2023-11-29 18:47:56.000000 reactionmenu-3.1.6/reactionmenu/buttons.py
+-rw-r--r--   0 jaggenneil   (501) staff       (20)    30782 2023-11-29 18:47:56.000000 reactionmenu-3.1.6/reactionmenu/core.py
+-rw-r--r--   0 jaggenneil   (501) staff       (20)     2307 2023-11-29 18:47:56.000000 reactionmenu-3.1.6/reactionmenu/decorators.py
+-rw-r--r--   0 jaggenneil   (501) staff       (20)     3743 2023-11-29 18:47:56.000000 reactionmenu-3.1.6/reactionmenu/errors.py
+-rw-r--r--   0 jaggenneil   (501) staff       (20)    67510 2024-04-20 12:16:23.000000 reactionmenu-3.1.6/reactionmenu/views_menu.py
+drwxr-xr-x   0 jaggenneil   (501) staff       (20)        0 2024-04-25 13:51:11.521751 reactionmenu-3.1.6/reactionmenu.egg-info/
+-rw-r--r--   0 jaggenneil   (501) staff       (20)    50856 2024-04-25 13:51:11.000000 reactionmenu-3.1.6/reactionmenu.egg-info/PKG-INFO
+-rw-r--r--   0 jaggenneil   (501) staff       (20)      387 2024-04-25 13:51:11.000000 reactionmenu-3.1.6/reactionmenu.egg-info/SOURCES.txt
+-rw-r--r--   0 jaggenneil   (501) staff       (20)        1 2024-04-25 13:51:11.000000 reactionmenu-3.1.6/reactionmenu.egg-info/dependency_links.txt
+-rw-r--r--   0 jaggenneil   (501) staff       (20)       18 2024-04-25 13:51:11.000000 reactionmenu-3.1.6/reactionmenu.egg-info/requires.txt
+-rw-r--r--   0 jaggenneil   (501) staff       (20)       13 2024-04-25 13:51:11.000000 reactionmenu-3.1.6/reactionmenu.egg-info/top_level.txt
+-rw-r--r--   0 jaggenneil   (501) staff       (20)       38 2024-04-25 13:51:11.522501 reactionmenu-3.1.6/setup.cfg
+-rw-r--r--   0 jaggenneil   (501) staff       (20)       71 2023-09-03 09:24:09.000000 reactionmenu-3.1.6/setup.py
```

### Comparing `reactionmenu-3.1.5/LICENSE` & `reactionmenu-3.1.6/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021-present Defxult#8269
+Copyright (c) 2021-present @defxult
 
 Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"),
 to deal in the Software without restriction, including without limitation
 the rights to use, copy, modify, merge, publish, distribute, sublicense,
 and/or sell copies of the Software, and to permit persons to whom the
 Software is furnished to do so, subject to the following conditions:
```

### Comparing `reactionmenu-3.1.5/PKG-INFO` & `reactionmenu-3.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reactionmenu
-Version: 3.1.5
+Version: 3.1.6
 Summary: A library to create a discord.py 2.0+ paginator. Supports pagination with buttons, reactions, and category selection using selects.
 Author: Defxult
 License: MIT
 Project-URL: Homepage, https://github.com/Defxult/reactionmenu
 Project-URL: Changelog, https://github.com/Defxult/reactionmenu/blob/main/CHANGELOG.md
 Keywords: buttons,buttons paginator,buttons menu,discord,discord.py,discord.py 2.0,d.py,components,components paginator,components menu,discord components,discord components menu,discord buttons,discord buttons paginator,discord buttons menu,discord paginator,discord pagination,discord reaction menu,discord reactions,discord embed,discord menu,discord interactions,embed menu,embed reaction menu,embed paginator,interactions,interactions menu,interactions paginator,menus,paginator,pagination,pagination menu,reaction menu
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,22 +15,22 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: discord.py>=2.0.0
 
-![logo](https://cdn.discordapp.com/attachments/655186216060321816/820162226316378162/discord.jpg)
+![logo](https://cdn.discordapp.com/attachments/655186216060321816/820162226316378162/discord.jpg?ex=662c8918&is=661a1418&hm=8cec97b3bc3727c866814e3890eee87fd2eec32c638a5b377a9e564fb488881c&)
 <div align="center">
 
 [![Downloads](https://pepy.tech/badge/reactionmenu)](https://pepy.tech/project/reactionmenu) 
 [![Downloads](https://pepy.tech/badge/reactionmenu/month)](https://pepy.tech/project/reactionmenu)
 [![Downloads](https://pepy.tech/badge/reactionmenu/week)](https://pepy.tech/project/reactionmenu)
 
-![python_version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)
+![python_version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)
 </div>
 
 ## How to install
 You can install the latest [PyPI](https://pypi.org/project/reactionmenu/) version of the library by doing:
 ```
 $ pip install reactionmenu
 ```
@@ -49,15 +49,15 @@
 
 ```
 class reactionmenu.ReactionMenu(method: Union[Context, discord.Interaction], /, *, menu_type: MenuType, **kwargs)
 ```
 
 A `ReactionMenu` is a menu that uses emojis which are either custom guild emojis or a normal emoji to control the pagination process. If you're not looking for any of the fancy features and just want something simple, this is the one to use.
 
-![showcase](https://cdn.discordapp.com/attachments/655186216060321816/819885696176226314/showcase.gif)
+![showcase](https://cdn.discordapp.com/attachments/655186216060321816/819885696176226314/showcase.gif?ex=6634c20e&is=66224d0e&hm=9c7a9960dfe95e2abf99cc37fc88af9b40d036d047158a6c4e51b9cc59edcf16&)
 
 <details>
   <summary><b>Click to show ReactionMenu documentation</b></summary>
 
 ### How to import
 ```py
 from reactionmenu import ReactionMenu, ReactionButton
@@ -122,15 +122,15 @@
 menu.add_page(content='Its so hot!')
 menu.add_page(content='Its so cold!')
 ```
 
 #### ReactionMenu.TypeText
 A `TypeText` menu is a text based pagination menu. No embeds are involved in the pagination process, only plain text is used.
 
-![showcase-text](https://cdn.discordapp.com/attachments/655186216060321816/929172629947027466/text_showcase.gif)
+![showcase-text](https://cdn.discordapp.com/attachments/655186216060321816/929172629947027466/text_showcase.gif?ex=663583f2&is=66230ef2&hm=08e5208f0b95dd6d6fc203878fab1a19d32566cf28a32b25e7a4320ce3d4e924&)
 
 #### Stacked Pages
 With `v3.1.0+`, you can paginate with more than just an embed or text. You can combine text, embeds, as well as files. But depending on the `menu_type` the combination can be restricted. Here is an example of a menu with a `menu_type` of `TypeEmbed` that is stacked.
 
 ```py
 # You can use regular commands as well
 @bot.tree.command(description="These are stacked pages", guild=discord.Object(id=...))
@@ -142,15 +142,15 @@
     menu.add_page(discord.Embed(title="Hi, I'm Wumpos!"), files=[discord.File("wumpos.gif")])
     
     menu.add_button(ReactionButton.back())
     menu.add_button(ReactionButton.next())
     
     await menu.start()
 ```
-![stacked](https://cdn.discordapp.com/attachments/655186216060321816/955966821268332554/stacked.gif)
+![stacked](https://cdn.discordapp.com/attachments/655186216060321816/955966821268332554/stacked.gif?ex=66317a7b&is=661f057b&hm=06c4a45634f7471fbfdee81d3fb18cef4390bdc01740c304ea6ef000396adf06&)
 
 Since the `menu_type` is `TypeEmbed`, there always has to be an embed on each page. If the `menu_type` was `TypeText`, embeds aren't allowed and you will be restricted to only using the `files` parameter.
 
 #### ReactionMenu.TypeEmbedDynamic
 A dynamic menu is used when you do not know how much information will be applied to the menu. For example, if you were to request information from a database, that information can always change. You query something and you might get 1,500 results back, and the next maybe only 800. A dynamic menu pieces all this information together for you and adds it to an embed page by rows of data. `ReactionMenu.add_row()` is best used in some sort of `Iterable` where everything can be looped through, but only add the amount of data you want to the menu page.
 > **NOTE:** In a dynamic menu, all added data is placed in the description section of an embed. If you choose to use a `custom_embed`, all text in the description will be overridden with the data you add
 * Associated methods
@@ -468,15 +468,15 @@
 ## ViewMenu
 ```
 class reactionmenu.ViewMenu(method: Union[Context, discord.Interaction], /, *, menu_type: MenuType, **kwargs)
 ```
 
 A `ViewMenu` is a menu that uses discords Buttons feature. With buttons, you can enable and disable them, set a certain color for them with emojis, have buttons that send hidden messages, and add hyperlinks. This library offers a broader range of functionalities such as who pressed the button, how many times it was pressed and more. It uses views (`discord.ui.View`) to implement the Buttons functionality, but uses some of its own methods in order to make a Button pagination menu simple.
 
-![image](https://cdn.discordapp.com/attachments/655186216060321816/855818139450081280/buttons_showcase_reduced.gif)
+![image](https://cdn.discordapp.com/attachments/655186216060321816/855818139450081280/buttons_showcase_reduced.gif?ex=662d0d40&is=661a9840&hm=c27d8af03d464b3bb3942831c1f592042752aeb0baf903a3dbbffee7caade991&)
 
 <details>
   <summary><b>Click to show ViewMenu documentation</b></summary>
 
 
 ### How to import
 ```py
@@ -536,15 +536,15 @@
 menu.add_page(content='Its so hot!')
 menu.add_page(content='Its so cold!')
 ```
 
 #### ViewMenu.TypeText
 A `TypeText` menu is a text based pagination menu. No embeds are involved in the pagination process, only plain text is used.
 
-![text_view_showcase](https://cdn.discordapp.com/attachments/655186216060321816/929744985656549386/text_view_showcase.gif)
+![text_view_showcase](https://cdn.discordapp.com/attachments/655186216060321816/929744985656549386/text_view_showcase.gif?ex=66247b3e&is=662329be&hm=b94fa63761dee697cf4ce0a2e488e8a8119e65b9264d1178d64d8e26e944da91&)
 
 #### Stacked Pages
 With `v3.1.0+`, you can paginate with more than just an embed or text. You can combine text, embeds, as well as files. But depending on the `menu_type` the combination can be restricted. Here is an example of a menu with a `menu_type` of `TypeEmbed` that is stacked.
 
 ```py
 # You can use regular commands as well
 @bot.tree.command(description="These are stacked pages", guild=discord.Object(id=...))
@@ -556,15 +556,15 @@
     menu.add_page(discord.Embed(title="Hi, I'm Wumpos!"), files=[discord.File("wumpos.gif")])
     
     menu.add_button(ViewButton.back())
     menu.add_button(ViewButton.next())
     
     await menu.start()
 ```
-![stacked_view](https://cdn.discordapp.com/attachments/655186216060321816/955983620038860910/stacked_view.gif)
+![stacked_view](https://cdn.discordapp.com/attachments/655186216060321816/955983620038860910/stacked_view.gif?ex=66318a20&is=661f1520&hm=dc93e797cb16a1e3f87f36e02fa40b2733a40a1d469b7f1337d34d6037dad06e&)
 
 Since the `menu_type` is `TypeEmbed`, there always has to be an embed on each page. If the `menu_type` was `TypeText`, embeds aren't allowed and you will be restricted to only using the `files` parameter.
 
 #### ViewMenu.TypeEmbedDynamic
 A dynamic menu is used when you do not know how much information will be applied to the menu. For example, if you were to request information from a database, that information can always change. You query something and you might get 1,500 results back, and the next maybe only 800. A dynamic menu pieces all this information together for you and adds it to an embed page by rows of data. `ViewMenu.add_row()` is best used in some sort of `Iterable` where everything can be looped through, but only add the amount of data you want to the menu page.
 > **NOTE:** In a dynamic menu, all added data is placed in the description section of an embed. If you choose to use a `custom_embed`, all text in the description will be overridden with the data you add
 * Associated methods
@@ -715,17 +715,18 @@
 ```
 ---
 > **NOTE:** When it comes to buttons with a `custom_id` of `ViewButton.ID_CALLER`, `ViewButton.ID_SEND_MESSAGE`, `ViewButton.ID_CUSTOM_EMBED`, or link buttons, you can add as many as you'd like as long as in total it's 25 buttons or less. For all other button ID's, each menu can only have one.
 
 ### Using Selects
 Selects are used when you'd like to categorize information in your menu. Selects can only be used when the menu's `menu_type` is `TypeEmbed`. You should keep in mind that discords limitations on how many menu UI items (rows) can be applied to each message.
 
-![select_showcase](https://cdn.discordapp.com/attachments/655186216060321816/971361708121653268/select_showcase.gif)
+![select_showcase](https://cdn.discordapp.com/attachments/655186216060321816/971361708121653268/select_showcase.gif?ex=66321d16&is=661fa816&hm=f5a668a33715d0d5c77eb7c2a8ec9d01ef14b21c2d2f200c97d12ba70a7ab2bd&)
 
 * Associated Methods
+  * `Page.from_embeds(embeds: Sequence[Embed])` 
   * `ViewMenu.add_select(select: ViewSelect)`
   * `ViewMenu.remove_select(select: ViewSelect)`
   * `ViewMenu.remove_all_selects()`
   * `ViewMenu.disable_select(select: ViewSelect)`
   * `ViewMenu.disable_all_selects()`
   * `ViewMenu.enable_select(select: ViewSelect)`
   * `ViewMenu.enable_all_selects()`
@@ -735,14 +736,15 @@
 ```py
 from reactionmenu import ViewMenu, ViewSelect, Page
 
 menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbed)
 menu.add_page(discord.Embed(title="A showcase of console video games", color=discord.Color.blurple()))
 
 menu.add_select(ViewSelect(title="Console Video Games", options={
+    # NOTE: The discord.SelectOption parameter "default" cannot be set to True
     discord.SelectOption(label="PlayStation", emoji="<:PlayStation:549638412538478602>") : [
         Page(embed=discord.Embed(title="Ratchet & Clank", description=..., color=discord.Color.yellow()).set_image(url=...)),
         Page(embed=discord.Embed(title="God of War", description=..., color=discord.Color.blue()).set_image(url=...))
     ],
     discord.SelectOption(label="Xbox", emoji="<:Xbox:501880493285834752>") : [
         Page(embed=discord.Embed(title="Halo Infinite", description=..., color=discord.Color.green()).set_image(url=...)),
         Page(embed=discord.Embed(title="Gears of War 4", description=..., color=discord.Color.red()).set_image(url=...))
@@ -753,15 +755,15 @@
 menu.add_button(ViewButton.next())
 await menu.start()
 ```
 
 #### Go to page navigation
 You can use this type of select when you'd like to use the UI to select a page to go to.
 
-![goto_showcase](https://cdn.discordapp.com/attachments/655186216060321816/973629631905300501/Discord_6SP5AjoOOM.gif)
+![goto_showcase](https://cdn.discordapp.com/attachments/655186216060321816/973629631905300501/Discord_6SP5AjoOOM.gif?ex=663122c1&is=661eadc1&hm=a14135c7fa1c0b9c901b8216cbee7e77435fa1ba3148767d1870d52ba625001e&)
 
 * Associated methods
   * `ViewMenu.add_go_to_select(goto: ViewSelect.GoTo)`
   * `ViewMenu.enable_go_to_select(goto: ViewSelect.GoTo)`
   * `ViewMenu.enable_all_go_to_selects()`
   * `ViewMenu.disable_go_to_select(goto: ViewSelect.GoTo)`
   * `ViewMenu.disable_all_go_to_selects()`
```

### Comparing `reactionmenu-3.1.5/README.md` & `reactionmenu-3.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-![logo](https://cdn.discordapp.com/attachments/655186216060321816/820162226316378162/discord.jpg)
+![logo](https://cdn.discordapp.com/attachments/655186216060321816/820162226316378162/discord.jpg?ex=662c8918&is=661a1418&hm=8cec97b3bc3727c866814e3890eee87fd2eec32c638a5b377a9e564fb488881c&)
 <div align="center">
 
 [![Downloads](https://pepy.tech/badge/reactionmenu)](https://pepy.tech/project/reactionmenu) 
 [![Downloads](https://pepy.tech/badge/reactionmenu/month)](https://pepy.tech/project/reactionmenu)
 [![Downloads](https://pepy.tech/badge/reactionmenu/week)](https://pepy.tech/project/reactionmenu)
 
-![python_version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)
+![python_version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)
 </div>
 
 ## How to install
 You can install the latest [PyPI](https://pypi.org/project/reactionmenu/) version of the library by doing:
 ```
 $ pip install reactionmenu
 ```
@@ -28,15 +28,15 @@
 
 ```
 class reactionmenu.ReactionMenu(method: Union[Context, discord.Interaction], /, *, menu_type: MenuType, **kwargs)
 ```
 
 A `ReactionMenu` is a menu that uses emojis which are either custom guild emojis or a normal emoji to control the pagination process. If you're not looking for any of the fancy features and just want something simple, this is the one to use.
 
-![showcase](https://cdn.discordapp.com/attachments/655186216060321816/819885696176226314/showcase.gif)
+![showcase](https://cdn.discordapp.com/attachments/655186216060321816/819885696176226314/showcase.gif?ex=6634c20e&is=66224d0e&hm=9c7a9960dfe95e2abf99cc37fc88af9b40d036d047158a6c4e51b9cc59edcf16&)
 
 <details>
   <summary><b>Click to show ReactionMenu documentation</b></summary>
 
 ### How to import
 ```py
 from reactionmenu import ReactionMenu, ReactionButton
@@ -101,15 +101,15 @@
 menu.add_page(content='Its so hot!')
 menu.add_page(content='Its so cold!')
 ```
 
 #### ReactionMenu.TypeText
 A `TypeText` menu is a text based pagination menu. No embeds are involved in the pagination process, only plain text is used.
 
-![showcase-text](https://cdn.discordapp.com/attachments/655186216060321816/929172629947027466/text_showcase.gif)
+![showcase-text](https://cdn.discordapp.com/attachments/655186216060321816/929172629947027466/text_showcase.gif?ex=663583f2&is=66230ef2&hm=08e5208f0b95dd6d6fc203878fab1a19d32566cf28a32b25e7a4320ce3d4e924&)
 
 #### Stacked Pages
 With `v3.1.0+`, you can paginate with more than just an embed or text. You can combine text, embeds, as well as files. But depending on the `menu_type` the combination can be restricted. Here is an example of a menu with a `menu_type` of `TypeEmbed` that is stacked.
 
 ```py
 # You can use regular commands as well
 @bot.tree.command(description="These are stacked pages", guild=discord.Object(id=...))
@@ -121,15 +121,15 @@
     menu.add_page(discord.Embed(title="Hi, I'm Wumpos!"), files=[discord.File("wumpos.gif")])
     
     menu.add_button(ReactionButton.back())
     menu.add_button(ReactionButton.next())
     
     await menu.start()
 ```
-![stacked](https://cdn.discordapp.com/attachments/655186216060321816/955966821268332554/stacked.gif)
+![stacked](https://cdn.discordapp.com/attachments/655186216060321816/955966821268332554/stacked.gif?ex=66317a7b&is=661f057b&hm=06c4a45634f7471fbfdee81d3fb18cef4390bdc01740c304ea6ef000396adf06&)
 
 Since the `menu_type` is `TypeEmbed`, there always has to be an embed on each page. If the `menu_type` was `TypeText`, embeds aren't allowed and you will be restricted to only using the `files` parameter.
 
 #### ReactionMenu.TypeEmbedDynamic
 A dynamic menu is used when you do not know how much information will be applied to the menu. For example, if you were to request information from a database, that information can always change. You query something and you might get 1,500 results back, and the next maybe only 800. A dynamic menu pieces all this information together for you and adds it to an embed page by rows of data. `ReactionMenu.add_row()` is best used in some sort of `Iterable` where everything can be looped through, but only add the amount of data you want to the menu page.
 > **NOTE:** In a dynamic menu, all added data is placed in the description section of an embed. If you choose to use a `custom_embed`, all text in the description will be overridden with the data you add
 * Associated methods
@@ -447,15 +447,15 @@
 ## ViewMenu
 ```
 class reactionmenu.ViewMenu(method: Union[Context, discord.Interaction], /, *, menu_type: MenuType, **kwargs)
 ```
 
 A `ViewMenu` is a menu that uses discords Buttons feature. With buttons, you can enable and disable them, set a certain color for them with emojis, have buttons that send hidden messages, and add hyperlinks. This library offers a broader range of functionalities such as who pressed the button, how many times it was pressed and more. It uses views (`discord.ui.View`) to implement the Buttons functionality, but uses some of its own methods in order to make a Button pagination menu simple.
 
-![image](https://cdn.discordapp.com/attachments/655186216060321816/855818139450081280/buttons_showcase_reduced.gif)
+![image](https://cdn.discordapp.com/attachments/655186216060321816/855818139450081280/buttons_showcase_reduced.gif?ex=662d0d40&is=661a9840&hm=c27d8af03d464b3bb3942831c1f592042752aeb0baf903a3dbbffee7caade991&)
 
 <details>
   <summary><b>Click to show ViewMenu documentation</b></summary>
 
 
 ### How to import
 ```py
@@ -515,15 +515,15 @@
 menu.add_page(content='Its so hot!')
 menu.add_page(content='Its so cold!')
 ```
 
 #### ViewMenu.TypeText
 A `TypeText` menu is a text based pagination menu. No embeds are involved in the pagination process, only plain text is used.
 
-![text_view_showcase](https://cdn.discordapp.com/attachments/655186216060321816/929744985656549386/text_view_showcase.gif)
+![text_view_showcase](https://cdn.discordapp.com/attachments/655186216060321816/929744985656549386/text_view_showcase.gif?ex=66247b3e&is=662329be&hm=b94fa63761dee697cf4ce0a2e488e8a8119e65b9264d1178d64d8e26e944da91&)
 
 #### Stacked Pages
 With `v3.1.0+`, you can paginate with more than just an embed or text. You can combine text, embeds, as well as files. But depending on the `menu_type` the combination can be restricted. Here is an example of a menu with a `menu_type` of `TypeEmbed` that is stacked.
 
 ```py
 # You can use regular commands as well
 @bot.tree.command(description="These are stacked pages", guild=discord.Object(id=...))
@@ -535,15 +535,15 @@
     menu.add_page(discord.Embed(title="Hi, I'm Wumpos!"), files=[discord.File("wumpos.gif")])
     
     menu.add_button(ViewButton.back())
     menu.add_button(ViewButton.next())
     
     await menu.start()
 ```
-![stacked_view](https://cdn.discordapp.com/attachments/655186216060321816/955983620038860910/stacked_view.gif)
+![stacked_view](https://cdn.discordapp.com/attachments/655186216060321816/955983620038860910/stacked_view.gif?ex=66318a20&is=661f1520&hm=dc93e797cb16a1e3f87f36e02fa40b2733a40a1d469b7f1337d34d6037dad06e&)
 
 Since the `menu_type` is `TypeEmbed`, there always has to be an embed on each page. If the `menu_type` was `TypeText`, embeds aren't allowed and you will be restricted to only using the `files` parameter.
 
 #### ViewMenu.TypeEmbedDynamic
 A dynamic menu is used when you do not know how much information will be applied to the menu. For example, if you were to request information from a database, that information can always change. You query something and you might get 1,500 results back, and the next maybe only 800. A dynamic menu pieces all this information together for you and adds it to an embed page by rows of data. `ViewMenu.add_row()` is best used in some sort of `Iterable` where everything can be looped through, but only add the amount of data you want to the menu page.
 > **NOTE:** In a dynamic menu, all added data is placed in the description section of an embed. If you choose to use a `custom_embed`, all text in the description will be overridden with the data you add
 * Associated methods
@@ -694,17 +694,18 @@
 ```
 ---
 > **NOTE:** When it comes to buttons with a `custom_id` of `ViewButton.ID_CALLER`, `ViewButton.ID_SEND_MESSAGE`, `ViewButton.ID_CUSTOM_EMBED`, or link buttons, you can add as many as you'd like as long as in total it's 25 buttons or less. For all other button ID's, each menu can only have one.
 
 ### Using Selects
 Selects are used when you'd like to categorize information in your menu. Selects can only be used when the menu's `menu_type` is `TypeEmbed`. You should keep in mind that discords limitations on how many menu UI items (rows) can be applied to each message.
 
-![select_showcase](https://cdn.discordapp.com/attachments/655186216060321816/971361708121653268/select_showcase.gif)
+![select_showcase](https://cdn.discordapp.com/attachments/655186216060321816/971361708121653268/select_showcase.gif?ex=66321d16&is=661fa816&hm=f5a668a33715d0d5c77eb7c2a8ec9d01ef14b21c2d2f200c97d12ba70a7ab2bd&)
 
 * Associated Methods
+  * `Page.from_embeds(embeds: Sequence[Embed])` 
   * `ViewMenu.add_select(select: ViewSelect)`
   * `ViewMenu.remove_select(select: ViewSelect)`
   * `ViewMenu.remove_all_selects()`
   * `ViewMenu.disable_select(select: ViewSelect)`
   * `ViewMenu.disable_all_selects()`
   * `ViewMenu.enable_select(select: ViewSelect)`
   * `ViewMenu.enable_all_selects()`
@@ -714,14 +715,15 @@
 ```py
 from reactionmenu import ViewMenu, ViewSelect, Page
 
 menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbed)
 menu.add_page(discord.Embed(title="A showcase of console video games", color=discord.Color.blurple()))
 
 menu.add_select(ViewSelect(title="Console Video Games", options={
+    # NOTE: The discord.SelectOption parameter "default" cannot be set to True
     discord.SelectOption(label="PlayStation", emoji="<:PlayStation:549638412538478602>") : [
         Page(embed=discord.Embed(title="Ratchet & Clank", description=..., color=discord.Color.yellow()).set_image(url=...)),
         Page(embed=discord.Embed(title="God of War", description=..., color=discord.Color.blue()).set_image(url=...))
     ],
     discord.SelectOption(label="Xbox", emoji="<:Xbox:501880493285834752>") : [
         Page(embed=discord.Embed(title="Halo Infinite", description=..., color=discord.Color.green()).set_image(url=...)),
         Page(embed=discord.Embed(title="Gears of War 4", description=..., color=discord.Color.red()).set_image(url=...))
@@ -732,15 +734,15 @@
 menu.add_button(ViewButton.next())
 await menu.start()
 ```
 
 #### Go to page navigation
 You can use this type of select when you'd like to use the UI to select a page to go to.
 
-![goto_showcase](https://cdn.discordapp.com/attachments/655186216060321816/973629631905300501/Discord_6SP5AjoOOM.gif)
+![goto_showcase](https://cdn.discordapp.com/attachments/655186216060321816/973629631905300501/Discord_6SP5AjoOOM.gif?ex=663122c1&is=661eadc1&hm=a14135c7fa1c0b9c901b8216cbee7e77435fa1ba3148767d1870d52ba625001e&)
 
 * Associated methods
   * `ViewMenu.add_go_to_select(goto: ViewSelect.GoTo)`
   * `ViewMenu.enable_go_to_select(goto: ViewSelect.GoTo)`
   * `ViewMenu.enable_all_go_to_selects()`
   * `ViewMenu.disable_go_to_select(goto: ViewSelect.GoTo)`
   * `ViewMenu.disable_all_go_to_selects()`
```

### Comparing `reactionmenu-3.1.5/pyproject.toml` & `reactionmenu-3.1.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 
 [project]
 authors = [{name = "Defxult"}]
 name = "reactionmenu"
 readme = "README.md"
-version = "3.1.5"
+version = "3.1.6"
 description = "A library to create a discord.py 2.0+ paginator. Supports pagination with buttons, reactions, and category selection using selects."
 requires-python = ">=3.8"
 license = {text = "MIT"}
 dependencies = ["discord.py>=2.0.0"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
```

### Comparing `reactionmenu-3.1.5/reactionmenu/__init__.py` & `reactionmenu-3.1.6/reactionmenu/__init__.py`

 * *Files identical despite different names*

### Comparing `reactionmenu-3.1.5/reactionmenu/abc.py` & `reactionmenu-3.1.6/reactionmenu/abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 MIT License
 
-Copyright (c) 2021-present Defxult#8269
+Copyright (c) 2021-present @defxult
 
 Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"),
 to deal in the Software without restriction, including without limitation
 the rights to use, copy, modify, merge, publish, distribute, sublicense,
 and/or sell copies of the Software, and to permit persons to whom the
 Software is furnished to do so, subject to the following conditions:
@@ -87,14 +87,25 @@
     
     def __repr__(self) -> str:
         return f"<Page {' '.join([f'{attr_name}={getattr(self, attr_name)!r}' for attr_name in self.__class__.__slots__ if type(getattr(self, attr_name)) not in (type(None), type(MISSING))])}>"
     
     def _shallow(self) -> Self:
         from copy import copy
         return copy(self)
+    
+    @staticmethod
+    def from_embeds(embeds: Sequence[discord.Embed]) -> List[Page]:
+        """|static method|
+        
+        Converts a sequence of embeds into a list of :class:`Page`
+        """
+        pages: List[Page] = []
+        for e in embeds:
+            pages.append(Page(embed=discord.Embed.copy(e)))
+        return pages
 
 class PaginationEmojis:
     """A set of basic emojis for your convenience to use for your buttons emoji
     - ◀️ as `BACK_BUTTON`
     - ▶️ as `NEXT_BUTTON`
     - ⏪ as `FIRST_PAGE`
     - ⏩ as `LAST_PAGE`
@@ -369,15 +380,15 @@
     
     @abc.abstractmethod
     async def start(self):
         raise NotImplementedError
     
     # ABC class methods
     
-    @abc.abstractclassmethod
+    @abc.abstractmethod
     async def quick_start(cls):
         raise NotImplementedError
     
     @staticmethod
     def separate(values: Sequence[Any]) -> Tuple[List[discord.Embed], List[str]]:
         """|static method|
```

### Comparing `reactionmenu-3.1.5/reactionmenu/buttons.py` & `reactionmenu-3.1.6/reactionmenu/buttons.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 MIT License
 
-Copyright (c) 2021-present Defxult#8269
+Copyright (c) 2021-present @defxult
 
 Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"),
 to deal in the Software without restriction, including without limitation
 the rights to use, copy, modify, merge, publish, distribute, sublicense,
 and/or sell copies of the Software, and to permit persons to whom the
 Software is furnished to do so, subject to the following conditions:
```

### Comparing `reactionmenu-3.1.5/reactionmenu/core.py` & `reactionmenu-3.1.6/reactionmenu/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 MIT License
 
-Copyright (c) 2021-present Defxult#8269
+Copyright (c) 2021-present @defxult
 
 Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"),
 to deal in the Software without restriction, including without limitation
 the rights to use, copy, modify, merge, publish, distribute, sublicense,
 and/or sell copies of the Software, and to permit persons to whom the
 Software is furnished to do so, subject to the following conditions:
```

### Comparing `reactionmenu-3.1.5/reactionmenu/decorators.py` & `reactionmenu-3.1.6/reactionmenu/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 MIT License
 
-Copyright (c) 2021-present Defxult#8269
+Copyright (c) 2021-present @defxult
 
 Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"),
 to deal in the Software without restriction, including without limitation
 the rights to use, copy, modify, merge, publish, distribute, sublicense,
 and/or sell copies of the Software, and to permit persons to whom the
 Software is furnished to do so, subject to the following conditions:
```

### Comparing `reactionmenu-3.1.5/reactionmenu/errors.py` & `reactionmenu-3.1.6/reactionmenu/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 MIT License
 
-Copyright (c) 2021-present Defxult#8269
+Copyright (c) 2021-present @defxult
 
 Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"),
 to deal in the Software without restriction, including without limitation
 the rights to use, copy, modify, merge, publish, distribute, sublicense,
 and/or sell copies of the Software, and to permit persons to whom the
 Software is furnished to do so, subject to the following conditions:
```

### Comparing `reactionmenu-3.1.5/reactionmenu/views_menu.py` & `reactionmenu-3.1.6/reactionmenu/views_menu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 MIT License
 
-Copyright (c) 2021-present Defxult#8269
+Copyright (c) 2021-present @defxult
 
 Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"),
 to deal in the Software without restriction, including without limitation
 the rights to use, copy, modify, merge, publish, distribute, sublicense,
 and/or sell copies of the Software, and to permit persons to whom the
 Software is furnished to do so, subject to the following conditions:
@@ -127,15 +127,16 @@
     
     async def callback(self, interaction: discord.Interaction) -> None:
         """*INTERNAL USE ONLY* - The callback function from the select interaction. This should not be manually called"""
         for option, pages in self._view_select_options.items():
             if option.label == self.values[0]:
                 if self._menu:
                     self._menu._pc = _PageController(pages)
-                    await interaction.response.edit_message(**self._menu._determine_kwargs(self._menu._pc.first_page()))
+                    first_page = self._menu._pc.first_page()
+                    await interaction.response.edit_message(**self._menu._determine_kwargs(first_page))
                     break
         await self.__dispatch_relay(interaction)
 
     class GoTo(discord.ui.Select):
         """Represents a UI based version of a :class:`ViewButton` with the ID `ViewButton.ID_GO_TO_PAGE`
 
         Parameters
@@ -516,14 +517,20 @@
         for all_pages in pages:
             for individual_page in all_pages:
                 if not individual_page.embed:
                     raise ViewMenuException("The 'embed' parameter in a Page must be set when using selects")
         else:
             if self._menu_type == ViewMenu.TypeEmbed:
                 select._menu = self
+
+                # prevent default select options (https://github.com/Defxult/reactionmenu/issues/55)
+                for option in select.options:
+                    if option.default:
+                        option.default = False
+                
                 self.__view.add_item(select)
                 self.__selects.append(select)
             else:
                 raise ViewMenuException('Selects can only be added when the menu_type is TypeEmbed')
     
     def remove_select(self, select: ViewSelect) -> None:
         """Remove a select from the menu
@@ -1105,17 +1112,17 @@
             await inter.response.edit_message(**self._determine_kwargs(self._pc.first_page()))
         
         elif button.custom_id == ViewButton.ID_GO_TO_LAST_PAGE:
             await inter.response.edit_message(**self._determine_kwargs(self._pc.last_page()))
         
         elif button.custom_id == ViewButton.ID_GO_TO_PAGE:
             await inter.response.defer()
-            prompt: discord.Message = await self._msg.channel.send(f'{inter.user.display_name}, what page would you like to go to?') # type: ignore / `.channel` is know at this point
+            prompt: discord.Message = await self._msg.channel.send(f'{inter.user.display_name}, what page would you like to go to?') # type: ignore / `.channel` is known at this point
             try:
-                selection_message: discord.Message = await inter.client.wait_for('message', check=lambda m: all([m.channel.id == self._msg.channel.id, m.author.id == inter.user.id]), timeout=self.timeout) # type: ignore / `.channel` is know at this point
+                selection_message: discord.Message = await inter.client.wait_for('message', check=lambda m: all([m.channel.id == self._msg.channel.id, m.author.id == inter.user.id]), timeout=self.timeout) # type: ignore / `.channel` is known at this point
                 page = int(selection_message.content)
             except (asyncio.TimeoutError, ValueError):
                 return
             else:
                 if 1 <= page <= len(self._pages):
                     self._pc.index = page - 1
                     await self._msg.edit(**self._determine_kwargs(self._pc.current_page))
@@ -1144,15 +1151,15 @@
 
                 try:
                     if asyncio.iscoroutinefunction(func): await func(*args, **kwargs) # type: ignore / `func` is already confirmed to be a coroutine
                     else: func(*args, **kwargs)
                 except Exception as err:
                     call_failed_error_msg = inspect.cleandoc(
                         f"""
-                        The button with custom_id ViewButton.ID_CALLER with the label "{button.label}" raised an error during it's execution
+                        The button with custom_id ViewButton.ID_CALLER with the label "{button.label}" raised an error during its execution
                         -> {err.__class__.__name__}: {err}
                         """
                     )
                     raise ViewMenuException(call_failed_error_msg)
                 else:
                     if button.followup:
                         # if this executes, the user doesn't want to respond with a message, only with the caller function (already called ^)
```

### Comparing `reactionmenu-3.1.5/reactionmenu.egg-info/PKG-INFO` & `reactionmenu-3.1.6/reactionmenu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reactionmenu
-Version: 3.1.5
+Version: 3.1.6
 Summary: A library to create a discord.py 2.0+ paginator. Supports pagination with buttons, reactions, and category selection using selects.
 Author: Defxult
 License: MIT
 Project-URL: Homepage, https://github.com/Defxult/reactionmenu
 Project-URL: Changelog, https://github.com/Defxult/reactionmenu/blob/main/CHANGELOG.md
 Keywords: buttons,buttons paginator,buttons menu,discord,discord.py,discord.py 2.0,d.py,components,components paginator,components menu,discord components,discord components menu,discord buttons,discord buttons paginator,discord buttons menu,discord paginator,discord pagination,discord reaction menu,discord reactions,discord embed,discord menu,discord interactions,embed menu,embed reaction menu,embed paginator,interactions,interactions menu,interactions paginator,menus,paginator,pagination,pagination menu,reaction menu
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,22 +15,22 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: discord.py>=2.0.0
 
-![logo](https://cdn.discordapp.com/attachments/655186216060321816/820162226316378162/discord.jpg)
+![logo](https://cdn.discordapp.com/attachments/655186216060321816/820162226316378162/discord.jpg?ex=662c8918&is=661a1418&hm=8cec97b3bc3727c866814e3890eee87fd2eec32c638a5b377a9e564fb488881c&)
 <div align="center">
 
 [![Downloads](https://pepy.tech/badge/reactionmenu)](https://pepy.tech/project/reactionmenu) 
 [![Downloads](https://pepy.tech/badge/reactionmenu/month)](https://pepy.tech/project/reactionmenu)
 [![Downloads](https://pepy.tech/badge/reactionmenu/week)](https://pepy.tech/project/reactionmenu)
 
-![python_version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)
+![python_version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)
 </div>
 
 ## How to install
 You can install the latest [PyPI](https://pypi.org/project/reactionmenu/) version of the library by doing:
 ```
 $ pip install reactionmenu
 ```
@@ -49,15 +49,15 @@
 
 ```
 class reactionmenu.ReactionMenu(method: Union[Context, discord.Interaction], /, *, menu_type: MenuType, **kwargs)
 ```
 
 A `ReactionMenu` is a menu that uses emojis which are either custom guild emojis or a normal emoji to control the pagination process. If you're not looking for any of the fancy features and just want something simple, this is the one to use.
 
-![showcase](https://cdn.discordapp.com/attachments/655186216060321816/819885696176226314/showcase.gif)
+![showcase](https://cdn.discordapp.com/attachments/655186216060321816/819885696176226314/showcase.gif?ex=6634c20e&is=66224d0e&hm=9c7a9960dfe95e2abf99cc37fc88af9b40d036d047158a6c4e51b9cc59edcf16&)
 
 <details>
   <summary><b>Click to show ReactionMenu documentation</b></summary>
 
 ### How to import
 ```py
 from reactionmenu import ReactionMenu, ReactionButton
@@ -122,15 +122,15 @@
 menu.add_page(content='Its so hot!')
 menu.add_page(content='Its so cold!')
 ```
 
 #### ReactionMenu.TypeText
 A `TypeText` menu is a text based pagination menu. No embeds are involved in the pagination process, only plain text is used.
 
-![showcase-text](https://cdn.discordapp.com/attachments/655186216060321816/929172629947027466/text_showcase.gif)
+![showcase-text](https://cdn.discordapp.com/attachments/655186216060321816/929172629947027466/text_showcase.gif?ex=663583f2&is=66230ef2&hm=08e5208f0b95dd6d6fc203878fab1a19d32566cf28a32b25e7a4320ce3d4e924&)
 
 #### Stacked Pages
 With `v3.1.0+`, you can paginate with more than just an embed or text. You can combine text, embeds, as well as files. But depending on the `menu_type` the combination can be restricted. Here is an example of a menu with a `menu_type` of `TypeEmbed` that is stacked.
 
 ```py
 # You can use regular commands as well
 @bot.tree.command(description="These are stacked pages", guild=discord.Object(id=...))
@@ -142,15 +142,15 @@
     menu.add_page(discord.Embed(title="Hi, I'm Wumpos!"), files=[discord.File("wumpos.gif")])
     
     menu.add_button(ReactionButton.back())
     menu.add_button(ReactionButton.next())
     
     await menu.start()
 ```
-![stacked](https://cdn.discordapp.com/attachments/655186216060321816/955966821268332554/stacked.gif)
+![stacked](https://cdn.discordapp.com/attachments/655186216060321816/955966821268332554/stacked.gif?ex=66317a7b&is=661f057b&hm=06c4a45634f7471fbfdee81d3fb18cef4390bdc01740c304ea6ef000396adf06&)
 
 Since the `menu_type` is `TypeEmbed`, there always has to be an embed on each page. If the `menu_type` was `TypeText`, embeds aren't allowed and you will be restricted to only using the `files` parameter.
 
 #### ReactionMenu.TypeEmbedDynamic
 A dynamic menu is used when you do not know how much information will be applied to the menu. For example, if you were to request information from a database, that information can always change. You query something and you might get 1,500 results back, and the next maybe only 800. A dynamic menu pieces all this information together for you and adds it to an embed page by rows of data. `ReactionMenu.add_row()` is best used in some sort of `Iterable` where everything can be looped through, but only add the amount of data you want to the menu page.
 > **NOTE:** In a dynamic menu, all added data is placed in the description section of an embed. If you choose to use a `custom_embed`, all text in the description will be overridden with the data you add
 * Associated methods
@@ -468,15 +468,15 @@
 ## ViewMenu
 ```
 class reactionmenu.ViewMenu(method: Union[Context, discord.Interaction], /, *, menu_type: MenuType, **kwargs)
 ```
 
 A `ViewMenu` is a menu that uses discords Buttons feature. With buttons, you can enable and disable them, set a certain color for them with emojis, have buttons that send hidden messages, and add hyperlinks. This library offers a broader range of functionalities such as who pressed the button, how many times it was pressed and more. It uses views (`discord.ui.View`) to implement the Buttons functionality, but uses some of its own methods in order to make a Button pagination menu simple.
 
-![image](https://cdn.discordapp.com/attachments/655186216060321816/855818139450081280/buttons_showcase_reduced.gif)
+![image](https://cdn.discordapp.com/attachments/655186216060321816/855818139450081280/buttons_showcase_reduced.gif?ex=662d0d40&is=661a9840&hm=c27d8af03d464b3bb3942831c1f592042752aeb0baf903a3dbbffee7caade991&)
 
 <details>
   <summary><b>Click to show ViewMenu documentation</b></summary>
 
 
 ### How to import
 ```py
@@ -536,15 +536,15 @@
 menu.add_page(content='Its so hot!')
 menu.add_page(content='Its so cold!')
 ```
 
 #### ViewMenu.TypeText
 A `TypeText` menu is a text based pagination menu. No embeds are involved in the pagination process, only plain text is used.
 
-![text_view_showcase](https://cdn.discordapp.com/attachments/655186216060321816/929744985656549386/text_view_showcase.gif)
+![text_view_showcase](https://cdn.discordapp.com/attachments/655186216060321816/929744985656549386/text_view_showcase.gif?ex=66247b3e&is=662329be&hm=b94fa63761dee697cf4ce0a2e488e8a8119e65b9264d1178d64d8e26e944da91&)
 
 #### Stacked Pages
 With `v3.1.0+`, you can paginate with more than just an embed or text. You can combine text, embeds, as well as files. But depending on the `menu_type` the combination can be restricted. Here is an example of a menu with a `menu_type` of `TypeEmbed` that is stacked.
 
 ```py
 # You can use regular commands as well
 @bot.tree.command(description="These are stacked pages", guild=discord.Object(id=...))
@@ -556,15 +556,15 @@
     menu.add_page(discord.Embed(title="Hi, I'm Wumpos!"), files=[discord.File("wumpos.gif")])
     
     menu.add_button(ViewButton.back())
     menu.add_button(ViewButton.next())
     
     await menu.start()
 ```
-![stacked_view](https://cdn.discordapp.com/attachments/655186216060321816/955983620038860910/stacked_view.gif)
+![stacked_view](https://cdn.discordapp.com/attachments/655186216060321816/955983620038860910/stacked_view.gif?ex=66318a20&is=661f1520&hm=dc93e797cb16a1e3f87f36e02fa40b2733a40a1d469b7f1337d34d6037dad06e&)
 
 Since the `menu_type` is `TypeEmbed`, there always has to be an embed on each page. If the `menu_type` was `TypeText`, embeds aren't allowed and you will be restricted to only using the `files` parameter.
 
 #### ViewMenu.TypeEmbedDynamic
 A dynamic menu is used when you do not know how much information will be applied to the menu. For example, if you were to request information from a database, that information can always change. You query something and you might get 1,500 results back, and the next maybe only 800. A dynamic menu pieces all this information together for you and adds it to an embed page by rows of data. `ViewMenu.add_row()` is best used in some sort of `Iterable` where everything can be looped through, but only add the amount of data you want to the menu page.
 > **NOTE:** In a dynamic menu, all added data is placed in the description section of an embed. If you choose to use a `custom_embed`, all text in the description will be overridden with the data you add
 * Associated methods
@@ -715,17 +715,18 @@
 ```
 ---
 > **NOTE:** When it comes to buttons with a `custom_id` of `ViewButton.ID_CALLER`, `ViewButton.ID_SEND_MESSAGE`, `ViewButton.ID_CUSTOM_EMBED`, or link buttons, you can add as many as you'd like as long as in total it's 25 buttons or less. For all other button ID's, each menu can only have one.
 
 ### Using Selects
 Selects are used when you'd like to categorize information in your menu. Selects can only be used when the menu's `menu_type` is `TypeEmbed`. You should keep in mind that discords limitations on how many menu UI items (rows) can be applied to each message.
 
-![select_showcase](https://cdn.discordapp.com/attachments/655186216060321816/971361708121653268/select_showcase.gif)
+![select_showcase](https://cdn.discordapp.com/attachments/655186216060321816/971361708121653268/select_showcase.gif?ex=66321d16&is=661fa816&hm=f5a668a33715d0d5c77eb7c2a8ec9d01ef14b21c2d2f200c97d12ba70a7ab2bd&)
 
 * Associated Methods
+  * `Page.from_embeds(embeds: Sequence[Embed])` 
   * `ViewMenu.add_select(select: ViewSelect)`
   * `ViewMenu.remove_select(select: ViewSelect)`
   * `ViewMenu.remove_all_selects()`
   * `ViewMenu.disable_select(select: ViewSelect)`
   * `ViewMenu.disable_all_selects()`
   * `ViewMenu.enable_select(select: ViewSelect)`
   * `ViewMenu.enable_all_selects()`
@@ -735,14 +736,15 @@
 ```py
 from reactionmenu import ViewMenu, ViewSelect, Page
 
 menu = ViewMenu(ctx, menu_type=ViewMenu.TypeEmbed)
 menu.add_page(discord.Embed(title="A showcase of console video games", color=discord.Color.blurple()))
 
 menu.add_select(ViewSelect(title="Console Video Games", options={
+    # NOTE: The discord.SelectOption parameter "default" cannot be set to True
     discord.SelectOption(label="PlayStation", emoji="<:PlayStation:549638412538478602>") : [
         Page(embed=discord.Embed(title="Ratchet & Clank", description=..., color=discord.Color.yellow()).set_image(url=...)),
         Page(embed=discord.Embed(title="God of War", description=..., color=discord.Color.blue()).set_image(url=...))
     ],
     discord.SelectOption(label="Xbox", emoji="<:Xbox:501880493285834752>") : [
         Page(embed=discord.Embed(title="Halo Infinite", description=..., color=discord.Color.green()).set_image(url=...)),
         Page(embed=discord.Embed(title="Gears of War 4", description=..., color=discord.Color.red()).set_image(url=...))
@@ -753,15 +755,15 @@
 menu.add_button(ViewButton.next())
 await menu.start()
 ```
 
 #### Go to page navigation
 You can use this type of select when you'd like to use the UI to select a page to go to.
 
-![goto_showcase](https://cdn.discordapp.com/attachments/655186216060321816/973629631905300501/Discord_6SP5AjoOOM.gif)
+![goto_showcase](https://cdn.discordapp.com/attachments/655186216060321816/973629631905300501/Discord_6SP5AjoOOM.gif?ex=663122c1&is=661eadc1&hm=a14135c7fa1c0b9c901b8216cbee7e77435fa1ba3148767d1870d52ba625001e&)
 
 * Associated methods
   * `ViewMenu.add_go_to_select(goto: ViewSelect.GoTo)`
   * `ViewMenu.enable_go_to_select(goto: ViewSelect.GoTo)`
   * `ViewMenu.enable_all_go_to_selects()`
   * `ViewMenu.disable_go_to_select(goto: ViewSelect.GoTo)`
   * `ViewMenu.disable_all_go_to_selects()`
```

