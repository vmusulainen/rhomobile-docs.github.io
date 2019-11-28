---
id: notification
title: Notification
sidebar_label: Notification
---
The Notification API allows you to provide feedback to the user, either auditory, tactile or visual. Use this API to give a visual popup window, sound the device beeper or illuminate the device LEDs (hardware permitting).
## Static Methods
### `beep`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, Win32, WM</span>
#### Description
If the device is equipped with a beeper then a beep will be emitted. Not supported on iOS devices.

#### Parameters
propertyMap: hash

frequency: integer

volume: integer

duration: integer
### `hidePopup`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, CE, iOS, Win32, WM</span>
#### Description
Closes the current popup window. On Windows Mobile/CE, Windows and RhoSimulators only Status window, displayed by showStatus can be hide.


### `playFile`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WM</span>
#### Description
Play an audio file if that media type is supported by the device.

#### Parameters
path: string

media_type: string
### `removeScheduler`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS</span>
#### Description



### `setScheduler`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS</span>
#### Description


#### Parameters
propertyMap: hash

message: string

title: string

start: hash

hour: integer

minute: integer

seconds: integer

interval: integer

repeats: boolean
### `showPopup`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, CE, iOS, Win32, WM</span>
#### Description
Bring the application up front and show a message in a popup window. The message can be passed as a string or a hash. The popup window closes after you click on one of the buttons in the 'button' array. All custom icons' paths must be absolute paths to the icon file. Icon is not supported on iOS devices.

#### Parameters
propertyMap: hash

message: string

title: string

icon: string

buttons: array

types: array
### `showStatus`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, CE, iOS, Win32, WM</span>
#### Description
Display a window containing a status message. The window closes after the user clicks on its hide button. Note: Android will show a toast message for a short time in addition to a dialog window.

#### Parameters
title: string

status_text: string

hide_button_label: string
### `vibrate`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WM</span>
#### Description
Vibrate the device's pager hardware. Need 'vibrate' capability set at build.yml for Android.

#### Parameters
duration: integer
