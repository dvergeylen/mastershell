---
layout: default
title: "r2e"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="r2e">
  <a href="/en/common/r2e.html">r2e</a> <a href="#r2e"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Forwards RSS feeds to an email address.
> Requires a configured `sendmail` or smtp setup.
> More information: <https://github.com/rss2email/rss2email>.

#### Create a new feed database that sends email to an email address:
```shell
r2e new {{email_address}}
```
#### Subscribe to a feed:
```shell
r2e add {{feed_name}} {{feed_URI}}
```
#### Send new stories to an email address:
```shell
r2e run
```
#### List all feeds:
```shell
r2e list
```
#### Delete a feed at a specified index:
```shell
r2e delete {{index}}
```
{% endraw %}