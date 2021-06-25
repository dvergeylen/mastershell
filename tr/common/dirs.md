---
layout: default
title: "dirs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dirs">
  <a href="/tr/common/dirs.html">dirs</a> <a href="#dirs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Dizin yığını görüntüler veya üzerinde oynama yapar.
> Dizin yığını, `pushd` ve `popd` komutlarıyla üzerinde oynama yapılabilen, son ziyaret edilen dizinleri gösteren bir listedir.
> Daha fazla bilgi için: <https://www.gnu.org/software/bash/manual/bash.html#Directory-Stack-Builtins>.

#### Dizin yığınını her madde arasında boşluk olacak şekilde görüntüle:
```shell
dirs
```
#### Dizin yığınını her satır başı tek madde olacak şekilde görüntüle:
```shell
dirs -p
```
#### Dizin yığınında 0'dan başlamak üzere yalnızca nth girişini göster:
```shell
dirs +{{N}}
```
#### Dizin yığınını temizle:
```shell
dirs -c
```
{% endraw %}