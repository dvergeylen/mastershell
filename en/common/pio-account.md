---
layout: default
title: "pio account"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pio-account">
  <a href="/en/common/pio-account.html">pio account</a> <a href="#pio-account"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage your PlatformIO account in the command-line.
> More information: <https://docs.platformio.org/en/latest/core/userguide/account/>.

#### Register a new PlatformIO account:
```shell
pio account register --username {{username}} --email {{email}} --password {{password}} --firstname {{firstname}} --lastname {{lastname}}
```
#### Permanently delete your PlatformIO account and related data:
```shell
pio account destroy
```
#### Log in to your PlatformIO account:
```shell
pio account login --username {{username}} --password {{password}}
```
#### Log out of your PlatformIO account:
```shell
pio account logout
```
#### Update your PlatformIO profile:
```shell
pio account update --username {{username}} --email {{email}} --firstname {{firstname}} --lastname {{lastname}} --current-password {{password}}
```
#### Show detailed information about your PlatformIO account:
```shell
pio account show
```
#### Reset your password using your username or email:
```shell
pio account forgot --username {{username_or_email}}
```
{% endraw %}