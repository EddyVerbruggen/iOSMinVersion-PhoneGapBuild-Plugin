# iOS Min Version

by [Eddy Verbruggen](http://www.x-services.nl), for PhoneGap >= 3.0.0


> This plugin was meant for PhoneGap Build, but it's largely useless these days - I'll remove it some day.


1. [Description](https://github.com/EddyVerbruggen/iOSMinVersion-PhoneGapBuild-Plugin#1-description)
2. [Installation](https://github.com/EddyVerbruggen/iOSMinVersion-PhoneGapBuild-Plugin#2-installation)

## 1. Description

If you are using PhoneGap Build and want to specify the minimal iOS version for your app, then you've come to the right place.
Add this plugin and set MIN_VERSION to 6.0, 6.1, 7.0, or whatever you like, as long as it's valid.

## 2. Installation

The only thing you need to do is editing your `www/config.xml`.
Add this line:

```xml
<gap:plugin name="nl.x-services.plugins.iosminversion">
  <param name="MIN_VERSION" value="7.0" />
</gap:plugin>
```

This makes sure your app is not available for iOS version lower than 7.0.

Don't set it lower than supported by PhoneGap Build (which is 5.0 currently).
