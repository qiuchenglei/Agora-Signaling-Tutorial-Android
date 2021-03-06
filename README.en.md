# Agora Android Signaling Tutorial

*其他语言版本： [简体中文](README.md)*

The Agora Android Signaling Tutorial is an open-source demo that will help you get message chat integrated directly into your Android applications using the Agora Signaling SDK.

With this sample app, you can:

- Login Signaling server
- Inquire whether the calling object is online
- Send point to point message and receive point to point message off line
- Join channel
- Send channel message, receive channel message
- Leave channel
- Logout Signaling server

Agora Signaling SDK supports iOS / Android / Web. You can find demos of these platform here:

- iOS : https://github.com/AgoraIO/Agora-Signaling-Tutorial-iOS-Swift
- Web : https://github.com/AgoraIO/Agora-Signaling-Tutorial-Web
- MacOS : https://github.com/AgoraIO/Agora-Signaling-Tutorial-macOS-Swift
- Linux : https://github.com/AgoraIO/Agora-Signaling-Tutorial-Linux
- Java : https://github.com/AgoraIO/Agora-Signaling-Tutorial-Java
- Windows: https://github.com/AgoraIO/Agora-Signaling-Tutorial-Windows


## Running the App
First, create a developer account at [Agora.io](https://dashboard.agora.io/signin/), and obtain an App ID.
Update "app/src/main/res/values/strings_config.xml" with your App ID .

```
<string name="agora_app_id"><#YOUR APP ID#></string>

```
## Integration mode
- The first step is to download the signaling SDK in Agora.io SDK. After decompressing, copy the *.jar under the LIBS folder to the app/libs of this project. The arm64-v8a/x86/armeabi-v7a under the LIBS folder is copied to the app/src/main/jniLibs of this project.

- The second step: add the following dependency in the "app/build.gradle" file dependency property of this project (the example is added in this code):

  compile fileTree(dir: 'libs', include: ['*.jar'])


Finally, open project with Android Studio, connect your Android device, build and run.

Or use `Gradle` to build and run.

## Developer Environment Requirements
- Android Studio 2.0 or above
- Real devices (Nexus 5X or other devices)
- Some simulators are function missing or have performance issue, so real device is the best choice

## Connect Us
- You can find full API document at [Document Center](https://docs.agora.io/en/)
- You can file bugs about this demo at [issue](https://github.com/AgoraIO/Agora-Android-Tutorial-1to1/issues)

## License
The MIT License (MIT).
