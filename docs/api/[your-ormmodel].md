---
id: [your-ormmodel]
title: [Your-OrmModel]
sidebar_label: [Your-OrmModel]
---
RhoMobile applications provide automatic JavaScript CRUD methods for any models that you have defined to interact with the database.  You must define a model class by using the [ORM.addModel](Orm#maddModel) method before you can use the API's referenced here.  See [Orm](Orm) to learn about defining and adding a model.All methods here are accessed from the model instance object that you have created. In places where you see `[Your-OrmModel]` on this page, you would use the instance object instead.    :::js    var productModel = Rho.ORM.addModel(function(model){      model.modelName("Product");      model.enable("sync");      model.property("name","string");      model.property("brand","string");      model.property("price","float");      model.set("partition","user");    });    // create model object and save it to database    var product = productModel.create({      brand: 'Apple',      name: 'iPhone5',      price: 199.99});    // read product from database    var product = productModel.find('first');    product.get('brand'); // Apple    product.get('name'); // iPhone5        
## Instance Methods
### `canModify`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns true if the Rhodes model object is not currently being synced (if it is being synced, you should disable editing of the object). Before displaying an edit page for an object, your application can check if the object is currently being accessed by the sync process. If it is, you should disable editing of the object. can_modify could return true, for example, on a new local record that was created and sent to the RhoConnect application, but no response has been received yet.


### `create`: object
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Create a new Rhodes model object and save it to the database. This is the fastest way to insert a single item into the database.

#### Parameters
attributes: hash
### `deleteAll`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Delete all Rhodes model objects for a source.For JavaScript you cannot specify conditions.


### `destroy`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Destroy a Rhodes model object and removes the record from the database.


### `find`: array
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Find model objects.

#### Parameters
queryType: string

queryOptions: hash

conditions: hash

propertyName: 

propertyValue: 

order: string

orderdir: string

select: array
### `get`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Get the value of a property of the current model.Ex: myModel.get('name'); See also the vars() method.

#### Parameters
propertyName: string
### `has`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns true or false if the model has the propertyName given.

#### Parameters
propertyName: string
### `make`: object
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Create a new Rhodes model object JavaScript reference but does not save it to the database. To save this reference to the database, you will need to execute the .save() method. See the ORM new example.

#### Parameters
attributes: hash
### `object`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns the unique ID for the data record. Use this to identify records. You can also use this in a .find() method for retrieving a specific record.


### `save`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Saves the current Rhodes model object to the database.


### `set`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Sets the value of a property of the current model. Ex: myModel.set('name','new name'); This does not save to the database until you execute a myModel.save().

#### Parameters
propertyName: string

propertyValue: string
### `updateAttributes`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Updates the current Rho model object attributes and saves it to the database. This is the fastest way to add or update model attributes.

#### Parameters
attributes: hash
### `vars`: hash
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns an object containing all propertyName and values for the model. You can use myModel.vars().name instead of myModel.get('name').


