## FreshGrade Cordova iOS config injections
*This plugin is used to inject key/value pairs into Info.plist at build time*


### App Transport Security Plugin for Apache Cordova [![npm version](https://badge.fury.io/js/cordova-plugin-transport-security.svg)](http://badge.fury.io/js/cordova-plugin-transport-security)

**Cordova / PhoneGap Plugin to allow 'Arbitrary Loads' by adding a declaration to the Info.plist file to bypass the iOS 9 App Transport Security**

#### Apple guidance

> App Transport Security (ATS) enforces best practices in the secure connections between an app and its back end. ATS prevents accidental disclosure, provides secure default behavior, and is easy to adopt; it is also on by default in iOS 9 and OS X v10.11. You should adopt ATS as soon as possible, regardless of whether you’re creating a new app or updating an existing one.

> If you’re developing a new app, you should use HTTPS exclusively. If you have an existing app, you should use HTTPS as much as you can right now, and create a plan for migrating the rest of your app as soon as possible. In addition, your communication through higher-level APIs needs to be encrypted using TLS version 1.2 with forward secrecy. If you try to make a connection that doesn't follow this requirement, an error is thrown. If your app needs to make a request to an insecure domain, you have to specify this domain in your app's Info.plist file.

Source: [iOS Developer Library](https://developer.apple.com/library/prerelease/ios/releasenotes/General/WhatsNewIniOS/Articles/iOS9.html#//apple_ref/doc/uid/TP40016198-SW14)

It's important to note that this does not impact apps built with Xcode < 7 running on iOS 9.

#### Platforms
Applies to iOS (9+) only.