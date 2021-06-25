---
layout: default
title: "electron-packager"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="electron-packager">
  <a href="/en/common/electron-packager.html">electron-packager</a> <a href="#electron-packager"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool used to build Electron app executables for Windows, Linux and macOS.
> Requires a valid package.json in the application directory.
> More information: <https://github.com/electron/electron-packager>.

#### Package an application for the current architecture and platform:
```shell
electron-packager "{{path/to/app}}" "{{app_name}}"
```
#### Package an application for all architectures and platforms:
```shell
electron-packager "{{path/to/app}}" "{{app_name}}" --all
```
#### Package an application for 64-bit Linux:
```shell
electron-packager "{{path/to/app}}" "{{app_name}}" --platform="{{linux}}" --arch="{{x64}}"
```
#### Package an application for ARM macOS:
```shell
electron-packager "{{path/to/app}}" "{{app_name}}" --platform="{{darwin}}" --arch="{{arm64}}"
```
{% endraw %}