Cordova Badge-Plugin
====================

[Cordova][cordova] plugin to access and modify the badge number of the app icon.


## Supported Platforms
- **iOS**

## Installation
The plugin can either be installed into the local development environment or cloud based through [PhoneGap Build][PGB].

```bash
# ~~ from master ~~
cordova plugin add https://github.com/nickbarth/cordova-plugin-badge.git
```

### Set the badge of the app icon

```javascript
window.badge.set(Number);
```

### Get the badge of the app icon
The badge of the app can be accessed through the `notification.badge.get` interface.<br>
The method takes a callback function as its argument which will be called with the badge number. Optional the scope of the callback function ca be defined through a second argument.

```javascript
window.badge.get(function (badge) {
	// console.log('Badge of the app icon: ' + badge);
}, scope);
```

## License

This software is released under the [Apache 2.0 License][apache2_license].

&copyr; 2013-2014 appPlant UG, Inc. All rights reserved

[cordova]: https://cordova.apache.org
[android_notification_guide]: http://developer.android.com/guide/topics/ui/notifiers/notifications.html
[wp8_notification_guide]: http://msdn.microsoft.com/en-us/library/windowsphone/develop/hh202948.aspx
[CLI]: http://cordova.apache.org/docs/en/3.0.0/guide_cli_index.md.html#The%20Command-line%20Interface
[PGB]: http://docs.build.phonegap.com/en_US/3.3.0/index.html
[PGB_plugin]: https://build.phonegap.com/plugins/724
[set]: #set-the-badge-of-the-app-icon
[get]: #get-the-badge-of-the-app-icon
[clear]: #clear-the-badge-of-the-app-icon
[set_clear_on_tap]: #clear-the-badge-automatically-if-the-user-taps-the-app-icon
[examples]: #examples
[set_title]: specify-custom-notification-title-on-android
[apache2_license]: http://opensource.org/licenses/Apache-2.0
