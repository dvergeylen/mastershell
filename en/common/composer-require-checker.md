---
layout: default
title: "composer-require-checker"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="composer-require-checker">
  <a href="/en/common/composer-require-checker.html">composer-require-checker</a> <a href="#composer-require-checker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A CLI tool to analyse Composer dependencies for soft dependencies.
> More information: <https://github.com/maglnet/ComposerRequireChecker>.

#### Analyse a Composer JSON file:
```shell
composer-require-checker check {{path/to/composer.json}}
```
#### Analyse a Composer JSON file with a specific configuration:
```shell
composer-require-checker check --config-file {{path/to/config.json}} {{path/to/composer.json}}
```
{% endraw %}