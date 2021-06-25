---
layout: default
title: "zmv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zmv">
  <a href="/en/common/zmv.html">zmv</a> <a href="#zmv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Move or rename files matching a specified extended glob pattern.
> See also `zcp` and `zln`.
> More information: <http://zsh.sourceforge.net/Doc/Release/User-Contributions.html>.

#### Move files using a regular expression-like pattern:
```shell
zmv '{{(*).log}}' '{{$1.txt}}'
```
#### Preview the result of a move, without making any actual changes:
```shell
zmv -n '{{(*).log}}' '{{$1.txt}}'
```
#### Interactively move files, with a prompt before every change:
```shell
zmv -i '{{(*).log}}' '{{$1.txt}}'
```
#### Verbosely print each action as it's being executed:
```shell
zmv -v '{{(*).log}}' '{{$1.txt}}'
```
{% endraw %}