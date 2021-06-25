---
layout: default
title: "dget"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dget">
  <a href="/en/linux/dget.html">dget</a> <a href="#dget"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Download Debian packages.
> More information: <https://manpages.debian.org/dget>.

#### Download a binary package:
```shell
dget {{package_name}}
```
#### Download and extract a package source from its `.dsc` file:
```shell
dget {{http://deb.debian.org/debian/pool/main/h/haskell-tldr/haskell-tldr_0.4.0-2.dsc}}
```
#### Download a package source tarball from its `.dsc` file but don't extract it:
```shell
dget -d {{http://deb.debian.org/debian/pool/main/h/haskell-tldr/haskell-tldr_0.4.0-2.dsc}}
```
{% endraw %}