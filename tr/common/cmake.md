---
layout: default
title: "cmake"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmake">
  <a href="/tr/common/cmake.html">cmake</a> <a href="#cmake"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Çok platformlu yapım sistem oluşturucusu.
> Hedeflenen sisteme göre Makefile, Visual Studio projeleri ve benzerlerini oluşturur.
> Daha fazla bilgi için: <https://cmake.org/cmake/help/latest/manual/cmake.1.html>.

#### Bir Makefile oluştur ve onu aynı dizindeki bir projeyi derlemek için kullan:
```shell
cmake && make
```
#### Bir Makefile oluştur ve onu farklı bir "yapim" dizinindeki projeyi derlemek için kullan (kaynak-dışı yapım):
```shell
cmake -H. -B {{build}} && make -C {{yapim}}
```
{% endraw %}