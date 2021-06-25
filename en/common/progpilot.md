---
layout: default
title: "progpilot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="progpilot">
  <a href="/en/common/progpilot.html">progpilot</a> <a href="#progpilot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A PHP static analysis tool for detecting security vulnerabilities.
> More information: <https://github.com/designsecurity/progpilot>.

#### Analyse the current directory:
```shell
progpilot
```
#### Analyse a specific file or directory:
```shell
progpilot {{path/to/file_or_directory}}
```
#### Specify a custom configuration file:
```shell
progpilot --configuration {{path/to/configuration.yml}}
```
{% endraw %}