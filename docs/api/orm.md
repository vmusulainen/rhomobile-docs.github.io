---
id: orm
title: ORM
sidebar_label: ORM
---
This JavaScript API class allows you to interact with the local RHOM database and programatically add models or get references to models.
## Static Methods
### `addModel`: model
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Creates an ORM model reference.

#### Parameters
Anoynomous Function methods: 

modelName("value"): string

enable("value"): string

property("name","type"): string,string

name: string

type: string

addIndex("name",[colArray]): string, array

name: string

colArray: array

addUniqueIndex("name",[colArray]): string, array

name: string

colArray: array

belongs_to("name"): string

set(property,value): string,value

partition: string

sync_type: string

sync_priority: integer
### `databaseFullReset`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Deletes all records from the property bag and model tables.

#### Parameters
resetClientInfo: boolean

resetLocalModels: boolean
### `databaseFullResetAndLogout`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Deletes all records from the property bag and model tables. Logout the user from RhoConnectClient. For examples, see Resetting the Database in Using the Local Database with ORM.


### `databaseFullResetEx`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Deletes all records from the property bag and model tables for the model names passed in parameters.

#### Parameters
propertyMap: hash

models: array

reset_client_info: boolean

reset_local_models: boolean
### `databaseFullclientResetAndLogout`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Deletes all records from the property bag and model tables. Logout the user from RhoConnectClient and erase all RhoConnectClient device information. Equivalent to ORM::ORM.databaseFullReset(true) followed by RhoConnectClient.logout.


### `databaseLocalReset`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Reset only local (non-sync-enabled) models.


### `export`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Export db.


### `getClientId`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns the current sync client id.


### `getModel`: model
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns a model.

#### Parameters
modelName: string
### `haveLocalChanges`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns true if any of the Rhodes model objects have local database changes that need to be synchronized, false otherwise.


### `import`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Import db.

#### Parameters
zipName: string
