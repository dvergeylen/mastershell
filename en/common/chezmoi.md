---
layout: default
title: "Chezmoi"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chezmoi">
  <a href="/en/common/chezmoi.html">Chezmoi</a> <a href="#chezmoi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A multi-machine dotfile manager, written in Go.
> More information: <https://chezmoi.io>.

#### Initialize chezmoi on your machine:
```shell
chezmoi init
```
#### Tell chezmoi to manage a dotfile:
```shell
chezmoi add {{path/to/file}}
```
#### Edit the source state of a tracked dotfile:
```shell
chezmoi edit {{path/to/file}}
```
#### See changes chezmoi would make:
```shell
chezmoi diff
```
#### Apply the changes:
```shell
chezmoi -v apply
```
#### Set chezmoi up on another machine by downloading existing dotfiles from a Git repository:
```shell
chezmoi init {{https://example.com/path/to/repository.git}}
```
#### Fetch the latest changes from a remote repository:
```shell
chezmoi update
```
{% endraw %}