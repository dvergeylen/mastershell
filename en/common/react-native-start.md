---
layout: default
title: "react-native start"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="react-native-start">
  <a href="/en/common/react-native-start.html">react-native start</a> <a href="#react-native-start"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line tools to start the React Native server.
> More information: <https://github.com/react-native-community/cli/blob/master/docs/commands.md#start>.

#### Start the server that communicates with connected devices:
```shell
react-native start
```
#### Start the metro bundler with a clean cache:
```shell
react-native start --reset-cache
```
#### Start the server in a custom port (defaults to 8081):
```shell
react-native start --port {{3000}}
```
#### Start the server in verbose mode:
```shell
react-native start --verbose
```
#### Specify the maximum number of workers for transforming files (default is the number of CPU cores):
```shell
react-native start --max-workers {{count}}
```
#### Disable interactive mode:
```shell
react-native start --no-interactive
```
{% endraw %}