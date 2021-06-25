---
layout: default
title: "starship init"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="starship-init">
  <a href="/en/common/starship-init.html">starship init</a> <a href="#starship-init"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print shell integration code for starship.
> More information: <https://starship.rs>.

#### Display the subcommand help:
```shell
starship init --help
```
#### Print the starship integration code for the specified shell:
```shell
starship init {{bash|elvish|fish|ion|powershell|tcsh|zsh}}
```
#### Append the `starship` integration code to `~/.bashrc`:
```shell
starship init {{bash}} >> {{~/.bashrc}}
```
#### Append the `starship` integration code to `~/.zshrc`:
```shell
starship init {{zsh]} >> {{~/.zshrc}}
```
{% endraw %}