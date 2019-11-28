---
id: intent
title: Intent
sidebar_label: Intent
---
The Intent API provides an inter-application broadcast message-passing framework.
## Static Methods
### `send`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Sends an intent. The receiver of the intent can either be another RhoMobile  application that is listening for this Intent characteristic or on Android can be a native Android application setup with an Intent-Filter that will trigger based on the parameters of this method.**Android Note**: On Android, the callback should be used only when the intentType is set to START_ACTIVITY. The only valid way for an Android app to pass a private file from a package directly to another application is to set the 'uri' parameter with content URI: Sample JavaScript:    :::javascript    var params = {        intentType: Rho.Intent.START_ACTIVITY,        action: "ACTION_VIEW",        uri: "content://com.rhomobile.sample/rhodata/apps/public/sample.pdf"    }    Rho.Intent.send(params);In most cases the extension of the exported file also must be added to the 'android:no_compression' list in the `build.yml:`Sample Build.yml    :::ruby    android:      no_compression: ['pdf','html','css']

#### Parameters
params: hash

intentType: string

permission: string

action: string

categories: array

: string

appName: string

targetClass: string

uri: string

mimeType: string

data: hash

createChooser: boolean

chooserTitle: string
### `startListening`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Start listening for custom intents.For Android, this is how we have implemented [Android Intent Filters](http://developer.android.com/guide/components/intents-filters.html#Receiving). In order to listen for Intents you will have to update the `AndroidManifest.erb` file and add a special section to it. This file is now generated with RhoMobile Version 4.1 when you create a new project. The file is located in the root of project.Add the following snippet to AndroidManifest.erb within the `manifest` tags    :::xml    &lt;receiver android:name='com.rho.intent.IntentReceiver'&gt;      &lt;intent-filter&gt;        &lt;action android:name="Intent.ACTION_BATTERY_CHANGED" /&gt;      &lt;/intent-filter&gt;    &lt;/receiver&gt;Notice that this looks very similar to a standard AndroidManifest.XML file section except the `receiver` is the common RhoMobile intent receiver. The `intent-filter` tags within this section are standard AndroidManifest.XML notation that you would put in for the Intent-Filters that you want to listen for. Consult the [Android Docs](http://developer.android.com/guide/components/intents-filters.html#Receiving) for more information about Intent Filters. From your Android application, you would use the [sendBroadcast() method](http://developer.android.com/reference/android/content/Context.html#sendBroadcast(android.content.Intent\)) with the appropriate parameters for this filter.


### `stopListening`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Stop listening for custom intents.


