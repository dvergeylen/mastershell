---
layout: default
title: "pulseaudio"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pulseaudio">
  <a href="/tr/linux/pulseaudio.html">pulseaudio</a> <a href="#pulseaudio"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ses sistem arkaplan uygulaması ve yöneticisi.
> Daha fazla bilgi için: <https://www.freedesktop.org/wiki/Software/PulseAudio/>.

#### Pulseaudio'nun çalışıp çalışmadığını kontrol et (sıfır olmayan çıktı, çalışmadığı anlamına gelir):
```shell
pulseaudio --check
```
#### Pulseaudio'yu arkaplanda çalıştır:
```shell
pulseaudio --start
```
#### Arkaplanda çalışan tüm pulseaudio uygulamalarını öldür:
```shell
pulseaudio --kill
```
#### Müsait modülleri sırala:
```shell
pulseaudio --dump-modules
```
#### Belirtilen argümanlarla bir modülü mevcut çalışan arkaplan uygulamasına yükle:
```shell
pulseaudio --load="{{modül_ismi}} {{argümanlar}}"
```
{% endraw %}