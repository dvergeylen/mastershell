---
layout: default
title: "tldr-lint"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tldr-lint">
  <a href="/en/common/tldr-lint.html">tldr-lint</a> <a href="#tldr-lint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lint and format `tldr` pages.
> More information: <https://github.com/tldr-pages/tldr-lint>.

#### Lint all pages:
```shell
tldr-lint {{pages_directory}}
```
#### Format a specific page to stdout:
```shell
tldr-lint --format {{page.md}}
```
#### Format all pages in place:
```shell
tldr-lint --format --in-place {{pages_directory}}
```
{% endraw %}