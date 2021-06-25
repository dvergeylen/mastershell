---
layout: default
title: "surfraw"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="surfraw">
  <a href="/en/common/surfraw.html">surfraw</a> <a href="#surfraw"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI to query a variety of web search engines.
> Consists of a collection of elvi, each of which knows how to search a specific website.
> More information: <http://surfraw.org>.

#### Display the list of supported website search scripts (elvi):
```shell
surfraw -elvi
```
#### Open the elvi's results page for a specific search in the browser:
```shell
surfraw {{elvi}} "{{search_terms}}"
```
#### Display an elvi description and its specific options:
```shell
surfraw {{elvi}} -local-help
```
#### Search using an elvi with specific options and open the results page in the browser:
```shell
surfraw {{elvi}} {{elvi_options}} "{{search_terms}}"
```
#### Display the URL to the elvi's results page for a specific search:
```shell
surfraw -print {{elvi}} "{{search_terms}}"
```
#### Search using the alias:
```shell
sr {{elvi}} "{{search_terms}}"
```
{% endraw %}