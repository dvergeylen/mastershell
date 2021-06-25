---
layout: default
title: "svccfg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="svccfg">
  <a href="/en/sunos/svccfg.html">svccfg</a> <a href="#svccfg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Import, export, and modify service configurations.
> More information: <https://www.unix.com/man-page/linux/1m/svccfg>.

#### Validate configuration file:
```shell
svccfg validate {{smf.xml}}
```
#### Export service configurations to file:
```shell
svccfg export {{servicename}} > {{smf.xml}}
```
#### Import/update service configurations from file:
```shell
svccfg import {{smf.xml}}
```
{% endraw %}