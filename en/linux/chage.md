---
layout: default
title: "chage"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chage">
  <a href="/en/linux/chage.html">chage</a> <a href="#chage"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change user account and password expiry information.

#### List password information for the user:
```shell
chage -l {{username}}
```
#### Enable password expiration in 10 days:
```shell
sudo chage -M {{10}} {{username}}
```
#### Disable password expiration:
```shell
sudo chage -M -1 {{username}}
```
#### Set account expiration date:
```shell
sudo chage -E {{YYYY-MM-DD}}
```
#### Force user to change password on next log in:
```shell
sudo chage -d 0
```
{% endraw %}