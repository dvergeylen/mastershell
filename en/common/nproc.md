---
layout: default
title: "nproc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nproc">
  <a href="/en/common/nproc.html">nproc</a> <a href="#nproc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print the number of processing units (normally CPUs) available.
> More information: <https://www.gnu.org/software/coreutils/nproc>.

#### Display the number of available processing units:
```shell
nproc
```
#### Display the number of installed processing units, including any inactive ones:
```shell
nproc --all
```
#### If possible, subtract a given number of units from the returned value:
```shell
nproc --ignore {{count}}
```
{% endraw %}