---
id: nativetoolbar
title: NativeToolbar
sidebar_label: NativeToolbar
---
The NativeToolbar method let you create and remove a toolbar at runtime.
## Static Methods
### `create`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Creates a new toolbar and removes the current toolbar and replaces it with this one. Any images used for UI elements should be specified by either an absolute path. i.e. '/sdcard/nmt/blabla.com.bla./data/public/img/button.png'

#### Parameters
toolbarElements: array

toolbarElement: hash

label: string

action: string

icon: string

coloredIcon: boolean

width: integer

toolBarProperties: hash

backgroundColor: integer

maskColor: integer

viewHeight: integer
### `isCreated`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Check if Toolbar already exists.


### `remove`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Removes the current toolbar. Does nothing if there is no active toolbar.


