---
layout: default
title: "android"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#am">am</a>
* <a href="#bugreport">bugreport</a>
* <a href="#bugreportz">bugreportz</a>
* <a href="#cmd">cmd</a>
* <a href="#dalvikvm">dalvikvm</a>
* <a href="#dumpsys">dumpsys</a>
* <a href="#getprop">getprop</a>
* <a href="#input">input</a>
* <a href="#logcat">logcat</a>
* <a href="#pm">pm</a>
* <a href="#settings">settings</a>
* <a href="#wm">wm</a>

{% raw %}
<h2 id="am">
  <a href="/en/android/am.html">am</a> <a href="#am"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android activity manager.
> More information: <https://developer.android.com/studio/command-line/adb#am>.

#### Start a specific activity:
```shell
am start -n {{com.android.settings/.Settings}}
```
#### Start an activity and pass data to it:
```shell
am start -a {{android.intent.action.VIEW}} -d {{tel:123}}
```
#### Start an activity matching a specific action and category:
```shell
am start -a {{android.intent.action.MAIN}} -c {{android.intent.category.HOME}}
```
#### Convert an intent to an URI:
```shell
am to-uri -a {{android.intent.action.VIEW}} -d {{tel:123}}
```
{% endraw %}{% raw %}
<h2 id="bugreport">
  <a href="/en/android/bugreport.html">bugreport</a> <a href="#bugreport"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show an Android bug report.
> This command can only be used through `adb shell`.
> More information: <https://android.googlesource.com/platform/frameworks/native/+/master/cmds/bugreport/>.

#### Show a complete bug report of an Android device:
```shell
bugreport
```
{% endraw %}{% raw %}
<h2 id="bugreportz">
  <a href="/en/android/bugreportz.html">bugreportz</a> <a href="#bugreportz"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate a zipped Android bug report.
> This command can only be used through `adb shell`.
> More information: <https://android.googlesource.com/platform/frameworks/native/+/master/cmds/bugreportz/>.

#### Generate a complete zipped bug report of an Android device:
```shell
bugreportz
```
#### Show the progress of a running `bugreportz` operation:
```shell
bugreportz -p
```
#### Show the version of `bugreportz`:
```shell
bugreportz -v
```
#### Display help:
```shell
bugreportz -h
```
{% endraw %}{% raw %}
<h2 id="cmd">
  <a href="/en/android/cmd.html">cmd</a> <a href="#cmd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android service manager.
> More information: <https://cs.android.com/android/platform/superproject/+/master:frameworks/native/cmds/cmd/>.

#### List every running service:
```shell
cmd -l
```
#### Call a specific service:
```shell
cmd {{alarm}}
```
#### Call a service with arguments:
```shell
cmd {{vibrator}} {{vibrate 300}}
```
{% endraw %}{% raw %}
<h2 id="dalvikvm">
  <a href="/en/android/dalvikvm.html">dalvikvm</a> <a href="#dalvikvm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Java virtual machine.
> More information: <https://source.android.com/devices/tech/dalvik>.

#### Start a Java program:
```shell
dalvikvm -classpath {{path/to/file.jar}} {{classname}}
```
{% endraw %}{% raw %}
<h2 id="dumpsys">
  <a href="/en/android/dumpsys.html">dumpsys</a> <a href="#dumpsys"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Provide information about Android system services.
> This command can only be used through `adb shell`.
> More information: <https://developer.android.com/studio/command-line/dumpsys>.

#### Get diagnostic output for all system services:
```shell
dumpsys
```
#### Get diagnostic output for a specific system service:
```shell
dumpsys {{service}}
```
#### List all services `dumpsys` can give information about:
```shell
dumpsys -l
```
#### List service-specific arguments for a service:
```shell
dumpsys {{service}} -h
```
#### Exclude a specific service from the diagnostic output:
```shell
dumpsys --skip {{service}}
```
#### Specify a timeout period in seconds (defaults to 10s):
```shell
dumpsys -t {{seconds}}
```
{% endraw %}{% raw %}
<h2 id="getprop">
  <a href="/en/android/getprop.html">getprop</a> <a href="#getprop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show information about Android system properties.
> More information: <https://manned.org/getprop>.

#### Display information about Android system properties:
```shell
getprop
```
#### Display information about a specific property:
```shell
getprop {{prop}}
```
#### Display the SDK API level:
```shell
getprop {{ro.build.version.sdk}}
```
#### Display the Android version:
```shell
getprop {{ro.build.version.release}}
```
#### Display the Android device model:
```shell
getprop {{ro.vendor.product.model}}
```
#### Display the OEM unlock status:
```shell
getprop {{ro.oem_unlock_supported}}
```
#### Display the MAC address of the Android's WiFi card:
```shell
getprop {{ro.boot.wifimacaddr}}
```
{% endraw %}{% raw %}
<h2 id="input">
  <a href="/en/android/input.html">input</a> <a href="#input"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Send event codes or touchscreen gestures to an Android device.
> This command can only be used through `adb shell`.
> More information: <https://developer.android.com/reference/android/view/KeyEvent.html#constants_1>.

#### Send an event code for a single character to an Android device:
```shell
input keyevent {{event_code}}
```
#### Send a text to an Android device (`%s` represents spaces):
```shell
input text "{{text}}"
```
#### Send a single tap to an Android device:
```shell
input tap {{x_pos}} {{y_pos}}
```
#### Send a swipe gesture to an Android device:
```shell
input swipe {{x_start}} {{y_start}} {{x_end}} {{y_end}} {{duration_in_ms}}
```
#### Send a long press to an Android device using a swipe gesture:
```shell
input swipe {{x_pos}} {{y_pos}} {{x_pos}} {{y_pos}} {{duration_in_ms}}
```
{% endraw %}{% raw %}
<h2 id="logcat">
  <a href="/en/android/logcat.html">logcat</a> <a href="#logcat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Dump a log of system messages.
> More information: <https://developer.android.com/studio/command-line/logcat>.

#### Display system logs:
```shell
logcat
```
#### Write system logs to a file:
```shell
logcat -f {{path/to/file}}
```
#### Display lines that match a regular expression:
```shell
logcat --regex {{regular_expression}}
```
{% endraw %}{% raw %}
<h2 id="pm">
  <a href="/en/android/pm.html">pm</a> <a href="#pm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show information about apps on an Android device.
> More information: <https://developer.android.com/studio/command-line/adb#pm>.

#### Print a list of all installed apps:
```shell
pm list packages
```
#### Print a list of all installed system apps:
```shell
pm list packages -s
```
#### Print a list of all installed 3rd-Party apps:
```shell
pm list packages -3
```
#### Print a list of apps matching specific keywords:
```shell
pm list packages {{keywords}}
```
#### Print the path of the APK of a specific app:
```shell
pm path {{app}}
```
{% endraw %}{% raw %}
<h2 id="settings">
  <a href="/en/android/settings.html">settings</a> <a href="#settings"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get information about the Android OS.
> More information: <https://adbinstaller.com/commands/adb-shell-settings-5b670d5ee7958178a2955536>.

#### Display a list of settings in the `global` namespace:
```shell
settings list {{global}}
```
#### Get the value of a specific setting:
```shell
settings get {{global}} {{airplane_mode_on}}
```
#### Set the value of a setting:
```shell
settings put {{system}} {{screen_brightness}} {{42}}
```
#### Delete a specific setting:
```shell
settings delete {{secure}} {{screensaver_enabled}}
```
{% endraw %}{% raw %}
<h2 id="wm">
  <a href="/en/android/wm.html">wm</a> <a href="#wm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show information about the screen of an Android device.
> This command can only be used through `adb shell`.
> More information: <https://adbinstaller.com/commands/adb-shell-wm-5b672b17e7958178a2955538>.

#### Display the physical size of an Android device's screen:
```shell
wm {{size}}
```
#### Display the physical density of an Android device's screen:
```shell
wm {{density}}
```
{% endraw %}