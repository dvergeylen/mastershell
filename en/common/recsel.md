---
layout: default
title: "recsel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="recsel">
  <a href="/en/common/recsel.html">recsel</a> <a href="#recsel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print records from a recfile: a human-editable, plain text database.
> More information: <https://www.gnu.org/software/recutils/manual/recutils.html>.

#### Extract name and version field:
```shell
recsel -p name,version {{data.rec}}
```
#### Use "~" to match a string with a given regular expression:
```shell
recsel -e "{{field_name}} ~ '{{regular_expression}}' {{data.rec}}"
```
#### Use a predicate to match a name and a version:
```shell
recsel -e "name ~ '{{regular_expression}}' && version ~ '{{regular_expression}}'" {{data.rec}}
```
{% endraw %}