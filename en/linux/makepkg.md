---
layout: default
title: "makepkg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="makepkg">
  <a href="/en/linux/makepkg.html">makepkg</a> <a href="#makepkg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates a package installable with the `pacman` package manager.
> Runs the commands from a `PKGBUILD` file to build the package.
> More information: <https://wiki.archlinux.org/index.php/Makepkg>.

#### Make a package (run in the same directory as a `PKGBUILD`):
```shell
makepkg
```
#### Make a package and install its dependencies:
```shell
makepkg --syncdeps
```
#### Same as above, but install the package with `pacman` when done:
```shell
makepkg --syncdeps --install
```
#### Make a package, but skip source checksums:
```shell
makepkg --skipchecksums
```
{% endraw %}