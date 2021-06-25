---
layout: default
title: "apache2ctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apache2ctl">
  <a href="/en/linux/apache2ctl.html">apache2ctl</a> <a href="#apache2ctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The CLI tool to administrate HTTP web server Apache.
> This command comes with Debian based OSes, for RHEL based ones see `httpd`.
> More information: <https://manpages.debian.org/latest/apache2/apache2ctl.8.en.html>.

#### Start the Apache daemon. Throw a message if it is already running:
```shell
sudo apache2ctl start
```
#### Stop the Apache daemon:
```shell
sudo apache2ctl stop
```
#### Restart the Apache daemon:
```shell
sudo apache2ctl restart
```
#### Test syntax of the configuration file:
```shell
sudo apache2ctl -t
```
#### List loaded modules:
```shell
sudo apache2ctl -M
```
{% endraw %}