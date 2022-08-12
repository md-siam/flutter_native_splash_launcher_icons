<img src="screenshots/badges/built-with-love.svg" height="28px"/>&nbsp;&nbsp;
<img src="screenshots/badges/flutter-dart.svg" height="28px" />&nbsp;&nbsp;
<a href="https://choosealicense.com/licenses/mit/" target="_blank"><img src="screenshots/badges/license-MIT.svg" height="28px" /></a>&nbsp;&nbsp;
<img src="screenshots/badges/Flutter-3.svg" height="28px" />&nbsp;&nbsp;
<img src="screenshots/badges/dart-null_safety-blue.svg" height="28px"/>

# Native Splash & App Icon Generator

<img align="right" src="screenshots/store_icons/icon1.png" height="190"></img>

This repo is for teaching us how to implement the "native splash screen" in flutter & also how to generate "app icon" automatically for iOS, Android, & Web platforms. You can follow this [YouTube](https://www.youtube.com/watch?v=eMHbgIgJyUQ) video to learn about [flutter_launcher_icons](https://pub.dev/packages/flutter_launcher_icons) package.

## App-Icon Generator Process

In `pubspec.yaml`, copy and pest the following into the **dev_dependencies** section.

```yaml
dev_dependencies:
  flutter_test:
    sdk: flutter
  flutter_lints: ^2.0.1
  flutter_launcher_icons: ^0.10.0

flutter_icons:
  android: true
  ios: true
  image_path: "assets/app_icon/icon1.png"
  adaptive_icon_background: "#EEEEEE"
  min_sdk_android: 21 # android min sdk min:16, default 21
  web:
    generate: true
    image_path: "assets/app_icon/icon1.png"
    background_color: "#EEEEEE"
    theme_color: "#EEEEEE"
```

Now, in terminal:

```shell
$ flutter pub get
$ flutter pub run flutter_launcher_icons:main
```

<h3><p align="center">DONE WITH APP ICON</p></h3>

## App Demo

<table align="center" style="margin: 0px auto;">
  <tr>
    <th align="center">iOS Simulator</th>
    <th align="center">Android Emulator</th>
  </tr>
  <tr>
    <td align="center"><img align="right" src="screenshots/gif/ios_simulator.gif" height="500"></img></td>
    <td align="center"><img align="right" src="screenshots/gif/android_emulator.gif" height="500"></img></td>
  </tr>
</table>
