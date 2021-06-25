---
layout: default
title: "mitmdump"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mitmdump">
  <a href="/en/common/mitmdump.html">mitmdump</a> <a href="#mitmdump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View, record, and programmatically transform HTTP traffic.
> The command-line counterpart to mitmproxy.
> More information: <https://docs.mitmproxy.org/stable/overview-tools/#mitmdump>.

#### Start a proxy and save all output to a file:
```shell
mitmdump -w {{filename}}
```
#### Filter a saved traffic file to just POST requests:
```shell
mitmdump -nr {{input_filename}} -w {{output_filename}} "{{~m post}}"
```
#### Replay a saved traffic file:
```shell
mitmdump -nc {{filename}}
```
{% endraw %}