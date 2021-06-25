---
layout: default
title: "security-checker"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="security-checker">
  <a href="/en/common/security-checker.html">security-checker</a> <a href="#security-checker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Check if a PHP application uses dependencies with known security vulnerabilities.
> More information: <https://github.com/sensiolabs/security-checker>.

#### Look for security issues in the project dependencies (based on the `composer.lock` file in the current directory):
```shell
security-checker security:check
```
#### Use a specific `composer.lock` file:
```shell
security-checker security:check {{path/to/composer.lock}}
```
#### Return results as a JSON object:
```shell
security-checker security:check --format=json
```
{% endraw %}