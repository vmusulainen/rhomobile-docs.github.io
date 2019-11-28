---
id: newormmodel
title: NewORMModel
sidebar_label: NewORMModel
---
NewORMModel CoreAPI module
## Instance Properties
### `associations`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Parameters:

Returns model's associations.
### `fixed_schema`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Parameters:

Returns true if the model's type is of fixed schema.
### `freezed`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Parameters:

Returns true if the model is frozen.
### `loaded`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Parameters:

Returns true if model is loaded.
### `model_name`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Parameters:

Returns model's name.
### `partition`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Parameters:

Returns model's Db partition.
### `source_id`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Parameters:

Returns model's source_id.
### `sync_priority`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Parameters:

This number determines the order in which the models are processed and synchronised. Priority starts from lower value 1. Lower the number, higher is the priority. Default value is 1000.
### `sync_type`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Parameters:

Returns model's Sync type.
## Instance Methods
### `anyChangedObjects`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Checks whether the model has any changed objects.


### `buildComplexWhereCond`: array
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Aux function.

#### Parameters
attrKey: string

attrValues: array

valOp: string

valFunc: string
### `buildFindLimits`: hash
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Aux function.

#### Parameters
whatArg: string

hashArgs: hash
### `buildFindOrder`: hash
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Aux function.

#### Parameters
order_attrs: array

order_ops: array
### `buildFindOrderString`: hash
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Aux function. Internally used to make order string.

#### Parameters
order_attrs: array

order_ops: array
### `buildSimpleWhereCond`: array
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Aux function.

#### Parameters
what: string

conditions: array
### `canModify`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Checks whether the object can be modified.

#### Parameters
objId: string
### `can_modify`: boolean
<span style="font-size:smaller">Languages: Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Checks whether the object can be modified.

#### Parameters
objId: string
### `changed?`: boolean
<span style="font-size:smaller">Languages: Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns true if a Rhodes model object has local database changes that need to be synchronized, false otherwise.


### `clear`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
This method clears all the models and the associated tables with the models. It is used only for testing purpose and not for the developing.


### `client_id`: string
<span style="font-size:smaller">Languages: Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns the current sync client id.


### `count`: integer
<span style="font-size:smaller">Languages: Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns the number of objects in the named model.


### `create`: object
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Create a new Rhodes model object and save it to the database. This is the fastest way to insert a single item into the database.

#### Parameters
attrs: hash
### `createInstance`: hash
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Creates model's instance and initializes model's object but doesn't store it in DB.

#### Parameters
attrs: hash
### `createObject`: hash
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Initializes model's object and stores it in the DB.

#### Parameters
attrs: hash
### `deleteAll`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Delete all Rhodes model objects for a source filtering by conditions. This method accepts parameters as key-value pairs. It accept conditions as a parameter.

#### Parameters
params: hash

conditions: hash
### `deleteObject`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Deletes object's attributes from the DB.

#### Parameters
objId: string
### `deleteObjects`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Deletes all object's according to the specified conditions.It is applicable only for Fixed_schema Model.

#### Parameters
strOptions: hash

quests: array
### `deleteObjectsPropertyBagByCondArray`: array
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Deletes all objects for the given Property Bag model according to the specified conditions. It is applicable only for Property bag Model.

#### Parameters
conditions: string

quests: array

strOptions: hash
### `deleteObjectsPropertyBagByCondHash`: array
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Deletes all objects for the given Property Bag model according to the specified conditions. It is applicable only for Property bag Model.

#### Parameters
conditions: hash

strOptions: hash
### `delete_all`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Delete all Rhodes model objects for a source filtering by conditions. This method accepts parameters as key-value pairs. It accepts 2 keys- conditions and op.

#### Parameters
params: hash

conditions: hash or array
### `destroy`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Destroys model's instance.


### `enable`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Sets model's Boolean property to true (enables model's property)

#### Parameters
propertyName: string
### `enumerate`: array
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
enumerate method returns array of ORMModel objects.


### `find`: array
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Find model objects.

#### Parameters
queryType: string

queryOptions: hash

conditions: hash or array

propertyName: 

propertyValue: 

order: string or array

orderdir: string or array

select: array
### `findObjects`: array
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns array of objects for the given model queried according to the specified conditions. It is applicable only for Fixed_schema Model.

#### Parameters
whatParam: string

strOptions: hash

quests: array

selectAttrs: array

orderAttrs: array
### `findObjectsPropertyBagByCondArray`: array
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns array of objects for the given Property Bag model queried according to the specified conditions. It is applicable only for Property bag Model.

#### Parameters
whatParam: string

conditions: string

quests: array

strOptions: hash

selectAttrs: array
### `findObjectsPropertyBagByCondHash`: array
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns array of objects for the given Property Bag model queried according to the specified conditions. It is applicable only for Property bag Model.

#### Parameters
whatParam: string

conditions: hash

strOptions: hash

selectAttrs: array
### `find_all`: hash
<span style="font-size:smaller">Languages: Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
find('all') replaces the legacy ruby method find_all.


### `find_by_sql`: array
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns array of objects for the given model queried according to the specified SQL.

#### Parameters
sqlQuery: string
### `get`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Get the value of a property of the current model.Ex: myModel.get('name'); See also the vars() method.

#### Parameters
propertyName: string
### `getBackendRefreshTime`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns time string when the source has been synced.


### `getBelongsTo`: array
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns info about model's relationships with other models.

#### Parameters
propertyName: string
### `getCount`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns total number of objects for the model.


### `getModel`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
getModel method returns instance of the ORMModel.

#### Parameters
modelName: string
### `getModelProperty`: hash
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns info about model's field property.

#### Parameters
propertyName: string
### `get_source_id`: hash
<span style="font-size:smaller">Languages: Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns the source id number for this Rhodes model object.                    Please use the model property source_id.


### `get_source_name`: hash
<span style="font-size:smaller">Languages: Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns the source name for this Rhodes model object.                    Please use the model property model_name.


### `has`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns true if the model has the propertyName given.

#### Parameters
propertyName: string
### `hasChanges`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Checks whether the object has any changes. Returns true when an object is created or updated.

#### Parameters
objId: string
### `init`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Initializes new model's instance.

#### Parameters
modelName: string
### `initModel`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Initializes model's internal DB.


### `make`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Create a new ORM model object JavaScript reference but does not save it to the database. To save this reference to the database, you will need to execute the .save() method.


### `new`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Initializes new model's instance.

#### Parameters
modelName: string
### `onSyncCreateError`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Handles sync create errors.

#### Parameters
objects: array

action: string
### `onSyncDeleteError`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Handles sync delete errors for the object.

#### Parameters
objId: string

attrHash: hash

action: string
### `onSyncUpdateError`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Handles sync update errors for the object.

#### Parameters
objId: string

attrHash: hash

rollbackHash: hash

action: string
### `paginate`: array
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
 The paginate method takes care of setting the proper page limit and offset when a large number of records are fetched. This method accepts parameters as key-value pairs.                

#### Parameters
params: hash

page: integer

per_page: integer

conditions: array or hash

order: string or array

orderdir: string or array

select: string
### `pushChanges`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Pushes all changes for the source. For details [push_changes](api/rhom-api#pushchanges)


### `push_changes`
<span style="font-size:smaller">Languages: Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Pushes all changes for the source.


### `save`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Saves the object's attributes in the DB.


### `saveObject`: hash
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Saves (creates if necessary or updates if already exists) object's attributes in the DB.

#### Parameters
objId: string

attrs: hash
### `set`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Sets model's property to value with additional processing for :sync property.

#### Parameters
propertyName: string

partition: string

sync_type: string

sync_priority: integer

freezed: boolean

schema_version: float

propertyValue: string
### `setBelongsTo`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Using this method, you can set sync association between models. For details [Associations](guide/rhom_ruby#associations)

#### Parameters
propertyName: string

sourceName: string
### `setModelProperty`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Initializes new model's field property.

#### Parameters
propertyName: string

propertyType: string

propOption: string
### `setSchemaIndex`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Initializes new model's schema index.

#### Parameters
indexName: string

indexCols: array

is_unique: boolean
### `updateAttributes`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Updates the current Rho model object attributes and saves it to the database. This is the fastest way to add or update model attributes.

#### Parameters
attributes: hash
### `updateObject`: hash
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Updates object's attributes in the DB.

#### Parameters
objId: string

oldAttrs: hash

newAttrs: hash
### `update_attributes`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Updates the current Rho model object attributes and saves it to the database. This is the fastest way to add or update model attributes.

#### Parameters
attributes: hash
### `validateFreezedAttribute`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Validates object's frozen attribute.

#### Parameters
attrName: string
### `validateFreezedAttributes`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Validates all object's frozen attributes.

#### Parameters
attrHash: hash
### `vars`: hash
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns an object containing all propertyName and values for the model. You can use myModel.vars().name instead of myModel.get('name').


