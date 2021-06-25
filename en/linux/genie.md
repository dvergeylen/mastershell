---
layout: default
title: "genie"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="genie">
  <a href="/en/linux/genie.html">genie</a> <a href="#genie"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set up and use a "bottle" namespace to run systemd under WSL (Windows Subsystem for Linux).
> To run these from Windows rather than an already-running distribution, precede them with `wsl`.
> More information: <https://github.com/arkane-systems/genie>.

#### Initialize the bottle (run once, at start):
```shell
genie -i
```
#### Run a login shell inside the bottle:
```shell
genie -s
```
#### Run a specified command inside the bottle:
```shell
genie -c {{command}}
```
{% endraw %}