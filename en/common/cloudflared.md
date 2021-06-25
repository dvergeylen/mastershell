---
layout: default
title: "cloudflared"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cloudflared">
  <a href="/en/common/cloudflared.html">cloudflared</a> <a href="#cloudflared"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line tool to create a persistent connection to the Cloudflare network.
> More information: <https://developers.cloudflare.com/argo-tunnel/>.

#### Authenticate and associate the connection to a domain in the Cloudflare account:
```shell
cloudflared tunnel login
```
#### Establish a tunnel to a host in Cloudflare from the local server:
```shell
cloudflared tunnel --hostname {{hostname}} localhost:{{port_number}}
```
#### Establish a tunnel to a host in Cloudflare from the local server, without verifying the local server's certificate:
```shell
cloudflared tunnel --hostname {{hostname}} localhost:{{port_number}} --no-tls-verify
```
#### Save logs to a file:
```shell
cloudflared tunnel --hostname {{hostname}} http://localhost:{{port_number}} --loglevel {{panic|fatal|error|warn|info|debug}} --logfile {{path/to/file}}
```
#### Install cloudflared as a system service:
```shell
cloudflared service install
```
{% endraw %}