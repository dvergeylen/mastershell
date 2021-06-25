---
layout: default
title: "progress"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="progress">
  <a href="/en/linux/progress.html">progress</a> <a href="#progress"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display/Monitor the progress of running coreutils.
> More information: <https://github.com/Xfennec/progress>.

#### Show the progress of running coreutils:
```shell
progress
```
#### Show the progress of running coreutils in quiet mode:
```shell
progress -q
```
#### Launch and monitor a single long-running command:
```shell
{{command}} & progress -mp $!
```
{% endraw %}