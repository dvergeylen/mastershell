---
layout: default
title: "react-native"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="react-native">
  <a href="/en/common/react-native.html">react-native</a> <a href="#react-native"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A framework for building native apps with React.
> More information: <https://reactnative.dev>.

#### Initialize a new React Native project in a directory of the same name:
```shell
react-native init {{project_name}}
```
#### Start the metro bundler:
```shell
react-native start
```
#### Start the metro bundler with a clean cache:
```shell
react-native start --reset-cache
```
#### Build the current application and start it on a connected Android device or emulator:
```shell
react-native run-android
```
#### Build the current application and start it on an iOS simulator:
```shell
react-native run-ios
```
#### Build the current application in `release` mode and start it on a connected Android device or emulator:
```shell
react-native run-android --variant={{release}}
```
#### Start `logkitty` and print logs to stdout:
```shell
react-native log-android
```
#### Start `tail system.log` for an iOS simulator and print logs to stdout:
```shell
react-native log-ios
```
{% endraw %}