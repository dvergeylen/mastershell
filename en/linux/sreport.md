---
layout: default
title: "sreport"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sreport">
  <a href="/en/linux/sreport.html">sreport</a> <a href="#sreport"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate reports on jobs, users, and clusters from accounting data.
> More information: <https://slurm.schedmd.com/sreport.html>.

#### Show pipe delimited cluster utilization data:
```shell
sreport --parsable cluster utilization
```
#### Show number of jobs run:
```shell
sreport job sizes printjobcount
```
#### Show users with highest cpu time use:
```shell
sreport user topuser
```
{% endraw %}