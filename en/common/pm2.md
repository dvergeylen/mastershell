---
layout: default
title: "pm2"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pm2">
  <a href="/en/common/pm2.html">pm2</a> <a href="#pm2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Process manager for Node.js.
> Used for log management, monitoring and configuring processes.
> More information: <https://pm2.keymetrics.io>.

#### Start a process with a name that can be used for later operations:
```shell
pm2 start {{app.js}} --name {{myapp}}
```
#### List processes:
```shell
pm2 list
```
#### Monitor all processes:
```shell
pm2 monit
```
#### Stop a process:
```shell
pm2 stop {{myapp}}
```
#### Restart a process:
```shell
pm2 restart {{myapp}}
```
#### Dump all processes for resurrecting them later:
```shell
pm2 save
```
#### Resurrect previously dumped processes:
```shell
pm2 resurrect
```
{% endraw %}