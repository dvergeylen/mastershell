---
layout: default
title: "apt-key"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-key">
  <a href="/en/linux/apt-key.html">apt-key</a> <a href="#apt-key"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Key management utility for the APT Package Manager on Debian and Ubuntu.
> Note: `apt-key` is now deprecated (except for the use of `apt-key del` in maintainer scripts).
> More information: <https://manpages.debian.org/latest/apt/apt-key.8.html>.

#### List trusted keys:
```shell
apt-key list
```
#### Add a key to the trusted keystore:
```shell
apt-key add {{public_key_file.asc}}
```
#### Delete a key from the trusted keystore:
```shell
apt-key del {{key_id}}
```
#### Add a remote key to the trusted keystore:
```shell
wget -qO - {{https://host.tld/filename.key}} | apt-key add -
```
#### Add a key from keyserver with only key id:
```shell
apt-key adv --keyserver {{pgp.mit.edu}} --recv {{KEYID}}
```
{% endraw %}