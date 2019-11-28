---
id: database
title: Database
sidebar_label: Database
---
Database is low-level API to access SQLite local database.
## Instance Methods
### `close`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Closes the database. The database will not be accessible until it is opened again.


### `commitTransaction`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Commit database transaction. Saves all updates to the database from the start of the transaction.


### `destroyTable`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Destroys a database table.

#### Parameters
tableName: string
### `destroyTables`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Destroy a list of database tables.

#### Parameters
propertyMap: hash

include: array

exclude: array
### `executeBatchSql`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Execute a series of sql statements included in the sqlStmt string parameter.

#### Parameters
sqlStmt: string
### `executeSql`: array
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Execute the sql statement specified in the method's parameters.

#### Parameters
sqlStmt: string

args: array
### `export`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Exports the contents of the current database to a file.


### `import`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Import the contents of the archived database into the current database.

#### Parameters
zipName: string
### `initialize`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
This method is a constructor for this class. Instead of saying Rho.Database.initialize(dbPath,dbPartition) you would use new Rho.Database(dbPath,dbPartition). ex: `var db = new Rho.Database(Rho.Application.databaseFilePath('test'), 'test');` Make sure you issue a `.close()` when you are finished using the database. If the database file does not exist it will be created using a SQL schema: rhodes\platform\shared\db\res\db\syncdb.schema. Do not use predefined partition names: app, user, local. Do not open the same database file in different partitions. Do not use the same partition for different database files. Do not open the same file twice.

#### Parameters
dbPath: string

dbPartition: string
### `isTableExist`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Will return true or false if the specified table exists in the current database.

#### Parameters
tableName: string
### `isUiWaitForDb`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Indicates if UI waiting for DB? Should be used in separate thread, which updates database (implementing custom data sync logic). Will be true when database method calls from Main application thread and waits for database.


### `lockDb`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Lock database. This method should be used to synchronize Database access with RhoConnect client. The startTransaction method also locks the database but if you're going to read from database, lockDb is faster.


### `rollbackTransaction`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Rollback database transaction. This will cancel any pending actions to the database that were executed since the last Start and before a commit.


### `setDoNotBackupAttribute`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: iOS</span>
#### Description
Set "do not backup attribute" for the database file. This is special flag set on files, which will exclude it from iCloud service.

#### Parameters
setFlag: boolean
### `startTransaction`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Start database transaction. All operations will not be the saved to the database until a commit is executed.


### `unlockDb`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Unlock database, previously locked by lockDb.


