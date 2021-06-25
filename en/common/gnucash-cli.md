---
layout: default
title: "gnucash-cli"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gnucash-cli">
  <a href="/en/common/gnucash-cli.html">gnucash-cli</a> <a href="#gnucash-cli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line version of GnuCash.
> More information: <https://gnucash.org>.

#### Get quotes for currencies and stocks specified in a file and print them:
```shell
gnucash-cli --quotes get {{path/to/file.gnucash}}
```
#### Generate a financial report of a specific type, specified by `--name`:
```shell
gnucash-cli --report run --name "{{Balance Sheet}}" {{path/to/file.gnucash}}
```
{% endraw %}