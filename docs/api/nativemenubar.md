---
id: nativemenubar
title: NativeMenubar
sidebar_label: NativeMenubar
---
The NativeMenubar API lets you customize the Windows Mobile/CE native menu buttons.
## Static Properties
### `defaultMainMenu`: array
<span style="font-size:smaller">Languages: Ruby</span><br/><span style="font-size:smaller">Platforms: WM</span><br/><span style="font-size: smaller">Read Only</span>

This will return what the default right menu should be. This is a read-only property.
### `extraButton`: hash
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: WM</span><br/><span style="font-size: smaller">Parameters:

Defined behavior of the Left menu button for Windows Mobile applications. This takes the same HASH as a menu item {label: 'Left Button', action: 'alert("You pressed the left button")'}. If your menu is using menu items via mainMenu, then be sure to not set an action for the extraButton. Setting an action for the extraButton will cause the mainMenu setting to be ignored. 
### `extraMenu`: array
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: WM</span><br/><span style="font-size: smaller">Parameters:

The Left menu items for Windows Mobile applications. This defines the list of menu choices when the extraButton is pressed.
### `mainButton`: hash
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: WM</span><br/><span style="font-size: smaller">Parameters:

Defined behavior of the Right menu button for Windows Mobile applications. This takes the same HASH as a menu item {label: 'Right Button', action: 'javascript: alert("You pressed the right button");'}. If your menu is using menu items via mainMenu, then be sure to not set an action for the mainButton. Setting an action for the mainButton will cause the mainMenu setting to be ignored.
### `mainMenu`: array
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: WM</span><br/><span style="font-size: smaller">Parameters:

The Right menu items in Windows Mobile applications. This defines the list of menu choices when the mainButton is pressed.
