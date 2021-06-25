---
layout: default
title: "drupal-check"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="drupal-check">
  <a href="/en/common/drupal-check.html">drupal-check</a> <a href="#drupal-check"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Check Drupal PHP code for deprecations.
> More information: <https://github.com/mglaman/drupal-check>.

#### Check the code in a specific directory for deprecations:
```shell
drupal-check {{path/to/directory}}
```
#### Check the code excluding a comma-separated list of directories:
```shell
drupal-check --exclude-dir {{path/to/excluded_directory}},{{path/to/excluded_files/*.php}} {{path/to/directory}}
```
#### Don't show a progress bar:
```shell
drupal-check --no-progress {{path/to/directory}}
```
#### Perform static analysis to detect bad coding practices:
```shell
drupal-check --analysis {{path/to/directory}}
```
{% endraw %}