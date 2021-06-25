---
layout: default
title: "paccache"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="paccache">
  <a href="/en/linux/paccache.html">paccache</a> <a href="#paccache"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A pacman cache cleaning utility.

#### Remove all but the 3 most recent package versions from the pacman cache:
```shell
paccache -r
```
#### Set the number of package versions to keep:
```shell
paccache -rk {{num_versions}}
```
#### Perform a dry-run and show the number of candidate packages for deletion:
```shell
paccache -d
```
#### Move candidate packages to a directory instead of deleting them:
```shell
paccache -m {{path/to/directory}}
```
{% endraw %}