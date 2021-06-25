---
layout: default
title: "speedometer"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="speedometer">
  <a href="/en/linux/speedometer.html">speedometer</a> <a href="#speedometer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Python script that shows a network traffic graph in the terminal.
> More information: <http://excess.org/speedometer>.

#### Show graph for a specific interface:
```shell
speedometer -r {{eth0}} -t {{eth0}}
```
{% endraw %}