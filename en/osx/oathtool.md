---
layout: default
title: "oathtool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="oathtool">
  <a href="/en/osx/oathtool.html">oathtool</a> <a href="#oathtool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> OATH one-time password tool.

#### Generate TOTP token (behaves like Google Authenticator):
```shell
oathtool --totp --base32 {{secret}}
```
#### Generate a TOTP token for a specific time:
```shell
oathtool --totp --now {{2004-02-29 16:21:42}} --base32 {{secret}}
```
#### Validate a TOTP token:
```shell
oathtool --totp --base32 {{secret}} {{token}}
```
{% endraw %}