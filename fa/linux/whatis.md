---
layout: default
title: "whatis"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="whatis">
  <a href="/fa/linux/whatis.html">whatis</a> <a href="#whatis"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> نمایش توضیحات یک خطی از صفحات راهنما.

#### نمایش توضیحات یک دستور از صفحات راهنما:
```shell
whatis {{command}}
```
#### توضیحات در آخر خط ترمینال برش نمی خورد:
```shell
whatis --long {{command}}
```
#### نمایش توضیحات تمامی دستورات مطابق با الگو:
```shell
whatis --wildcard {{net*}}
```
#### جستجو در توضیحات صفحات راهنما با عبارات منظم:
```shell
whatis --regex '{{wish[0-9]\.[0-9]}}'
```
{% endraw %}