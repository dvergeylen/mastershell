---
layout: default
title: "rapper"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rapper">
  <a href="/en/common/rapper.html">rapper</a> <a href="#rapper"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Raptor RDF parsing utility.
> Part of the Raptor RDF Syntax Library.
> More information: <http://librdf.org/raptor/rapper.html>.

#### Convert an RDF/XML document to Turtle:
```shell
rapper -i rdfxml -o turtle {{file}}
```
#### Count the number of triples in a Turtle file:
```shell
rapper -i turtle -c {{file}}
```
{% endraw %}