---
layout: default
title: "leave"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="leave">
  <a href="/en/common/leave.html">leave</a> <a href="#leave"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remind when it's time to leave.
> To remove reminders use `kill $(pidof leave)`.

#### Set a reminder at a given time:
```shell
leave {{time_to_leave}}
```
#### Remind to leave at noon:
```shell
leave {{1200}}
```
#### Set a reminder in a specific amount of time:
```shell
leave +{{amount_of_time}}
```
#### Remind to leave in 4 hours and 4 minutes:
```shell
leave +{{0404}}
```
{% endraw %}