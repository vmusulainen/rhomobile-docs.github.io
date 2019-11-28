---
id: nativetabbar
title: NativeTabbar
sidebar_label: NativeTabbar
---
The NativeTabbar methods let you use multiple instances of the RhoMobile webview in separate tabs. 
## Static Methods
### `create`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Removes the current tabbar and replaces it with this one. Callback will be called when tab is switched.  Whilst the actual number of tabs you can create will depend on the memory available on your device there is an absolute upper limit of 30 tabs in any one application.

#### Parameters
tabElements: array

tabElement: hash

label: string

action: string

icon: string

reload: boolean

selectedColor: integer

disabled: boolean

backgroundColor: integer

useCurrentViewForTab: boolean

perishable: boolean

createOnInit: boolean

tabBarProperties: hash

verticalOrientation: boolean

backgroundColor: integer

hiddenTabs: boolean

createOnInit: boolean

placeTabsBottom: boolean

invisibleTabControl: boolean
### `currentTabIndex`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns the current tab 0-based index.


### `isCreated`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
If Tabbar already created.


### `remove`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Removes all tabbar except the default tabbar whose index value is 0. Does nothing if there is no active tabbar other than tab 0.


### `removeTab`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: WM</span>
#### Description
Removes the Tab by index. Method will remove the WebView for the specific tab, it will not remove the tab from the tab array, so all indexes will remain the same.You cannot delete the tab with useCurrentViewForTab flag.If you switch to previously removed tab, tab will be recreated.

#### Parameters
tabIndex: integer
### `setTabBadge`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: iOS</span>
#### Description
Set the iPhone badge to tab.

#### Parameters
tabIndex: integer

badge: string
### `switchTab`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Switch active tab.

#### Parameters
tabIndex: integer
