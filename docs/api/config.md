---
id: config
title: Config
sidebar_label: Config
---
Rho.Config module
## Static Properties
### `configPath`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Parameters:

Path to the config file.
## Instance Methods
### `getPropertyBool`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Get boolean value of config property.

#### Parameters
name: string
### `getPropertyInt`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Get integer value of config property.

#### Parameters
name: string
### `getPropertyString`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Get string value of config property.

#### Parameters
name: string
### `isPropertyExists`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns true if property exists in the loaded config file.

#### Parameters
name: string
### `loadFromFile`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Load config from the file specified by configPath property.


### `removeProperty`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Remove existing property and optionally save changes to file. Remove properties works only with properties that has been set with setProperty*** methods. Properties from config file doesn't changed.

#### Parameters
name: string

saveToFile: boolean
### `setPropertyBool`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Set boolean value of config property and optionally save changes to file. Properties save to separate file, common file (specify with configPath) doesn't change.

#### Parameters
name: string

value: boolean

saveToFile: boolean
### `setPropertyInt`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Set integer value of config property and optionally save changes to file. Properties save to separate file, common file (specify with configPath) doesn't change.

#### Parameters
name: string

value: integer

saveToFile: boolean
### `setPropertyString`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Set string value of config property and optionally save changes to file. Properties save to separate file, common file (specify with configPath) doesn't change.

#### Parameters
name: string

value: string

saveToFile: boolean
