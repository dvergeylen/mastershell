---
layout: default
title: "kosmorro"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kosmorro">
  <a href="/en/common/kosmorro.html">kosmorro</a> <a href="#kosmorro"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compute the ephemerides and the events for a given date, at a given position on Earth.
> More information: <http://kosmorro.space>.

#### Get ephemerides for Paris, France:
```shell
kosmorro --latitude={{48.7996}} --longitude={{2.3511}}
```
#### Get ephemerides for Paris, France, in the UTC+2 timezone:
```shell
kosmorro --latitude={{48.7996}} --longitude={{2.3511}} --timezone={{2}}
```
#### Get ephemerides for Paris, France, on June 9th, 2020:
```shell
kosmorro --latitude={{48.7996}} --longitude={{2.3511}} --date={{2020-06-09}}
```
#### Generate a PDF (note: TeXLive must be installed):
```shell
kosmorro --format={{pdf}} --output={{path/to/file.pdf}}
```
{% endraw %}