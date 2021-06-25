---
layout: default
title: "phpmd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="phpmd">
  <a href="/en/common/phpmd.html">phpmd</a> <a href="#phpmd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A PHP mess detector that checks for common potential problems.
> More information: <https://github.com/phpmd/phpmd>.

#### Display a list of available rulesets and formats:
```shell
phpmd
```
#### Scan a file or directory for problems using comma-separated rulesets:
```shell
phpmd {{path/to/file_or_directory}} {{xml|text|html}} {{rulesets}}
```
#### Specify the minimum priority threshold for rules:
```shell
phpmd {{path/to/file_or_directory}} {{xml|text|html}} {{rulesets}} --minimumpriority {{priority}}
```
#### Include only the specified extensions in analysis:
```shell
phpmd {{path/to/file_or_directory}} {{xml|text|html}} {{rulesets}} --suffixes {{extensions}}
```
#### Exclude the specified comma-separated directories:
```shell
phpmd {{path/to/file_or_directory}} {{xml|text|html}} {{rulesets}} --exclude {{directory_patterns}}
```
#### Output the results to a file instead of stdout:
```shell
phpmd {{path/to/file_or_directory}} {{xml|text|html}} {{rulesets}} --reportfile {{path/to/report_file}}
```
#### Ignore the use of warning-suppressive PHPDoc comments:
```shell
phpmd {{path/to/file_or_directory}} {{xml|text|html}} {{rulesets}} --strict
```
{% endraw %}