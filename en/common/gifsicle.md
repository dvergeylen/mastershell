---
layout: default
title: "gifsicle"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gifsicle">
  <a href="/en/common/gifsicle.html">gifsicle</a> <a href="#gifsicle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create GIFs.
> More information: <https://www.lcdf.org/gifsicle>.

#### Optimise a GIF:
```shell
gifsicle --batch --optimize=3 {{amin.gif}}
```
#### Make a GIF animation with gifsicle:
```shell
gifsicle --delay={{10}} --loop *.gif > {{anim.gif}}
```
#### Extract frames from an animation:
```shell
gifsicle {{anim.gif}} '#0' > {{firstframe.gif}}
```
#### You can also edit animations by replacing, deleting, or inserting frames:
```shell
gifsicle -b {{anim.gif}} --replace '#0' {{new.gif}}
```
{% endraw %}