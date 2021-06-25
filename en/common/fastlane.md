---
layout: default
title: "fastlane"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fastlane">
  <a href="/en/common/fastlane.html">fastlane</a> <a href="#fastlane"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Build and release mobile applications from the command-line.
> More information: <https://docs.fastlane.tools/actions/>.

#### Build and sign the iOS application in the current directory:
```shell
fastlane run build_app
```
#### Run `pod install` for the project in the current directory:
```shell
fastlane run cocoapods
```
#### Delete the derived data from Xcode:
```shell
fastlane run clear_derived_data
```
#### Remove the cache for pods:
```shell
fastlane run clean_cocoapods_cache
```
{% endraw %}