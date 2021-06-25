---
layout: default
title: "rspamc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rspamc">
  <a href="/en/linux/rspamc.html">rspamc</a> <a href="#rspamc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line client for rspamd servers.

#### Train the bayesian filter to recognise an email as spam:
```shell
rspamc learn_spam {{path/to/email_file}}
```
#### Train the bayesian filter to recognise an email as ham:
```shell
rspamc learn_ham {{path/to/email_file}}
```
#### Generate a manual report on an email:
```shell
rspamc symbols {{path/to/email_file}}
```
#### Show server statistics:
```shell
rspamc stat
```
{% endraw %}