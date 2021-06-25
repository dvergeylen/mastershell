---
layout: default
title: "fsck"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fsck">
  <a href="/en/linux/fsck.html">fsck</a> <a href="#fsck"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Check the integrity of a filesystem or repair it. The filesystem should be unmounted at the time the command is run.

#### Check filesystem `/dev/sdX`, reporting any damaged blocks:
```shell
fsck {{/dev/sdX}}
```
#### Check filesystem `/dev/sdX`, reporting any damaged blocks and interactively letting the user choose to repair each one:
```shell
fsck -r {{/dev/sdX}}
```
#### Check filesystem `/dev/sdX`, reporting any damaged blocks and automatically repairing them:
```shell
fsck -a {{/dev/sdX}}
```
{% endraw %}