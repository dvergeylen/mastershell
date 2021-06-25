---
layout: default
title: "git clone"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-clone">
  <a href="/en/common/git-clone.html">git clone</a> <a href="#git-clone"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Clone an existing repository.
> More information: <https://git-scm.com/docs/git-clone>.

#### Clone an existing repository:
```shell
git clone {{remote_repository_location}}
```
#### Clone an existing repository into a specific directory:
```shell
git clone {{remote_repository_location}} {{path/to/directory}}
```
#### Clone an existing repository and its submodules:
```shell
git clone --recursive {{remote_repository_location}}
```
#### Clone a local repository:
```shell
git clone -l {{path/to/local/repository}}
```
#### Clone quietly:
```shell
git clone -q {{remote_repository_location}}
```
#### Clone an existing repository only fetching the 10 most recent commits on the default branch (useful to save time):
```shell
git clone --depth {{10}} {{remote_repository_location}}
```
#### Clone an existing repository only fetching a specific branch:
```shell
git clone --branch {{name}} --single-branch {{remote_repository_location}}
```
#### Clone an existing repository using a specific SSH command:
```shell
git clone --config core.sshCommand="{{ssh -i path/to/private_ssh_key}}" {{remote_repository_location}}
```
{% endraw %}