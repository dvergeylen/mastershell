---
layout: default
title: "base64"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="base64">
  <a href="/nl/common/base64.html">base64</a> <a href="#base64"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Codeer of decodeer bestand of standaardinvoer van/naar Base64 naar standaarduitvoer.
> Meer informatie: <https://www.gnu.org/software/coreutils/base64>.

#### Codeer een bestand:
```shell
base64 {{bestandsnaam}}
```
#### Decodeer een bestand:
```shell
base64 --decode {{bestandsnaam}}
```
#### Codeer stdin:
```shell
{{eencommando}} | base64
```
#### Decodeer stdin:
```shell
{{eencommando}} | base64 --decode
```
{% endraw %}