# iOS Min Version

by [Eddy Verbruggen](http://www.x-services.nl), for PhoneGap >= 3.0.0


> **PhoneGap Build review team, please read this!**
>
> On Build it is not possible to specify a minimal iOS version, but it is possible to set this in the .plist.
> This plugin sets the correct value in the .plist based on the setting in config.xml.
>
> I am not sure whether or not during creation of the .ipa the plugin setting is used (the MinimumOSVersion is supposed to be based on the iPhone OS Deployment Target),
> so please check whether or not the resulting .plist has the correct value for `MinimumOSVersion` and reject this plugin in case it doesn't work.
>
> _This comment will be removed by me after approval._


1. [Description](https://github.com/EddyVerbruggen/iOSMinVersion-PhoneGapBuild-Plugin#1-description)
2. [Installation](https://github.com/EddyVerbruggen/iOSMinVersion-PhoneGapBuild-Plugin#2-installation)
3. [License](https://github.com/EddyVerbruggen/iOSMinVersion-PhoneGapBuild-Plugin#3-license)

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

## 3. License

[The MIT License (MIT)](http://www.opensource.org/licenses/mit-license.html)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
