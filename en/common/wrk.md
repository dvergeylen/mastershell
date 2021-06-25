---
layout: default
title: "wrk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wrk">
  <a href="/en/common/wrk.html">wrk</a> <a href="#wrk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> HTTP benchmarking tool.
> More information: <https://github.com/wg/wrk>.

#### Run a benchmark for `30` seconds, using `12` threads, and keeping `400` HTTP connections open:
```shell
wrk -t{{12}} -c{{400}} -d{{30s}} "{{http://127.0.0.1:8080/index.html}}"
```
#### Run a benchmark with a custom header:
```shell
wrk -t{{2}} -c{{5}} -d{{5s}} -H "{{Host: example.com}}" "{{http://example.com/index.html}}"
```
#### Run a benchmark with a request timeout of `2` seconds:
```shell
wrk -t{{2}} -c{{5}} -d{{5s}} --timeout {{2s}} "{{http://example.com/index.html}}"
```
{% endraw %}