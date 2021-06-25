---
layout: default
title: "cowsay"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cowsay">
  <a href="/en/common/cowsay.html">cowsay</a> <a href="#cowsay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print ASCII art (by default a cow) saying or thinking something.
> More information: <https://github.com/tnalpgge/rank-amateur-cowsay>.

#### Print an ASCII cow saying "hello, world":
```shell
cowsay "{{hello, world}}"
```
#### Print an ASCII cow saying text from stdin:
```shell
echo "{{hello, world}}" | cowsay
```
#### List all available art types:
```shell
cowsay -l
```
#### Print the specified ASCII art saying "hello, world":
```shell
cowsay -f {{art}} "{{hello, world}}"
```
#### Print a dead thinking ASCII cow:
```shell
cowthink -d "{{I'm just a cow, not a great thinker...}}"
```
#### Print an ASCII cow with custom eyes saying "hello, world":
```shell
cowsay -e {{characters}} "{{hello, world}}"
```
{% endraw %}