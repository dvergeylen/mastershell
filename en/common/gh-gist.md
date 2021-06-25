---
layout: default
title: "gh gist"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gh-gist">
  <a href="/en/common/gh-gist.html">gh gist</a> <a href="#gh-gist"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Work with GitHub Gists on the command-line.
> More information: <https://cli.github.com/manual/gh_gist>.

#### Create a new Gist from a space-separated list of files:
```shell
gh gist create {{path/to/files}}
```
#### Create a new Gist with a description:
```shell
gh gist create {{filename}} --desc "{{description}}"
```
#### Edit a Gist:
```shell
gh gist edit {{id_or_url}}
```
#### List Gists owned by the currently logged in user:
```shell
gh gist list --limit {{int}}
```
#### View a Gist in the default browser without rendering Markdown:
```shell
gh gist view {{id_or_url}} --web --raw
```
{% endraw %}