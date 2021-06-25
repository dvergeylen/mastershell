---
layout: default
title: "git lfs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-lfs">
  <a href="/en/common/git-lfs.html">git lfs</a> <a href="#git-lfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Work with large files in Git repositories.
> More information: <https://git-lfs.github.com>.

#### Initialise Git LFS:
```shell
git lfs install
```
#### Track files that match a glob:
```shell
git lfs track '{{*.bin}}'
```
#### Change the Git LFS endpoint URL (useful if the LFS server is separate from the Git server):
```shell
git config -f .lfsconfig lfs.url {{lfs_endpoint_url}}
```
#### List tracked patterns:
```shell
git lfs track
```
#### List tracked files that have been committed:
```shell
git lfs ls-files
```
#### Push all Git LFS objects to the remote server (useful if errors are encountered):
```shell
git lfs push --all {{remote_name}} {{branch_name}}
```
#### Fetch all Git LFS objects:
```shell
git lfs fetch
```
#### Checkout all Git LFS objects:
```shell
git lfs checkout
```
{% endraw %}