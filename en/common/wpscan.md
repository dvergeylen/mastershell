---
layout: default
title: "wpscan"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wpscan">
  <a href="/en/common/wpscan.html">wpscan</a> <a href="#wpscan"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> WordPress vulnerability scanner.
> More information: <https://github.com/wpscanteam/wpscan>.

#### Update the vulnerability database:
```shell
wpscan --update
```
#### Scan a WordPress website:
```shell
wpscan --url {{url}}
```
#### Scan a WordPress website, using random user agents and passive detection:
```shell
wpscan --url {{url}} --stealthy
```
#### Scan a WordPress website, checking for vulnerable plugins and specifying the path to the `wp-content` directory:
```shell
wpscan --url {{url}} --enumerate {{vp}} --wp-content-dir {{remote/path/to/wp-content}}
```
#### Scan a WordPress website through a proxy:
```shell
wpscan --url {{url}} --proxy {{protocol://ip:port}} --proxy-auth {{username:password}}
```
#### Perform user identifiers enumeration on a WordPress website:
```shell
wpscan --url {{url}} --enumerate {{u}}
```
#### Execute a password guessing attack on a WordPress website:
```shell
wpscan --url {{url}} --usernames {{username|path/to/usernames.txt}} --passwords {{path/to/passwords.txt}} threads {{20}}
```
#### Scan a WordPress website, collecting vulnerability data from the WPVulnDB (https://wpvulndb.com/):
```shell
wpscan --url {{url}} --api-token {{token}}
```
{% endraw %}