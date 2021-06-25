---
layout: default
title: "timew"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="timew">
  <a href="/en/common/timew.html">timew</a> <a href="#timew"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A time tracking tool used to measure the duration of activities.
> More information: <https://taskwarrior.org/docs/timewarrior>.

#### Start a new stopwatch, giving a tag name to the activity being tracked:
```shell
timew start {{activity_tag}}
```
#### View running stopwatches:
```shell
timew
```
#### Stop the stopwatch with a given tag name:
```shell
timew stop {{activity_tag}}
```
#### Stop all running stopwatches:
```shell
timew stop
```
#### View tracked items:
```shell
timew summary
```
{% endraw %}