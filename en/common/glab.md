---
layout: default
title: "glab"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="glab">
  <a href="/en/common/glab.html">glab</a> <a href="#glab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> GitLab CLI tool to help working with GitLab from the command-line.
> More information: <https://clementsam.tech/glab/>.

#### Create a merge request:
```shell
glab mr create
```
#### List merge requests:
```shell
glab mr list
```
#### Create a new issue:
```shell
glab issue create
```
#### View and filter the current repository's open issues:
```shell
glab issue list
```
#### List pipelines:
```shell
glab pipeline list
```
#### Clone a repository into a specific directory:
```shell
glab repo clone {{user}}/{{repository}} {{directory}}
```
{% endraw %}