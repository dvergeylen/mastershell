---
layout: default
title: "postfix"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="postfix">
  <a href="/en/linux/postfix.html">postfix</a> <a href="#postfix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Postfix mail transfer agent (MTA) control program.
> See also `dovecot`, a mail delivery agent (MDA) that integrates with Postfix.
> More information: <http://postfix.org>.

#### Check the configuration:
```shell
sudo postfix check
```
#### Check the status of the Postfix daemon:
```shell
sudo postfix status
```
#### Start Postfix:
```shell
sudo postfix start
```
#### Gracefully stop Postfix:
```shell
sudo postfix stop
```
#### Flush the mail queue:
```shell
sudo postfix flush
```
#### Reload the configuration files:
```shell
sudo postfix reload
```
{% endraw %}