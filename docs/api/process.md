---
id: process
title: Process
sidebar_label: Process
---
This API is used to either navigate to a URL or call a javascript function when an attached card reader decodes data. Only the foreground application is given access to the card reader hardware, when an application is sent to the background its state will be saved and it will automatically relinquish control of the card reader. When brought back to the foreground, an application previously using the card reader will have its previous configuration (eg. pinTimeout) reapplied to the card reader automatically.
## Instance Methods
### `closeHandle`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Close process handle.


### `getProcessExitCode`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
GetProcessExitCode.


### `runApplication`: self_instance
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Run an application.

#### Parameters
appName: string

params: string

blockingCall: boolean
### `waitForApplication`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
WaitForApplication.


