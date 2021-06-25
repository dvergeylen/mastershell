---
layout: default
title: "compare"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="compare">
  <a href="/de/common/compare.html">compare</a> <a href="#compare"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeige Unterschiede von zwei Bildern.
> Weitere Informationen: <https://imagemagick.org/script/compare.php>.

#### Vergleiche 2 Bilder:
```shell
compare {{pfad/zu/bild1.png}} {{pfad/zu/bild2.png}} {{pfad/zu/diff.png}}
```
#### Vergleiche 2 Bilder mit einer bestimmten Metrik (standardmäßig NCC):
```shell
compare -verbose -metric {{PSNR}} {{pfad/zu/bild1.png}} {{pfad/zu/bild2.png}} {{pfad/zu/diff.png}}
```
{% endraw %}