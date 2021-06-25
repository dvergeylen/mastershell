---
layout: default
title: "flutter"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="flutter">
  <a href="/en/common/flutter.html">flutter</a> <a href="#flutter"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Google's free, open source, and cross-platform mobile app SDK.
> More information: <https://github.com/flutter/flutter/wiki/The-flutter-tool>.

#### Display help about a specific command:
```shell
flutter help {{command}}
```
#### Check if all external tools are correctly installed:
```shell
flutter doctor
```
#### List or change Flutter channel:
```shell
flutter channel {{stable|beta|dev|master}}
```
#### Run Flutter on all started emulators and connected devices:
```shell
flutter run -d all
```
#### Download all packages specified in `pubspec.yaml`:
```shell
flutter pub get
```
#### Run tests in a terminal from the root of the project:
```shell
flutter test {{test/example_test.dart}}
```
#### Build a release APK targeting most modern smartphones:
```shell
flutter build apk --target-platform {{android-arm}},{{android-arm64}}
```
{% endraw %}