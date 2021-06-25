---
layout: default
title: "adb install"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb-install">
  <a href="/pl/common/adb-install.html">adb install</a> <a href="#adb-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Install: wysyłaj pakiety do instancji emulatora Androida lub podłączonych urządzeń z systemem Android.
> Więcej informacji: <https://developer.android.com/studio/command-line/adb>.

#### Wyślij aplikację na Androida do emulatora / urządzenia:
```shell
adb install {{scieżka/do/pliku.apk}}
```
#### Zainstaluj ponownie istniejącą aplikację, zachowując jej dane:
```shell
adb install -r {{scieżka/do/pliku.apk}}
```
#### Przyznaj wszystkie uprawnienia wymienione w pliku manifestu aplikacji:
```shell
adb install -g {{scieżka/do/pliku.apk}}
```
#### Szybko zaktualizuj zainstalowany pakiet, aktualizując tylko te części APK, które się zmieniły:
```shell
adb install --fastdeploy {{scieżka/do/pliku.apk}}
```
{% endraw %}