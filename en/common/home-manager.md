---
layout: default
title: "home-manager"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="home-manager">
  <a href="/en/common/home-manager.html">home-manager</a> <a href="#home-manager"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage a user environment using Nix.
> More information: <https://github.com/rycee/home-manager>.

#### Activate the configuration defined in `~/.config/nixpkgs/home.nix`:
```shell
home-manager build
```
#### Activate the configuration and switch to it:
```shell
home-manager switch
```
{% endraw %}