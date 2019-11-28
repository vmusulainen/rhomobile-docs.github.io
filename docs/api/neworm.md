---
id: neworm
title: NewORM
sidebar_label: NewORM
---
ORM CoreAPI module
## Instance Methods
### `addModel`: model
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Creates an ORM model reference.

#### Parameters
Anoynomous Function methods: 

enable("value"): string

setModelproperty("name","type","option"): string,string,string

name: string

type: string

option: string

set("property","value"): string,value

partition: string

sync_type: string

sync_priority: integer

freezed: boolean

schema_version: float
### `databaseClientReset`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Resets client info and sync models (optionally, local models as well)

#### Parameters
resetLocalModels: boolean
### `databaseFullReset`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Resets selected models, client info and local models.

#### Parameters
resetClientInfo: boolean

resetLocalModels: boolean
### `databaseFullResetAndLogout`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Resets sync models, client info and local models and does the user logout.


### `databaseFullResetEx`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Resets selected models, client info and local models.

#### Parameters
models: array

resetClientInfo: boolean

resetLocalModels: boolean
### `databaseFullclientResetAndLogout`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Resets sync models, client info and local models and does the user logout.


### `databaseLocalReset`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Resets local database.


### `generateId`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns newly generated unique object Id.


### `getClientId`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns current Client Id.


### `haveLocalChanges`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns TRUE whenever there are any local (non-synced) changes.


### `useNewOrm`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns TRUE if NewORM is enabled in rhoconfig.txt.


