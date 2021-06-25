---
layout: default
title: "shc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="shc">
  <a href="/en/common/shc.html">shc</a> <a href="#shc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generic shell script compiler.

#### Compile a shell script:
```shell
shc -f {{script}}
```
#### Compile a shell script and specify an output binary file:
```shell
shc -f {{script}} -o {{binary}}
```
#### Compile a shell script and set an expiration date for the executable:
```shell
shc -f {{script}} -e {{dd/mm/yyyy}}
```
#### Compile a shell script and set a message to display upon expiration:
```shell
shc -f {{script}} -e {{dd/mm/yyyy}} -m "{{Please contact your provider}}"
```
{% endraw %}