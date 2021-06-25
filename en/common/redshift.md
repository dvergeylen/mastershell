---
layout: default
title: "redshift"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="redshift">
  <a href="/en/common/redshift.html">redshift</a> <a href="#redshift"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Adjust the color temperature of your screen according to your surroundings.
> More information: <https://jonls.dk/redshift>.

#### Turn on Redshift with 5700K temperature during day and 3600K at night:
```shell
redshift -t {{5700}}:{{3600}}
```
#### Turn on Redshift with a manually-specified custom location:
```shell
redshift -l {{latitude}}:{{longitude}}
```
#### Turn on Redshift with 70% screen brightness during day and 40% brightness at night:
```shell
redshift -b {{0.7}}:{{0.4}}
```
#### Turn on Redshift with custom gamma levels (between 0 and 1):
```shell
redshift -g {{red}}:{{green}}:{{blue}}
```
#### Turn on Redshift with a constant unchanging color temperature:
```shell
redshift -O {{temperature}}
```
{% endraw %}