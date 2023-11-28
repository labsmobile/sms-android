<p align="center">
  <img src="https://avatars.githubusercontent.com/u/152215067?s=200&v=4" height="80">
</p>

# LabsMobile-Android

![](https://img.shields.io/badge/version-1.0.0-blue.svg)
 
Send SMS messages through the LabsMobile platform and the SDK for Android. Create an account and install the Android SDK in your application and in seconds you will be able to send SMS messages.

## Documentation

Labsmobile API documentation can be found[here][apidocs].

## Features
  - Send SMS messages.
  - Includes all features of the LabsMobile API.
  - Send and validate OTP passwords.

## Requirements

- Android development environment.
- LabsMobile SDK for Android. More information at [SDK Android][sdk].
- A user account with LabsMobile. Click on the link to create an account [here][signUp].


## Installation

**Place the LabsMobile SDK in the libs directory of your application module.**
**Add the following dependencies in the build.gradle file:**
  - compile 'com.squareup.okhttp3:logging-interceptor:3.0.1'
  - compile 'com.squareup.retrofit2:retrofit:2.0.0'
  - compile 'com.squareup.retrofit2:converter-simplexml:2.0.0-beta4'   
**If there are dependency conflicts change the last line of the above snippet to:**
  ```java
    compile('com.squareup.retrofit2:converter-simplexml:2.0.0-beta4') {
        exclude group: 'xpp3', module: 'xpp3'
        exclude group: 'stax', module: 'stax-api'
        exclude group: 'stax', module: 'stax'
    }
  ```
**You will need the following permission declared in the AndroidManifest.xml file in order to use any method of the SDK.**
  ```java
  <uses-permission android:name="android.permission.INTERNET" />
  ```

**If you want to use the functionality of automatic background verifications, you will need these additional persmissions.**
  ```java
    <uses-permission android:name="android.permission.RECEIVE_SMS" />
    <uses-permission android:name="android.permission.READ_SMS" />
  ```
## Samples

### Send of SMS

## Help

If you have questions, you can contact us through the support chat or through the support email support@labsmobile.com.

[apidocs]: https://apidocs.labsmobile.com/
[signUp]: https://www.labsmobile.com/en/signup
[sdk]: https://www.labsmobile.com/data/labs-mobile-android-sdk.zip