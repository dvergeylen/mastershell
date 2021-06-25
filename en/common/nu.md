---
layout: default
title: "nu"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nu">
  <a href="/en/common/nu.html">nu</a> <a href="#nu"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Nushell ("a new type of shell") takes a modern, structured approach to your command-line.
> More information: <https://www.nushell.sh>.

#### Start an interactive shell session:
```shell
nu
```
#### Execute a command and then exit:
```shell
nu --commands "{{command}}"
```
#### Execute a script:
```shell
nu {{path/to/script.nu}}
```
#### Execute a script with logging:
```shell
nu --loglevel {{error|warn|info|debug|trace}} {{path/to/script.nu}}
```
#### Print the Nushell version:
```shell
nu --version
```
{% endraw %}