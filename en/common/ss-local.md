---
layout: default
title: "ss-local"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ss-local">
  <a href="/en/common/ss-local.html">ss-local</a> <a href="#ss-local"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run a Shadowsocks client as a SOCKS5 proxy.
> More information: <https://github.com/shadowsocks/shadowsocks-libev/blob/master/doc/ss-local.asciidoc>.

#### Run a Shadowsocks proxy by specifying the host, server port, local port, password, and encryption method:
```shell
ss-local -s {{host}} -p {{server_port}} -l {{local port}} -k {{password}} -m {{encrypt_method}}
```
#### Run a Shadowsocks proxy by specifying the config file:
```shell
ss-local -c {{path/to/config/file.json}}
```
#### Use a plugin to run the proxy client:
```shell
ss-local --plugin {{plugin_name}} --plugin-opts {{plugin_options}}
```
#### Enable TCP fast open:
```shell
ss-local --fast-open
```
{% endraw %}