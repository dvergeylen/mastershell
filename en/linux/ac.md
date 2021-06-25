---
layout: default
title: "ac"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ac">
  <a href="/en/linux/ac.html">ac</a> <a href="#ac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print statistics on how long users have been connected.

#### Print how long the current user has been connected in hours:
```shell
ac
```
#### Print how long users have been connected in hours:
```shell
ac --individual-totals
```
#### Print how long a particular user has been connected in hours:
```shell
ac --individual-totals {{username}}
```
#### Print how long a particular user has been connected in hours per day (with total):
```shell
ac --daily-totals --individual-totals {{username}}
```
#### Also display additional details:
```shell
ac --compatibility
```
{% endraw %}