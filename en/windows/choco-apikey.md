---
layout: default
title: "choco-apikey"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-apikey">
  <a href="/en/windows/choco-apikey.html">choco-apikey</a> <a href="#choco-apikey"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage API keys for Chocolatey sources.
> More information: <https://chocolatey.org/docs/commands-apikey>.

#### Display a list of sources and their API keys:
```shell
choco apikey
```
#### Display a specific source and its API key:
```shell
choco apikey --source "{{source_url}}"
```
#### Set an API key for a source:
```shell
choco apikey --source "{{source_url}}" --key "{{api_key}}"
```
#### Remove an API key for a source:
```shell
choco apikey --source "{{source_url}}" --remove
```
{% endraw %}