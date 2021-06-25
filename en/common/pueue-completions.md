---
layout: default
title: "pueue completions"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pueue-completions">
  <a href="/en/common/pueue-completions.html">pueue completions</a> <a href="#pueue-completions"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generates shell completion files for bash, elvish, fish, powershell, and zsh.
> More information: <https://github.com/Nukesor/pueue>.

#### Generate completions for bash:
```shell
sudo pueue completions bash {{/usr/share/bash-completion/completions/pueue.bash}}
```
#### Generate completions for zsh:
```shell
sudo pueue completions zsh {{/usr/share/zsh/site-functions}}
```
#### Generate completions for fish:
```shell
sudo pueue completions fish {{/usr/share/fish/completions}}
```
{% endraw %}