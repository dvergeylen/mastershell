---
layout: default
title: "diffstat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="diffstat">
  <a href="/en/common/diffstat.html">diffstat</a> <a href="#diffstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create a histogram from the output of the `diff` command.
> More information: <https://manned.org/diffstat>.

#### Display changes in a histogram:
```shell
diff {{file1}} {{file2}} | diffstat
```
#### Display inserted, deleted and modified changes as a table:
```shell
diff {{file1}} {{file2}} | diffstat -t
```
{% endraw %}