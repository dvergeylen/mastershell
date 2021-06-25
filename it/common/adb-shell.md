---
layout: default
title: "adb shell"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb-shell">
  <a href="/it/common/adb-shell.html">adb shell</a> <a href="#adb-shell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Shell: Esegue un commando remoto sull'emulatore o dispositivo Android connesso.
> Maggiori informazioni: <https://developer.android.com/studio/command-line/adb>.

#### Avvia un interprete di comandi iterativo remoto sull'emulatore/dispositivo:
```shell
adb shell
```
#### Fornisce tutte le proprietà dell'emulatore o dispositivo:
```shell
adb shell getprop
```
#### Ripristina tutti i permessi di esecuzione ai loro valori predefiniti:
```shell
adb shell pm reset-permissions
```
#### Revoca un permesso pericoloso da un'applicazione:
```shell
adb shell pm revoke {{pacchetto}} {{permesso}}
```
#### Attiva un evento chiave:
```shell
adb shell input keyevent {{keycode}}
```
#### Pulisce i dati di un'applicazione sull'emulatore o dispositivo:
```shell
adb shell pm clear {{pacchetto}}
```
#### Avvia un'attività sull'emulatore/dispositivo:
```shell
adb shell am start -n {{pacchetto}}/{{attività}}
```
#### Avvia la schermata iniziale sull'emulatore o dispositivo:
```shell
adb shell am start -W -c android.intent.category.HOME -a android.intent.action.MAIN
```
{% endraw %}