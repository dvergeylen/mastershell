---
layout: default
title: "faketime"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="faketime">
  <a href="/en/linux/faketime.html">faketime</a> <a href="#faketime"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fake the system time for a given command.
> More information: <https://manpages.ubuntu.com/manpages/trusty/man1/faketime.1.html>.

#### Fake the time to this evening, before printing the result of `date`:
```shell
faketime '{{today 23:30}}' {{date}}
```
#### Open a new `bash` shell, which uses yesterday as the current date:
```shell
faketime '{{yesterday}}' {{bash}}
```
#### Simulate how any program would act next friday night:
```shell
faketime '{{next Friday 1 am}}' {{path/to/any/program}}
```
{% endraw %}