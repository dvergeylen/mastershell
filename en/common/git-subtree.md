---
layout: default
title: "git subtree"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-subtree">
  <a href="/en/common/git-subtree.html">git subtree</a> <a href="#git-subtree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool to manage project dependencies as subprojects.
> More information: <https://manpages.debian.org/testing/git-man/git-subtree.1.en.html>.

#### Add a Git repository as a subtree:
```shell
git subtree add --prefix={{path/to/directory/}} --squash {{repository_url}} {{branch_name}}
```
#### Update subtree repository to its latest commit:
```shell
git subtree pull --prefix={{path/to/directory/}} {{repository_url}} {{branch_name}}
```
#### Merge recent changes up to the latest subtree commit into the subtree:
```shell
git subtree merge --prefix={{path/to/directory/}} --squash {{repository_url}} {{branch_name}}
```
#### Push commits to a subtree repository:
```shell
git subtree push --prefix={{path/to/directory/}} {{repository_url}} {{branch_name}}
```
#### Extract a new project history from the history of a subtree:
```shell
git subtree split --prefix={{path/to/directory/}} {{repository_url}} -b {{branch_name}}
```
{% endraw %}