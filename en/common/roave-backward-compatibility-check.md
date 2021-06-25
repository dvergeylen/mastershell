---
layout: default
title: "roave-backward-compatibility-check"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="roave-backward-compatibility-check">
  <a href="/en/common/roave-backward-compatibility-check.html">roave-backward-compatibility-check</a> <a href="#roave-backward-compatibility-check"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool that can be used to verify backward compatibility breaks between two versions of a PHP library.
> More information: <https://github.com/Roave/BackwardCompatibilityCheck>.

#### Check for breaking changes since the last tag:
```shell
roave-backward-compatibility-check
```
#### Check for breaking changes since a specific tag:
```shell
roave-backward-compatibility-check --from={{git_reference}}
```
#### Check for breaking changes between the last tag and a specific reference:
```shell
roave-backward-compatibility-check --to={{git_reference}}
```
#### Check for breaking changes and output to Markdown:
```shell
roave-backward-compatibility-check --format=markdown > {{results.md}}
```
{% endraw %}