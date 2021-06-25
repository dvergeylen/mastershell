---
layout: default
title: "direnv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="direnv">
  <a href="/en/common/direnv.html">direnv</a> <a href="#direnv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Shell extension to load and unload environment variables depending on the current directory.
> More information: <https://github.com/direnv/direnv>.

#### Grant direnv permission to load the specified `.envrc`:
```shell
direnv allow
```
#### Revoke the authorization of a given `.envrc`:
```shell
direnv deny
```
#### Edit the `.envrc` file in the default text editor and reload the environment on exit:
```shell
direnv edit .
```
#### Trigger a reload of the environment:
```shell
direnv reload
```
#### Print some debug status information:
```shell
direnv status
```
{% endraw %}