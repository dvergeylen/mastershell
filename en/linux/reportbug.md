---
layout: default
title: "reportbug"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reportbug">
  <a href="/en/linux/reportbug.html">reportbug</a> <a href="#reportbug"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bug report tool of Debian distribution.
> More information: <https://manpages.debian.org/buster/reportbug/reportbug.1.en.html>.

#### Generate a bug report about a specific package, then send it by e-mail:
```shell
reportbug {{package}}
```
#### Report a bug that is not about a specific package (general problem, infrastructure, etc.):
```shell
reportbug other
```
#### Write the bug report to a file instead of sending it by e-mail:
```shell
reportbug -o {{filename}} {{package}}
```
{% endraw %}