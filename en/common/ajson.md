---
layout: default
title: "ajson"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ajson">
  <a href="/en/common/ajson.html">ajson</a> <a href="#ajson"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Executes JSONPath on JSON objects.
> More information: <https://github.com/spyzhov/ajson>.

#### Read JSON from a file and execute a specified JSONPath expression:
```shell
ajson '{{$..json[?(@.path)]}}' {{path/to/file.json}}
```
#### Read JSON from stdin and execute a specified JSONPath expression:
```shell
cat {{path/to/file.json}} | ajson '{{$..json[?(@.path)]}}'
```
#### Read JSON from a URL and evaluate a specified JSONPath expression:
```shell
ajson '{{avg($..price)}}' '{{https://example.com/api/}}'
```
#### Read some simple JSON and calculate a value:
```shell
echo '{{3}}' | ajson '{{2 * pi * $}}'
```
{% endraw %}