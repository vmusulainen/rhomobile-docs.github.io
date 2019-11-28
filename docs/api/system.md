---
id: system
title: System
sidebar_label: System
---
The System API is used to control and modify core aspects of the device such as the screen, OS and device capabilities.
## Static Properties
### `NodejsServerPort`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Port of the local (embedded) Node.js HTTP server if it started (only for Node.js type applications).
### `applicationIconBadge`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: iOS</span><br/><span style="font-size: smaller">Parameters:

Set the application icon to have this badge number. Set to 0 (zero) to remove badge.
### `country`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Current device country code.
### `deviceName`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Name of device application running on. Examples: '9000' (BB), 'iPhone', 'dream' (Android). In Consumer Android device, name of the Industrial Design along with manufacturer name shall be shown. 
### `deviceOwnerEmail`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android</span><br/><span style="font-size: smaller">Read Only</span>

Primary email of phone owner. To access this property 'pim' capability must be enabled in your build.yml.
### `deviceOwnerName`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android</span><br/><span style="font-size: smaller">Read Only</span>

Name(account name) of phone owner. To access this property 'pim' capability must be enabled in your build.yml.
### `devicePushId`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Push notifications device ID which may be used to receive push messages.To get this ID , Push service should be configured on the device. Please refer to Push documentation.
### `externalStorageDirectoryPath`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android</span><br/><span style="font-size: smaller">Read Only</span>

Return the primary shared/external storage directory. This directory may not currently be accessible if it has been mounted by the user on their computer, has been removed from the device, or some other problem has happened.
### `freeServerPort`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Get free local server port, available for binding.
### `hasCalendar`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Returns true if calendar support is available.
### `hasCamera`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, CE, iOS, WM</span><br/><span style="font-size: smaller">Read Only</span>

Returns true if there is a camera available on the device.
### `hasCellNetwork`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Use Network.hasCellNetwork to tell if device is connected to the cell network.
### `hasNetwork`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Use Network.hasNetwork to tell if the device is connected to the network.
### `hasSqlite`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Returns true if the device has sqlite capabilities (previously only BlackBerry did not support this).
### `hasTouchscreen`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Returns true if the device has touch screen capabilities.  For Win32 desktop builds this API will return whether mouse support is available.
### `hasWifiNetwork`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Use Network.hasWifiNetwork to tell if the device is connected to the wifi network.
### `httpProxyURI`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, Win32, WM</span><br/><span style="font-size: smaller">Parameters:

Set HTTP proxy parameters for using the Network module. Example: 'user:password@url:port'. Supports basic authentication only. Do not include 'http://'. Setting this property overrides http_proxy_uri, http_proxy_host, http_proxy_port, http_proxy_user and http_proxy_password. Proxy settings for Windows Mobile/CE with Zebra WebKit should be configured in the config.xml file.
### `isEmulator`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Returns true if the application is running on a platform emulator.
### `isRhoSimulator`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Returns true if the application is running on RhoSimulator.
### `isSymbolDevice`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Returns true if the device supports Symbol device capabilities. APIs will indicate if the property or method is available on Symbol devices only. You can use this property to help your application decide when to take advantage of advanced Symbol capabilities.
### `keyboardState`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: WM</span><br/><span style="font-size: smaller">Parameters:

For Windows Mobile and Windows CE the keyboard can be manually shown or hidden as required. All other platforms only support 'automatic'. The default state for Windows Mobile and Windows CE is manual, for all other platforms it is automatic.
### `localServerPort`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Port of the local (embedded) HTTP server. This parameter is mainly for debug purposes. If not specified, the platform will detect a free port on the device and use that one.
### `locale`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Current device locale Like 'en', 'ru' etc.
### `lockWindowSize`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Win32</span><br/><span style="font-size: smaller">Parameters:

Lock / unlock the window size change by the user. When running on RhoSimulator, this method is supported only for Windows OS.
### `main_window_closed`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

It is internal property for using in debugger (signal for main window close).
### `oemInfo`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, CE, WM</span><br/><span style="font-size: smaller">Read Only</span>

The OEM Information string for the terminal.
### `osVersion`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Version OS of device. Examples:  '4.1' (Android).
### `phoneId`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, CE, iOS, WM</span><br/><span style="font-size: smaller">Read Only</span>

Hardware based ID. It depends on capabilities configured for an application and has to remain same even across application uninstall/install.(except iOS ! - on iOS unisntall/reinstall will update this property - used UIDebice.identifierForVendor)
### `platform`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Platform where application is running.
### `ppiX`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Horizontal PPI (Pixels Per Inch).
### `ppiY`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Vertical PPI (Pixels Per Inch).
### `realScreenHeight`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Screen height in real pixels.
### `realScreenWidth`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Screen width in real pixels.
### `screenAutoRotate`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS</span><br/><span style="font-size: smaller">Parameters:

Screen auto rotate.
### `screenHeight`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Screen height in logical pixels (used for set coordinates).
### `screenOrientation`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Current screen orientation.
### `screenSleeping`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS</span><br/><span style="font-size: smaller">Parameters:

If true, then screen will go to sleep by system inactivity timeout. If false then screen never go to sleep while application is in foreground.
### `screenWidth`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Screen width in logical pixels (used for set coordinates).
### `uuid`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, CE, WM</span><br/><span style="font-size: smaller">Read Only</span>

The Unique Unit IDentifier for the terminal.
### `webviewFramework`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Browser framework identity string.
## Static Methods
### `applicationInstall`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, Win32, WM</span>
#### Description
Install an application.

#### Parameters
applicationUrl: string
### `applicationUninstall`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, Win32, WM</span>
#### Description
Uninstall the application. Not Supported on Windows CE devices.

#### Parameters
applicationName: string
### `bringToFront`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: WM</span>
#### Description
Bring application window to the top of the screen.


### `clearNetworkStatusNotify`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Use Network.clearStatusNotify: Clear network status callback.


### `deleteFolder`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Delete folder.

#### Parameters
pathToFolder: string
### `deleteRegistrySetting`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: WM</span>
#### Description
Deletes the specified value from the device registry. Only applicable on Windows Mobile / Embedded Handheld and CE devices. When running on RhoSimulator, this method is supported only for Windows OS.

#### Parameters
propertyMap: hash

hive: string

key: string

setting: string

persistent: boolean
### `exit`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Use Application.quit: exit application.


### `getRegistrySetting`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: WM</span>
#### Description
Retrieve a value from the device registry. Only applicable on Windows Mobile / Embedded Handheld and CE devices. When running on RhoSimulator, this method is supported only for Windows OS.

#### Parameters
propertyMap: hash

hive: string

key: string

setting: string
### `getStartParams`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, CE, Win32, WM</span>
#### Description
Return the command line parameters. At Android start parameters are returned as URL query string starting with '?', name-value delimiter '=' and name value pairs delimiter '&amp;'.


### `getSystemInfo`: hash
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS</span>
#### Description
Gathers system dependent information ( hw info, installed packages etc ). Return key/value pairs depend on platform.


### `get_locale`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Use System.locale property: Current device locale.


### `hideSplashScreen`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android</span>
#### Description
Hide Splash Screen if delay is configured as -1 in rhoconfig.txt


### `isApplicationInstalled`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, Win32, WM</span>
#### Description
Checks if the specified applicationName is installed on the device.

#### Parameters
applicationName: string
### `isBlobAttr`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Use Database.SQLite3.isBlobAttr: is model attribute is blob.

#### Parameters
partition: string

sourceID: integer

attrName: string
### `openUrl`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Open the application associated with the URL. Behavior may be different on different platforms and depend on installed software. For example, open URL with http:// prefix will execute the Web Browser installed on system and open URL in executed browser. Note: For opening pdf files on android devices it is necessary to add option "no_compression: [ pdf ]" to android section in build.yml. In android, "sms:","mailto:","tel:","http:","https:","file:" are supported. For file url the proper permission and path has to be given. For external storage space fully qualified path has to be given.(Example:-file:///storage/sdcard/sample.jpg).  Hence only external storage space and userFolder are supported for file uri in android.                

#### Parameters
url: string
### `replaceCurrentBundle`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Replace application bundle.

#### Parameters
pathToBundle: string

params: hash

do_not_restart_app: boolean
### `runApplication`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, Win32, WM</span>
#### Description
Run an application.

#### Parameters
appName: string

params: string

blockingCall: boolean
### `setDoNotBackupAttribute`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: iOS</span>
#### Description
Set do not backup attribute for file.

#### Parameters
pathToFile: string

doNotBackup: boolean
### `setNetworkStatusNotify`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Use Network.setStatusNotify: set network notification callback.

#### Parameters
url: string

poll_interval: integer
### `setPushNotification`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Use Push.setPushNotification: Register push callback, the method to call upon receiving a push message.

#### Parameters
url: string

url_params: string

push_client: string
### `setRegistrySetting`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: WM</span>
#### Description
Set a value in the device registry. Only applicable on Windows Mobile / Embedded Handheld and CE devices. When running on RhoSimulator, this method is supported only for Windows OS.

#### Parameters
propertyMap: hash

hive: string

type: string

key: string

setting: string

value: string

persistent: boolean
### `setScreenRotationNotification`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WM</span>
#### Description
Use ScreenOrientation.setScreenOrientationEvent: Notify (call a callback method) when the screen rotates.

#### Parameters
url: string

url_params: string
### `setWindowFrame`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Win32</span>
#### Description
Change application window position and size.

#### Parameters
x: integer

y: integer

width: integer

height: integer
### `setWindowPosition`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Win32</span>
#### Description
Change application window position.

#### Parameters
x: integer

y: integer
### `setWindowSize`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Win32</span>
#### Description
Change application window size.

#### Parameters
width: integer

height: integer
### `set_application_icon_badge`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: iOS</span>
#### Description
Use System.applicationIconBadge: Set the application icon to have this badge number. Set to 0 (zero) to remove badge.iOS only.

#### Parameters
badgeNumber: integer
### `set_http_proxy_url`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: CE, WIN32, WM</span>
#### Description
Use System.httpProxyURI property: To use client with the HTTP proxy.

#### Parameters
proxyURI: string
### `set_locale`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Use Application.setLocale method: set application specific locale.

#### Parameters
locale_code: string

country_code: string
### `set_sleeping`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Use System.screenSleeping property: enable / disable phone sleeping.

#### Parameters
enable: boolean
### `startTimer`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Start timer. (It's works only with Ruby)

#### Parameters
interval: integer

url: string

url_params: string
### `stopTimer`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Stop timer. (It's works only with Ruby)

#### Parameters
url: string
### `unset_http_proxy`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: CE, WIN32, WM</span>
#### Description
Use System.httpProxyURI property: Stop using HTTP proxy that was set by the command line, rhoconfig.txt or set_http_proxy_url.


### `unzipFile`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Unzip file.

#### Parameters
localPathToZip: string

password: string

outputFileName: string
### `updateBlobAttribs`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Use Database.updateBlobAttribs: update model blob attributes list.

#### Parameters
partition: string

sourceID: integer
### `zipFile`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Zip one file. Zip archive must placed to the folder where application can write files. 

#### Parameters
localPathToZip: string

localPathToFile: string

password: string
### `zipFiles`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Zip list of files.

#### Parameters
localPathToZip: string

basePath: string

filePathsToZip: array

password: string
