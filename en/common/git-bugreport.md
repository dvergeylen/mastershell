---
layout: default
title: "git bugreport"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-bugreport">
  <a href="/en/common/git-bugreport.html">git bugreport</a> <a href="#git-bugreport"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Captures debug information from the system and user, generating a text file to aid in the reporting of a bug in Git.
> More information: <https://git-scm.com/docs/git-bugreport>.

#### Create a new bugreport file in the current directory:
```shell
git bugreport
```
#### Create a new bugreport file in the specified directory, creating it if it does not exist:
```shell
git bugreport --output-directory {{path/to/directory}}
```
#### Create a new bugreport file with the specified filename suffix in `strftime` format:
```shell
git bugreport --suffix {{%m%d%y}}
```
{% endraw %}