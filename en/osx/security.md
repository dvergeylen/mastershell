---
layout: default
title: "security"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="security">
  <a href="/en/osx/security.html">security</a> <a href="#security"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Administer Keychains, keys, certificates and the Security framework.
> More information: <https://ss64.com/osx/security.html>.

#### List the available keychains:
```shell
security list-keychains
```
#### Delete a specific keychain:
```shell
security delete-keychain {{path}}
```
#### Create a keychain:
```shell
security create-keychain -p {{password}} {{name.keychain}}
```
{% endraw %}