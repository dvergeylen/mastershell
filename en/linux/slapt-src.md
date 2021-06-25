---
layout: default
title: "slapt-src"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="slapt-src">
  <a href="/en/linux/slapt-src.html">slapt-src</a> <a href="#slapt-src"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A utility to automate building of slackbuilds.
> SlackBuild sources need to be configured in the slapt-srcrc file.
> More information: <https://github.com/jaos/slapt-src>.

#### Update the list of available slackbuilds and versions:
```shell
slapt-src --update
```
#### List all available slackbuilds:
```shell
slapt-src --list
```
#### Fetch, build and install the specified slackbuild(s):
```shell
slapt-src --install {{slackbuild_name}}
```
#### Locate slackbuilds of interest by their name or description:
```shell
slapt-src --search {{search_term}}
```
#### Display information about a slackbuild:
```shell
slapt-src --show {{slackbuild_name}}
```
{% endraw %}