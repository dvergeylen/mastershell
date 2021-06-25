---
layout: default
title: "gnomon"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gnomon">
  <a href="/en/common/gnomon.html">gnomon</a> <a href="#gnomon"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to annotate console logging statements with timestamps and find slow processes.
> More information: <https://github.com/paypal/gnomon>.

#### Use UNIX (or DOS) pipes to pipe the stdout of any command through gnomon:
```shell
{{npm test}} | gnomon
```
#### Show number of seconds since the start of the process:
```shell
{{npm test}} | gnomon --type=elapsed-total
```
#### Show an absolute timestamp in UTC:
```shell
{{npm test}} | gnomon --type=absolute
```
#### Set a high threshold of 0.5 seconds for the elapsed time; exceeding which the timestamp will be colored bright red:
```shell
{{npm test}} | gnomon --high {{0.5}}
```
#### Set a medium threshold of 0.2 seconds (Timestamp will be colored bright yellow):
```shell
{{npm test}} | gnomon --medium {{0.2}}
```
{% endraw %}