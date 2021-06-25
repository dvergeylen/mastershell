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
  <a href="/de/android/am.html">am</a> <a href="#am"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Androids Aktivitäten-Manager.
> Weitere Informationen: <https://developer.android.com/studio/command-line/adb#am>.

#### Starte eine bestimmte Aktivität:
```shell
am start -n {{com.android.settings/.Settings}}
```
#### Starte eine Aktivität und übergib ihr Daten:
```shell
am start -a {{android.intent.action.VIEW}} -d {{tel:123}}
```
#### Starte eine Aktivität, auf die eine bestimmte Aktion und Kategorie zutrifft:
```shell
am start -a {{android.intent.action.MAIN}} -c {{android.intent.category.HOME}}
```
#### Konvertiere ein bestimmtes Ziel in einen URI:
```shell
am to-uri -a {{android.intent.action.VIEW}} -d {{tel:123}}
```
{% endraw %}{% raw %}
<h2 id="bugreport">
  <a href="/de/android/bugreport.html">bugreport</a> <a href="#bugreport"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeige Android-Fehlerberichte.
> Dieser Befehl kann nur mit `adb shell` verwendet werden.
> Weitere Informationen: <https://android.googlesource.com/platform/frameworks/native/+/master/cmds/bugreport/>.

#### Zeige einen vollständigen Fehlerbericht eines Android Geräts an:
```shell
bugreport
```
{% endraw %}{% raw %}
<h2 id="bugreportz">
  <a href="/de/android/bugreportz.html">bugreportz</a> <a href="#bugreportz"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generiere einen gezippten Android-Fehlerbericht.
> Dieser Befehl kann nur mit `adb shell` verwendet werden.
> Weitere Informationen: <https://android.googlesource.com/platform/frameworks/native/+/master/cmds/bugreportz/>.

#### Generiere einen vollständigen Fehlerbericht eines Android Geräts:
```shell
bugreportz
```
#### Zeige den Fortschritt eines laufenden `bugreportz` Prozesses an:
```shell
bugreportz -p
```
#### Zeige die Versionsnummer von `bugreportz` an:
```shell
bugreportz -v
```
#### Zeige Hilfe an:
```shell
bugreportz -h
```
{% endraw %}{% raw %}
<h2 id="cmd">
  <a href="/de/android/cmd.html">cmd</a> <a href="#cmd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Androids Service-Manager.
> Weitere Informationen: <https://cs.android.com/android/platform/superproject/+/master:frameworks/native/cmds/cmd/>.

#### Liste alle laufenden Services auf:
```shell
cmd -l
```
#### Rufe einen bestimmten Service auf:
```shell
cmd {{alarm}}
```
#### Rufe einen bestimmten Service mit Parametern auf:
```shell
cmd {{vibrator}} {{vibrate 300}}
```
{% endraw %}{% raw %}
<h2 id="dalvikvm">
  <a href="/de/android/dalvikvm.html">dalvikvm</a> <a href="#dalvikvm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Androids Java Virtual Machine.
> Weitere Informationen: <https://source.android.com/devices/tech/dalvik>.

#### Starte ein Java-Programm:
```shell
dalvikvm -classpath {{pfad/zu/datei.jar}} {{klassenname}}
```
{% endraw %}{% raw %}
<h2 id="dumpsys">
  <a href="/de/android/dumpsys.html">dumpsys</a> <a href="#dumpsys"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Stelle Informationen über Android-Systemservices bereit.
> Dieser Befehl kann nur mit `adb shell` verwendet werden.
> Weitere Informationen: <https://developer.android.com/studio/command-line/dumpsys>.

#### Erhalte diagnostische Informationen über alle Systemservices:
```shell
dumpsys
```
#### Erhalte diagnostische Informationen über einen bestimmten Systemservice:
```shell
dumpsys {{service}}
```
#### Liste alle Services, über die `dumpsys` Informationen bereitstellen kann auf:
```shell
dumpsys -l
```
#### Liste Service-spezifische Argumente für einen Service auf:
```shell
dumpsys {{service}} -h
```
#### Schließe einen bestimmten Service von den diagnostischen Informationen aus:
```shell
dumpsys --skip {{service}}
```
#### Gib ein Timeout in Sekunden an (standardmäßig 10s):
```shell
dumpsys -t {{sekunden}}
```
{% endraw %}{% raw %}
<h2 id="getprop">
  <a href="/de/android/getprop.html">getprop</a> <a href="#getprop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeige Informationen über Android-Systemeigenschaften.
> Weitere Informationen: <https://manned.org/getprop>.

#### Gib Informationen über Android-Systemeigenschaften aus:
```shell
getprop
```
#### Gib Informationen über eine bestimmte Systemeigenschaft aus:
```shell
getprop {{eigenschaft}}
```
#### Gib das SDK-API-Level aus:
```shell
getprop {{ro.build.version.sdk}}
```
#### Gib die Android-Version aus:
```shell
getprop {{ro.build.version.release}}
```
#### Gib das Modell des Geräts aus:
```shell
getprop {{ro.vendor.product.model}}
```
#### Gib den OEM-Entsperrstatus aus:
```shell
getprop {{ro.oem_unlock_supported}}
```
#### Gib die MAC-Adresse der WiFi-Karte aus:
```shell
getprop {{ro.boot.wifimacaddr}}
```
{% endraw %}{% raw %}
<h2 id="input">
  <a href="/de/android/input.html">input</a> <a href="#input"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sende Eventcodes oder Touchscreengesten an ein Android-Gerät.
> Dieser Befehl kann nur mit `adb shell` verwendet werden.
> Weitere Informationen: <https://developer.android.com/reference/android/view/KeyEvent.html#constants_1>.

#### Sende einen Eventcode für die Eingabe eines einzelnen Zeichens an ein Gerät:
```shell
input keyevent {{eventcode}}
```
#### Sende einen Text an ein Gerät (`%s` wird als Leerzeichen verwendet):
```shell
input text "{{text}}"
```
#### Sende ein einzelnes Tippen auf den Touchscreen an ein Gerät:
```shell
input tap {{x_pos}} {{y_pos}}
```
#### Sende ein Wischen über den Touchscreen an ein Gerät:
```shell
input swipe {{x_start}} {{y_start}} {{x_ende}} {{y_ende}} {{dauer_in_ms}}
```
#### Sende ein langes Tippen auf den Touschscreen an ein Gerät:
```shell
input swipe {{x_pos}} {{y_pos}} {{x_pos}} {{y_pos}} {{dauer_in_ms}}
```
{% endraw %}{% raw %}
<h2 id="logcat">
  <a href="/de/android/logcat.html">logcat</a> <a href="#logcat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gib ein Protokoll aller Systemmeldungen aus:
> Weitere Informationen: <https://developer.android.com/studio/command-line/logcat>.

#### Gib ein Protokoll aller Systemmeldungen aus:
```shell
logcat
```
#### Schreibe alle Systemmeldungen in eine Datei:
```shell
logcat -f {{pfad/zu/datei}}
```
#### Gib Zeilen aus, die einem regulären Ausdruck entsprechen:
```shell
logcat --regex {{regex}}
```
{% endraw %}{% raw %}
<h2 id="pm">
  <a href="/de/android/pm.html">pm</a> <a href="#pm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeige Informationen über Apps auf einem Android Gerät.
> Weitere Informationen: <https://developer.android.com/studio/command-line/adb#pm>.

#### Gib eine Liste aller installierten Apps aus:
```shell
pm list packages
```
#### Gib eine Liste aller installierten System-Apps aus:
```shell
pm list packages -s
```
#### Gib eine Liste aller installierten Apps von Drittanbietern aus:
```shell
pm list packages -3
```
#### Gib eine Liste aller Apps, auf die ein bestimmtes Schlüsselwort zutrifft, aus:
```shell
pm list packages {{Schlüsselwort}}
```
#### Gib den Pfad der APK einer bestimmten App aus:
```shell
pm path {{app}}
```
{% endraw %}{% raw %}
<h2 id="settings">
  <a href="/de/android/settings.html">settings</a> <a href="#settings"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte Android-Systemeinstellungen.
> Weitere Informationen: <https://adbinstaller.com/commands/adb-shell-settings-5b670d5ee7958178a2955536>.

#### Gib eine Liste aller Einstellungen im Namespace `global` aus:
```shell
settings list {{global}}
```
#### Gib den Wert einer bestimmten Einstellung aus:
```shell
settings get {{global}} {{airplane_mode_on}}
```
#### Setze den Wert einer bestimmten Einstellung:
```shell
settings put {{system}} {{screen_brightness}} {{42}}
```
#### Lösche eine bestimmte Einstellung:
```shell
settings delete {{secure}} {{screensaver_enabled}}
```
{% endraw %}{% raw %}
<h2 id="wm">
  <a href="/de/android/wm.html">wm</a> <a href="#wm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeige Informationen über den Bildschirm eines Android-Geräts.
> Dieser Befehl kann nur mit `adb shell` verwendet werden.

#### Gib die physische Größe des Bildschirms eines Geräts aus:
```shell
wm {{size}}
```
#### Gib die physische Pixeldichte des Bildschirms eines Geräts aus:
```shell
wm {{density}}
```
{% endraw %}