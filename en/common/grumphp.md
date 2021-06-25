---
layout: default
title: "grumphp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="grumphp">
  <a href="/en/common/grumphp.html">grumphp</a> <a href="#grumphp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A PHP Composer plugin that enables source code quality checks.
> More information: <https://github.com/phpro/grumphp>.

#### Register the Git hooks:
```shell
grumphp git:init
```
#### Trigger the pre-commit hook manually:
```shell
grumphp git:pre-commit
```
#### Check every versioned file:
```shell
grumphp run
```
{% endraw %}