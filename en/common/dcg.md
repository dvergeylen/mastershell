---
layout: default
title: "dcg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dcg">
  <a href="/en/common/dcg.html">dcg</a> <a href="#dcg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Drupal code generator.
> More information: <https://github.com/Chi-teck/drupal-code-generator>.

#### Start a wizard to choose what kind of code (e.g. module, service, form, etc.) to generate:
```shell
dcg
```
#### Directly specify the kind of code to generate:
```shell
dcg {{service|plugin|theme|module|form}}
```
#### Generate the code in a specific directory:
```shell
dcg --directory {{path/to/directory}}
```
{% endraw %}