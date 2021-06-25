---
layout: default
title: "disown"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="disown">
  <a href="/en/linux/disown.html">disown</a> <a href="#disown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Allow sub-processes to live beyond the shell that they are attached to.
> See also the `jobs` command.

#### Disown the current job:
```shell
disown
```
#### Disown a specific job:
```shell
disown %{{job_number}}
```
#### Disown all jobs:
```shell
disown -a
```
#### Keep job (do not disown it), but mark it so that no future SIGHUP is received on shell exit:
```shell
disown -h %{{job_number}}
```
{% endraw %}