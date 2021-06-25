---
layout: default
title: "gitmoji"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gitmoji">
  <a href="/en/common/gitmoji.html">gitmoji</a> <a href="#gitmoji"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An interactive command-line tool for using emojis on commits.
> More information: <https://github.com/carloscuesta/gitmoji-cli>.

#### Start the commit wizard:
```shell
gitmoji --commit
```
#### Initialize the git hook (so `gitmoji` will be run every time `git commit` is run):
```shell
gitmoji --init
```
#### Remove the git hook:
```shell
gitmoji --remove
```
#### List all available emojis and their descriptions:
```shell
gitmoji --list
```
#### Search emoji list for a list of keywords:
```shell
gitmoji --search {{keyword1}} {{keyword2}}
```
#### Update cached list of emojis from main repository:
```shell
gitmoji --update
```
#### Configure global preferences:
```shell
gitmoji --config
```
{% endraw %}