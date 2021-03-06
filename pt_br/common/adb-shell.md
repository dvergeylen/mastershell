---
layout: default
title: "adb shell"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb-shell">
  <a href="/pt_br/common/adb-shell.html">adb shell</a> <a href="#adb-shell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Shell: Executar remotamente comandos shell em instâncias do emulador Android ou dispositivos Android conectados.
> Mais informações: <https://developer.android.com/studio/command-line/adb?hl=pt-br>.

#### Iniciar um shell interativo remoto no emulador/dispositivo:
```shell
adb shell
```
#### Obter todas as propriedades do emulador ou dispositivo:
```shell
adb shell getprop
```
#### Reverter todas as permissões de tempo de execução para o padrão:
```shell
adb shell pm reset-permissions
```
#### Revogar uma permissão perigosa para um aplicação:
```shell
adb shell pm revoke {{pacote}} {{permissao}}
```
#### Acionar um evento:
```shell
adb shell input keyevent {{keycode}}
```
#### Limpar os dados da aplicação no emulador/dispositivo:
```shell
adb shell pm clear {{pacote}}
```
#### Iniciar uma atividade no emulator/dispositivo:
```shell
adb shell am start -n {{pacote}}/{{atividade}}
```
#### Iniciar atividade "home" no emulator/dispositivo:
```shell
adb shell am start -W -c android.intent.category.HOME -a android.intent.action.MAIN
```
{% endraw %}