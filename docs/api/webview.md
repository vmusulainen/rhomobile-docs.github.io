---
id: webview
title: WebView
sidebar_label: WebView
---
The `Webview` is the core container used for rendering your application code. You can control certain behaviors of the webview by using this API class.
## Static Properties
### `acceptLanguage`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: WM</span><br/><span style="font-size: smaller">Parameters:

Configurable HTTP headers. Not yet implemented.
### `activeTab`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Return an active tab index. For change active tab use Use Rho.NativeTabbar.currentTab property.
### `cacheSize`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: WM</span><br/><span style="font-size: smaller">Read Only</span>

The browser cache size, in whole MBs. Defines in config.xml: Navigation\\Cache.
### `enableCache`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android</span><br/><span style="font-size: smaller">Read Only</span>

Enable / disable Browser cache. Use 'WebView.enableCache' parameter in rhoconfig.txt to configure this value.
### `enableDragAndDrop`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: iOS</span><br/><span style="font-size: smaller">Parameters:

enable drag and drop operations for iOS &gt;= 11.0
### `enableMediaPlaybackWithoutGesture`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android</span><br/><span style="font-size: smaller">Read Only</span>

Enable Media playback without gesture. If set to true, the application can play some medias (video, sound) without requiring a user gesture.
### `enablePageLoadingIndication`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, CE, WM</span><br/><span style="font-size: smaller">Read Only</span>

Show page loading indication. On Windows Mobile/CE this property can be set only in config.xml: GUI\\HourglassEnabled. At Android  use 'disable_loading_indication' parameter in rhoconfig.txt to configure this value.
### `enableWebPlugins`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android</span><br/><span style="font-size: smaller">Read Only</span>

Enable / disable web plug-ins. Use 'enable_web_plugins' parameter in rhoconfig.txt to configure this value. This option only has effect on Android versions before 4.0 (ICS). It mainly affects if Flash content is displayed.
### `enableZoom`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android</span><br/><span style="font-size: smaller">Read Only</span>

Enable WebView zoom. Use 'enable_screen_zoom' parameter in rhoconfig.txt to configure this value.
### `fontFamily`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: WM</span><br/><span style="font-size: smaller">Read Only</span>

Specifies the default font to use when rendering text in web pages. The specified font should be a TrueType font present on the device. On Windows the default font has been set to 'Tahoma' as this is present on all Symbol WM / CE devices, note that Tahoma has no italic or oblique variants. On the Enterprise Tablet the default is Droid Sans Fallback. The font specified must be stored in \Windows for Windows WM / CE devices, or /system/fonts for Enterprise Tablet. Defines in config.xml: HTMLStyles\\FontFamily 
### `framework`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span><br/><span style="font-size: smaller">Read Only</span>

Same as System.webViewFramework.
### `fullScreen`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, CE, Win32, WM</span><br/><span style="font-size: smaller">Parameters:

Use full screen mode.
### `keyboardDisplayRequiresUserAction`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: iOS</span><br/><span style="font-size: smaller">Parameters:

Attention: not worked with WKWebView!  Can be defined in rhoconfig.txt as "WebView.keyboardDisplayRequiresUserAction" to 1 or 0. When this property is set to true, the user must explicitly tap the elements in the web view to display the keyboard (or other relevant input view) for that element. When set to false, a focus event on an element causes the input view to be displayed and associated with that element automatically.
### `navigationTimeout`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: WM</span><br/><span style="font-size: smaller">Parameters:

Can be defined in config.xml: Navigation\\NavTimeout. Number of milliseconds(maximum is 45000) before the browser times out and navigates to the page specified in the badlink setting. If it is determined that the destination is unreachable regardless of wait time, the badlink may be loaded before NAVTIMEOUT. This is the time taken to establish communication with the server, not the time taken to fully load the page.Note that the navigation timeout will not be invoked when navigating to the start page, best practice is to store your first page locally to avoid connectivity issues at start up, you can then redirect to an online page if desired.
### `scrollTechnique`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: WM</span><br/><span style="font-size: smaller">Read Only</span>

Specifies the technique used to scroll about the page.Defines in config.xml: Scrolling\\ScrollTechnique.
### `textZoomLevel`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, WM</span><br/><span style="font-size: smaller">Parameters:

Sets the font size to be displayed on the page, set to 0 for the smallest font and 4 for the largest font.
### `userAgent`: string
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: WM</span><br/><span style="font-size: smaller">Read Only</span>

Defines in config.xml: Navigation\\UserAgent. When visiting a web server the WebKit browser will report its self as the specified user agent. Use the following substitution variables:* %p - platform name ("Windows CE " + version number)* %w - WebKit version number* %e - WebKit version number.Use the UserAgent setting to spoof your device to the server, e.g. to view content designed for the desktop on your mobile screen.From RhoElements 2.1 onwards the default value was changed to work out of the box with a greater number of server configurations, prior to RhoElements 2.1 the default user agent was: "Mozilla/5.0 (%p) AppleWebKit/%w (KHTML, like Gecko) WebKit/%e Safari/%w"                
### `viewportEnabled`: boolean
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: WM</span><br/><span style="font-size: smaller">Read Only</span>

Whether to enable or disable viewport meta tag processing.Defines in config.xml: Navigation\\ViewportEnabled.
### `viewportWidth`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: WM</span><br/><span style="font-size: smaller">Read Only</span>

Default viewport width to use for pages that do not have a viewport meta tag (uses 1:1 scaling if not specified).Defines in config.xml: Navigation\\ViewportWidth.
### `zoomPage`: float
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, WM</span><br/><span style="font-size: smaller">Parameters:

Sets the zoom factor of the page. Factor 1.0 is no zoom, values less than 1.0 are zoomed out and values greater than 1.0 are zoomed in.It is recommended to not to use the zoom value less than 1.0 because the page doesn't look in readable format.In Android new Zoom value takes effect on current page, Previous page has to be revisited for the new zoom values to take effect 
## Static Methods
### `active_tab`: integer
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Use NativeTabbar.currentTab property: returns the current tab index.


### `currentLocation`: string
<span style="font-size:smaller">Languages: Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Returns the relative url (location) of the current page(without server and port); the last URL loaded to WebView from Ruby controller action.If you open your page in WebView, and after it makes a few jumps by linking (for example, to outside web adresses for example), currentLocation will still return the initial url opened in WebView. Also, if you use JQMobile, current_location has the initial URL, but does not reflect the actual window.location containing the JQMobile additional address by adding #, etc. See currentUrl.

#### Parameters
tabIndex: integer
### `currentURL`: string
<span style="font-size:smaller">Languages: Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS</span>
#### Description
Returns the actual URL in WebView. This works the same as the JavaScript window.location.href.

#### Parameters
tabIndex: integer
### `executeJavascript`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Execute JavaScript on the current page from your controller.For most mobile platforms, WebView.execute_js has been implemented via redirection to URL with 'javascript:' schema. If WebView.execute_js used in an AJAX call handler method in the controller, it may lead to the situation where the success javascript handler will never be executed. This may happen because, at the moment of success handler should be executed, a URL of the page already has been changed. This means no handlers from the previous page are valid.

#### Parameters
javascriptText: string

tabIndex: integer
### `full_screen_mode`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Use WebView.fullScreen property: Switch to / from full screen mode.

#### Parameters
enable: boolean
### `getCookies`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS</span>
#### Description
Returns cookies map for specified URL. Crosswalk is not supported.

#### Parameters
url: string
### `navigate`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Force WebView to navigate to a URL. White page flickering during transition may happen if a controller action method doesn't return any rendered value, but instead performs a WebView.navigate(someUrl) call. It is important to avoid using WebView.navigate in Ruby action methods because WebView.navigate is intended to be used in callback methods asynchronously.

#### Parameters
url: string

tabIndex: integer
### `navigateBack`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Force WebView to navigate to the previous page using Browser back.

#### Parameters
tabIndex: integer
### `refresh`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, WinCE, Windows Desktop, Windows Embedded, Windows Phone, WM</span>
#### Description
Force WebView to refresh the current page.

#### Parameters
tabIndex: integer
### `removeAllCookies`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS</span>
#### Description
Removes all cookies for application's webview. Crosswalk is not supported.


### `removeCookie`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS</span>
#### Description
Removes cookie by its name for specified URL. Crosswalk is not supported.

#### Parameters
url: string

name: string
### `save`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS</span>
#### Description
Save current page to file system.

#### Parameters
format: string

path: string

tabIndex: integer
### `setCookie`
<span style="font-size:smaller">Languages: Ruby</span><br/><span style="font-size:smaller">Platforms: Android, iOS, Win32</span>
#### Description
When WebView loads the specified url (either by selecting link or from calling WebView.navigate), it will add this cookie to the HTTP request.Not implemented for WebKit.

#### Parameters
url: string

cookie: string
### `set_menu_items`
<span style="font-size:smaller">Languages: JS, Ruby</span><br/><span style="font-size:smaller">Platforms: Android, CE, WM</span>
#### Description
Use Application.nativeMenu property: set native menu items.

#### Parameters
menuItems: hash
