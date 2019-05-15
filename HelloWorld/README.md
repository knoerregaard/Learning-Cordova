# Cordova

## Commands

- npm cordova install -g
- cordova create HelloWorld
- cordova platform add android
- cordova platform add ios
- cordova platform ls
- cordova requirements
- cordova build / cordova build android
- cordova emulate android /cordova run android --device
- cordova run --emulator


## Android prerequisites (https://cordova.apache.org/docs/en/latest/guide/platforms/android/)
- Download and install Java JDK 8 (https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html) - User account is nessecary
    - Add environment variables
    - JAVA_HOME C:\Program Files\Java\jdk1.8.0_211
- Download and install Android SDK (https://developer.android.com/studio#downloads). Choose commandline tools only
    - Extract content to C:\Android\android-sdk
    - Add environment variables
        - ANDROID_HOME  C:\Android\android-sdk
        - Path          C:\Android\android-sdk\tools, C:\Android\android-sdk\tools\bin
- Download and install Android SDK Platform Tools (https://developer.android.com/studio/releases/platform-tools)
    - Add environment variables
        - Path C:\Android\android-sdk\platform-tools
- Install platform api
    - sdkmanager --list (list all installed and available packages)
    - sdkmanager "platforms;android-28"
    - Accept license
- Install Gradle (https://gradle.org/install/)
    - Add environment variables
        - Path C:\Gradle\gradle-5.4.1\bin

## Cordova new projekt
### Create new HelloWorld Projekt
To create a new projekt with Cordova use the command ```cordova create HelloWorld```.

### Debug/run application on device
You can run the application directly on your device. Connect your phone with usb cable. When ready enter ```cordova run android --device ```
Remember to activate the developer mode in your phone. Also ensure to enable USB debugging. If you dont do that the build will return with "Failed to deploy to device, no devices found."

## IOS Prerequisites (https://cordova.apache.org/docs/en/latest/guide/platforms/ios/)
Mac and XCode
When the project is compiled move your project to XCode on a Mac.
