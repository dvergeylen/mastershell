---
layout: default
title: "linkchecker"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="linkchecker">
  <a href="/en/common/linkchecker.html">linkchecker</a> <a href="#linkchecker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line client to check HTML documents and websites for broken links.
> More information: <https://linkchecker.github.io/linkchecker/>.

#### Find broken links on https://example.com/:
```shell
linkchecker {{https://example.com/}}
```
#### Also check URLs that point to external domains:
```shell
linkchecker --check-extern {{https://example.com/}}
```
#### Ignore URLs that match a specific regular expression:
```shell
linkchecker --ignore-url {{regular_expression}} {{https://example.com/}}
```
#### Output results to a CSV file:
```shell
linkchecker --file-output {{csv}}/{{path/to/file}} {{https://example.com/}}
```
{% endraw %}