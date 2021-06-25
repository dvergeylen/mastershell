---
layout: default
title: "reg compare"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg-compare">
  <a href="/en/windows/reg-compare.html">reg compare</a> <a href="#reg-compare"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compare keys and their values in the registry.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-compare>.

#### Compare all values under a specific key with a second key:
```shell
reg compare {{first_key_name}} {{second_key_name}}
```
#### Compare a specific value under two keys:
```shell
reg compare {{first_key_name}} {{second_key_name}} /v {{value}}
```
#### Compare all sub keys and values for two keys:
```shell
reg compare {{first_key_name}} {{second_key_name}} /s
```
#### Only output the matches between the specified keys:
```shell
reg compare {{first_key_name}} {{second_key_name}} /os
```
#### Output the differences and matches between the specified keys:
```shell
reg compare {{first_key_name}} {{second_key_name}} /oa
```
{% endraw %}