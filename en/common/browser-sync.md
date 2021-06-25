---
layout: default
title: "browser-sync"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="browser-sync">
  <a href="/en/common/browser-sync.html">browser-sync</a> <a href="#browser-sync"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Starts local web server that updates browser on file changes.
> More information: <https://browsersync.io/docs/command-line>.

#### Start a server from a specific directory:
```shell
browser-sync start --server {{path/to/directory}} --files {{path/to/directory}}
```
#### Start a server from local directory, watching all css files in some directory:
```shell
browser-sync start --server --files '{{path/to/directory/*.css}}'
```
#### Create configuration file:
```shell
browser-sync init
```
#### Start browser-sync from config file:
```shell
browser-sync start --config {{config_file}}
```
{% endraw %}