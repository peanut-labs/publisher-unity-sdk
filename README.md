# publisher-unity-sdk

Our Plugin allows you to launch the Peanut Labs Reward Center as an overlay on top of you application from anywhere in the application. We recommend using our Plugin because it comes with the basic navigation controls a user would need to go between, surveys, offers and our Reward Center.
A Peanut Labs Unity iOS & Android Plugin is provided via Github containing publisher_unity_sdk.unitypackage file. This package is needs to be imported into your project. We support all iOS & Android devices except iPhones below iPhone 4 and android 4.1+ (Jelly Bean and above)


Note: Our Plugin will not show you result as you expected unless you build and run in iOS or an Android environment, simulator or device. There is also example call of opening our rewards center packaged in our unity package. Simply open ExamplePublisher.cs file and can see examples.

### Usage

*	Generate the Peanut Labs User ID on your server side and pass that on to the client side app.
*	Import publisher_unity_sdk.unitypackage into your project.

```

From Unity go to Assets menu → Import package → Custom package → choose our unity package.

```

*	Once you imported our package make sure our plugin files are in your project structure.

```

Project_path/Plugins/PeanutLabsManager.cs
Project_path/Plugins/iOS/PeanutLabsManagerWrapper
Project_path/Plugins/SDK/*

IF Android

Project_path/Plugins/PeanutLabsManager.cs
Project_path/Plugins/Android/AndroidManifest
Project_path/Plugins/Android/plsdk
Project_path/Plugins/res/*


```

*	Open Rewards Center.

``` C#
Open Rewards Center with User Id
PeanutLabsManager.openRewardsCenterWithUserId(“USER_ID_HERE”);

```




