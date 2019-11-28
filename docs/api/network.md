---
id: network
title: Network
sidebar_label: Network
---
This API class allows you to interact with either the WAN or WiFI network of the device.
## Static Properties
### `authPassword`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Parameters:

Password for basic authentication. You must also specify `authType='basic' or `authType='digest'`
### `authType`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Parameters:

Type of authentication used for this request. Check the list of available options below. Leaving blank will result in no authentication type.
### `authUser`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Parameters:

User name for basic authentication. You must also specify `authType='basic'` or `authType='digest'`
### `headers`: hash
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Parameters:

List of HTTP headers to be used in the network  request.
### `httpVerb`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Parameters:

HTTP verb to be used in the network request.
### `responseTimeout`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Parameters:

Timeout of network requests in seconds. This property has module scope. Do not pass it as hash parameter to methods, use property accessors instead.
### `url`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Parameters:

URL of the request. This should be fully formatted URL like http://domain.com/
### `verifyPeerCertificate`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, CE, iOS, Win32, WM</span><br/><span style="font-size: smaller">Parameters:

Verify SSL certificates. When set to false it will allow untrusted certificates.
## Static Methods
### `cancel`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Cancel the request identified by callback. If callback is not specified then all requests will be canceled.                &gt; Note: for JS API: The method cancels all Rho.Network requests and does not accept args.


### `connectWan`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: WM</span>
#### Description
Connects the device to a Wide Area Network. The connection destination must be first configured through the Connection Manager (on the device) and the destination name provided to this method. If a connection is already established, you must first call disconnectWan before attempting another connection. A list of available connection destinations is written to the log file when either connectWan or disconnectWan are first specified. Specify the connection as 'Internet' to use the default internet connection defined on the device. If the specified destination does not exist no connection attempt will be made and an entry will be made in the log file.

#### Parameters
connectionDestination: string
### `detectConnection`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Begins polling the specified host on the specified URL to check if there is a network connection available. The connection status is reported back via the provided callback. Note that callback will be called only if connection status has changed compared to previous polling. Multiple concurrent detectionConnection is not supported.

#### Parameters
propertyMap: hash

host: string

port: integer

pollInterval: integer

detectionTimeout: integer
### `disconnectWan`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: WM</span>
#### Description
Disconnects the current WAN connection. DisconnectWan will only affect connections established by RhoElements so if you have not previously called connectWan this function will have no effect.


### `downloadFile`: hash
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Download a file to the specified filename. Note: if 'overwriteFile' flag is default or false, the HEAD request to the server will be performed before actual download to retrieve 'last-modified' header which is used to support resuming interrupted download. If targeted server doesn't support HEAD requests, 'overwriteFile' should be set to true.

#### Parameters
propertyMap: hash

url: string

filename: string

overwriteFile: boolean

createFolders: boolean
### `get`: hash
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Perform a HTTP GET request.&gt; Note: This method will perform a POST if you send a body with it. If performing a GET, do not add a body to the call.

#### Parameters
propertyMap: hash
### `hasCellNetwork`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WM</span>
#### Description
Returns true if the device is connected to a cell network. Not supported on Windows CE.


### `hasNetwork`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WM</span>
#### Description
Returns true if the device is connected to a network. Not supported on Windows CE.


### `hasWifiNetwork`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WM</span>
#### Description
Returns true if the device is connected to a WiFi network. Not supported on Windows CE.


### `post`: hash
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Perform a HTTP Post.

#### Parameters
propertyMap: hash

body: string
### `startStatusNotify`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WM</span>
#### Description
Start network status notifications. Notifications are sent when WiFi or Cell network appear / disappear. To check real Internet connectivity use detectConnection method. Not supported on Windows CE.

#### Parameters
pollInterval: integer
### `stopDetectingConnection`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Ceases network detection. Callback is no longer supported; it has been made optional to preserve backward compatibility.


### `stopStatusNotify`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WM</span>
#### Description
Stop network status notifications. Not supported on Windows CE.


### `uploadFile`: hash
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Upload the specified file using HTTP POST.

#### Parameters
propertyMap: hash

filename: string

body: string

fileContentType: string

multipart: array

: hash

filename: string

contentType: string

filenameBase: string

name: string
