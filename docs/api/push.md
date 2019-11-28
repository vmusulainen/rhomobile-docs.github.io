---
id: push
title: Push
sidebar_label: Push
---
The Push API provides access to Push messaging functionality. Use this API to give your application the ability to receive server initiated messages.
## Instance Properties
### `pushAppName`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Application name used by RhoConnect Push server to identify application.
### `pushServer`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

URL of RhoConnect Push server.
### `type`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Push engine type.
### `userNotifyMode`: string
<span style="font-size:smaller">Languages: Ruby</span><br/><span style="font-size:smaller">Platforms: Android</span><br/><span style="font-size: smaller">Parameters:

UI notification mode. Use `Rho.Notification` instead.
## Instance Methods
### `enumerate`: array
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns the push API objects configured within the application.


### `getDeviceId`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns push token used to identify particular device.


### `startNotifications`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Start listening for push messages, errors or other push related events.


### `stopNotifications`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Stop listening push events.


