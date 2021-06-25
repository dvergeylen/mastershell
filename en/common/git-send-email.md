---
layout: default
title: "git send-email"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-send-email">
  <a href="/en/common/git-send-email.html">git send-email</a> <a href="#git-send-email"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Send a collection of patches as emails.
> Patches can be specified as files, directions, or a revision list.
> More information: <https://git-scm.com/docs/git-send-email>.

#### Send the last commit in the current branch:
```shell
git send-email -1
```
#### Send a given commit:
```shell
git send-email -1 {{commit}}
```
#### Send multiple (e.g. 10) commits in the current branch:
```shell
git send-email {{-10}}
```
#### Send an introductory email message for the patch series:
```shell
git send-email -{{number_of_commits}} --compose
```
#### Review and edit the email message for each patch you're about to send:
```shell
git send-email -{{number_of_commits}} --annotate
```
{% endraw %}