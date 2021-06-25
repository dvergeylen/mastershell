---
layout: default
title: "xgettext"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xgettext">
  <a href="/en/common/xgettext.html">xgettext</a> <a href="#xgettext"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Extract gettext strings from code files.
> More information: <https://www.gnu.org/software/gettext/manual/html_node/xgettext-Invocation.html>.

#### Scan file and output strings to `messages.po`:
```shell
xgettext {{path/to/input_file}}
```
#### Use a different output filename:
```shell
xgettext --output {{path/to/output_file}} {{path/to/input_file}}
```
#### Append new strings to an existing file:
```shell
xgettext --join-existing --output {{path/to/output_file}} {{path/to/input_file}}
```
#### Don't add a header containing metadata to the output file:
```shell
xgettext --omit-header {{path/to/input_file}}
```
{% endraw %}