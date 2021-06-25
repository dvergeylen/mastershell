---
layout: default
title: "screenfetch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="screenfetch">
  <a href="/en/common/screenfetch.html">screenfetch</a> <a href="#screenfetch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display system information.
> More information: <https://github.com/KittyKatt/screenFetch>.

#### Start screenfetch:
```shell
screenfetch
```
#### Take a screenshot (requires 'scrot'):
```shell
screenfetch -s
```
#### Specify distribution logo:
```shell
screenfetch -A '{{distribution_name}}'
```
#### Specify distribution logo and text:
```shell
screenfetch -D '{{distribution_name}}'
```
#### Strip all color:
```shell
screenfetch -N
```
{% endraw %}