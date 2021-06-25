---
layout: default
title: "powerstat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="powerstat">
  <a href="/en/common/powerstat.html">powerstat</a> <a href="#powerstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Measures the power consumption of a computer that has a battery power source or supports the RAPL interface.
> More information: <http://manpages.ubuntu.com/manpages/bionic/man8/powerstat.8.html>.

#### Measure power with the default of 10 samples with an interval of 10 seconds:
```shell
powerstat
```
#### Measure power with custom number of samples and interval duration:
```shell
powerstat {{interval}} {{number_of_samples}}
```
#### Measure power using Intel's RAPL interface:
```shell
powerstat -R {{interval}} {{number_of_samples}}
```
#### Show an histogram of the power measurements:
```shell
powerstat -H {{interval}} {{number_of_samples}}
```
#### Enable all statistics gathering options:
```shell
powerstat -a {{interval}} {{number_of_samples}}
```
{% endraw %}