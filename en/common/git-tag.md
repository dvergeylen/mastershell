---
layout: default
title: "git tag"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-tag">
  <a href="/en/common/git-tag.html">git tag</a> <a href="#git-tag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create, list, delete or verify tags.
> A tag is a static reference to a specific commit.
> More information: <https://git-scm.com/docs/git-tag>.

#### List all tags:
```shell
git tag
```
#### Create a tag with the given name pointing to the current commit:
```shell
git tag {{tag_name}}
```
#### Create a tag with the given name pointing to a given commit:
```shell
git tag {{tag_name}} {{commit}}
```
#### Create an annotated tag with the given message:
```shell
git tag {{tag_name}} -m {{tag_message}}
```
#### Delete the tag with the given name:
```shell
git tag -d {{tag_name}}
```
#### Get updated tags from upstream:
```shell
git fetch --tags
```
#### List all tags whose ancestors include a given commit:
```shell
git tag --contains {{commit}}
```
{% endraw %}