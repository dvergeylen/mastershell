---
layout: default
title: "sphinx-build"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sphinx-build">
  <a href="/en/common/sphinx-build.html">sphinx-build</a> <a href="#sphinx-build"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sphinx documentation generator.
> More information: <http://www.sphinx-doc.org/en/master/man/sphinx-build.html>.

#### Build documentation:
```shell
sphinx-build -b {{html|epub|text|latex|man|...}} {{path/to/source_dir}} {{path/to/build_dir}}
```
#### Build documentations intended for readthedocs.io (requires the sphinx-rtd-theme pip package):
```shell
sphinx-build -b {{html}} {{path/to/docs_dir}} {{path/to/build_dir}}
```
{% endraw %}