---
layout: default
title: "gh release"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gh-release">
  <a href="/en/common/gh-release.html">gh release</a> <a href="#gh-release"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage GitHub releases from the command-line.
> More information: <https://cli.github.com/manual/gh_release>.

#### List releases in a GitHub repository, limited to 30 items:
```shell
gh release list
```
#### Display information about a specific release:
```shell
gh release view {{tag}}
```
#### Create a new release:
```shell
gh release create {{tag}}
```
#### Delete a specific release:
```shell
gh release delete {{tag}}
```
#### Download assets from a specific release:
```shell
gh release download {{tag}}
```
#### Upload assets to a specific release:
```shell
gh release upload {{tag}} {{path/to/file1}} {{path/to/file2}}
```
{% endraw %}