---
layout: default
title: "logwatch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="logwatch">
  <a href="/en/linux/logwatch.html">logwatch</a> <a href="#logwatch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Summarizes many different logs for common services (e.g., apache, pam_unix, sshd, etc.) in a single report.

#### Analyze logs for a range of dates at certain level of detail:
```shell
logwatch --range {{yesterday|today|all|help}} --detail {{low|medium|others}}'
```
#### Restrict report to only include information for a selected service:
```shell
logwatch --range {{all}} --service {{apache|pam_unix|etc}}
```
{% endraw %}