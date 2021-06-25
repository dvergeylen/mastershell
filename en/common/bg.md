---
layout: default
title: "bg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bg">
  <a href="/en/common/bg.html">bg</a> <a href="#bg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Resumes jobs that have been suspended (e.g. using `Ctrl + Z`), and keeps them running in the background.
> More information: <https://manned.org/bg>.

#### Resume the most recently suspended job and run it in the background:
```shell
bg
```
#### Resume a specific job (use `jobs -l` to get its ID) and run it in the background:
```shell
bg %{{job_id}}
```
{% endraw %}