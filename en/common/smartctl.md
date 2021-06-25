---
layout: default
title: "smartctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="smartctl">
  <a href="/en/common/smartctl.html">smartctl</a> <a href="#smartctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View a disk's SMART data and other information.
> More information: <https://en.wikipedia.org/wiki/S.M.A.R.T.>.

#### View SMART health summary:
```shell
sudo smartctl --health {{/dev/sdX}}
```
#### View device information:
```shell
sudo smartctl --info {{/dev/sdX}}
```
#### Begin a short self-test:
```shell
sudo smartctl --test short {{/dev/sdX}}
```
#### View current/last self-test status and other SMART capabilities:
```shell
sudo smartctl --capabilities {{/dev/sdX}}
```
#### View SMART self-test log (if supported):
```shell
sudo smartctl --log selftest {{/dev/sdX}}
```
{% endraw %}