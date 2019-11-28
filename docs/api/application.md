---
id: application
title: Application
sidebar_label: Application
---
The Application class is used for accessing or setting application level configuration settings.
## Static Properties
### `appBundleFolder`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Path to apps/app folder inside the application bundle.
### `appName`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Application name.
### `appsBundleFolder`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Path to apps folder inside the application bundle.
### `badLinkURI`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: WM</span><br/><span style="font-size: smaller">Read Only</span>

Bad link URI to navigate in browser. This is defined in config.xml: Navigation\\BadLinkURI.
### `bundleFolder`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Path to application bundle folder.
### `configPath`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Path to the configuration file.
### `country`: string
<span style="font-size:smaller">Languages: Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Current application country code.
### `databaseBlobFolder`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Path to folder where the database blob files are stored. Blobs are usually images or binary files. In the ORM Model you would specify that the attribute is of type blob Ex. When capturing an image, the actual file is saved in the databaseBlobFolder.
### `defaultNativeMenu`: array
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, CE, Win32, WM, WP8</span><br/><span style="font-size: smaller">Read Only</span>

Native Menu items.
### `invalidSecurityTokenStartPath`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, CE, iOS, Win32, WM</span><br/><span style="font-size: smaller">Read Only</span>

Page to navigate to in case of check of SecurityToken failed. Can be set in rhoconfig.txt: invalid_security_token_start_path;
### `locale`: string
<span style="font-size:smaller">Languages: Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Current application locale.Like 'en', 'ru' etc.
### `modelsManifestPath`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Path to file with the model list.
### `nativeMenu`: array
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, CE, Win32, WM, WP8</span><br/><span style="font-size: smaller">Parameters:

Native Menu items. To customise the native application menu and controller menu items in ruby follow [Application Menu API](http://docs.rhomobile.com/en/2.2.0/rhodesapi/menu-apis)
### `publicFolder`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Path to the application's public folder.
### `rhoPlatformVersion`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, CE, iOS, Sailfish, UWP, Win32, WM</span><br/><span style="font-size: smaller">Read Only</span>

The version of RhoMobile platform, which was used to build the application.
### `securityTokenNotPassed`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, CE, iOS, Win32, WM</span><br/><span style="font-size: smaller">Read Only</span>

Indicates if the security token check was failed. Security token can be set in build.yml: security_token. Same security token should be passed as command line parameter '-security_token=token_value' to application. If security token check failed : if this page exist then application navigate to it, otherwise application will exit.
### `settingsPageURI`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Parameters:

Settings page URI. Will be used when Options menu or toolbar item is chosen by user.
### `splash`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Splash screen image display options. This a string with several parameters divided by ';': delay=5;center;hcenter;vcenter;vzoom;hzoom;zoom.
### `startURI`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Parameters:

Startup page for your application.
### `title`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Win32, WM</span><br/><span style="font-size: smaller">Parameters:

Define Window caption text. If missed - caption from page used. Not supported on Windows CE devices.
### `userFolder`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Path to folder where the application can write files and create subfolders.
### `version`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Version from build time configuration file (build.yml).
## Static Methods
### `databaseFilePath`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Path to the ORM database file by partition name. Please note that this function does not create a database file. This function only generates the file path based on the application path and partition name.

#### Parameters
partitionName: string
### `expandDatabaseBlobFilePath`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Generates the absolute path to database blob file. Please note that this function does not the create database file. This function only generates the file path based on application path and partition name.

#### Parameters
relativePath: string
### `minimize`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: CE, Win32, WM</span>
#### Description
Minimize or move the application to background. When running in RhoSimulator this method is supported only for Windows OS.


### `modelFolderPath`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Folder of the model by name.

#### Parameters
name: string
### `processApplicationEvent`
<span style="font-size:smaller">Languages: Ruby</span><br/><span style="font-size:smaller">Platforms: Android, CE, iOS, Win32, WM</span>
#### Description
Ruby applications must use this method for processing of the application Event. May be called from setApplicationNotify callback.This method should be called for each event. The only exception is SyncUserChanged, where you can choose your own reset database logic.

#### Parameters
applicationEvent: string

eventData: hash
### `quit`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Quit the application.


### `relativeDatabaseBlobFilePath`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Generates the relative path to database blob file. Please note that this function does not create a database file. This function only generates the file path based on the application path and partition name.

#### Parameters
absolutePath: string
### `restore`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: CE, Win32, WM</span>
#### Description
Restores the application to be in the foreground. When running in RhoSimulator the method is supported only for Windows OS.


### `setApplicationNotify`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, CE, iOS, Win32, WM</span>
#### Description
This method allows your application to register for application specific events like application activation/deactivation, UI creation/destruction as well as others. Check the Callback section for details.


### `setLocale`
<span style="font-size:smaller">Languages: Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Set application specific locale.

#### Parameters
localeCode: string

countryCode: string
