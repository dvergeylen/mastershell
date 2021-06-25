---
layout: default
title: "deluged"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="deluged">
  <a href="/en/common/deluged.html">deluged</a> <a href="#deluged"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A daemon process for the Deluge BitTorrent client.
> More information: <https://deluge-torrent.org>.

#### Start the Deluge daemon:
```shell
deluged
```
#### Start the Deluge daemon on a specific port:
```shell
deluged -p {{port}}
```
#### Start the Deluge daemon using a specific configuration file:
```shell
deluged -c {{path/to/configuration_file}}
```
#### Start the Deluge daemon and output the log to a file:
```shell
deluged -l {{path/to/log_file}}
```
{% endraw %}