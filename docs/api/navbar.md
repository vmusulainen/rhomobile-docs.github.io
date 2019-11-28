---
id: navbar
title: Navbar
sidebar_label: Navbar
---
The NavBar API supports a native navigation bar for iOS devices.
## Static Methods
### `create`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: iOS</span>
#### Description
Removes the current NavBar and replaces it with this one.

#### Parameters
navBarProperties: hash

left: hash

label: string

action: string

right: hash

label: string

action: string

title: string
### `remove`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: iOS</span>
#### Description
Removes the current navigation bar. Does nothing if there is no active navigation bar.


### `started`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: iOS</span>
#### Description
Return true is navbar is started (used only for automatic tests)


