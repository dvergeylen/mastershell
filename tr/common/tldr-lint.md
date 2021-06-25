---
layout: default
title: "tldr-lint"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tldr-lint">
  <a href="/tr/common/tldr-lint.html">tldr-lint</a> <a href="#tldr-lint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> `tldr` sayfalarını gözden geçir ve biçimlendir.
> Daha fazla bilgi için: <https://github.com/tldr-pages/tldr-lint>.

#### Tüm sayfaları gözden geçir:
```shell
tldr-lint {{sayfa_dizini}}
```
#### Belirtilmiş bir sayfayı stdout'a biçimlendir:
```shell
tldr-lint --format {{page.md}}
```
#### Bir konumdaki tüm sayfaları biçimlendir:
```shell
tldr-lint --format --in-place {{sayfa_dizini}}
```
{% endraw %}