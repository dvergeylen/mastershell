---
layout: default
title: "nologin"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nologin">
  <a href="/en/linux/nologin.html">nologin</a> <a href="#nologin"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Alternative shell that prevents a user from logging in.

#### Set a user's login shell to `nologin` to prevent the user from logging in:
```shell
chsh -s {{user}} nologin
```
#### Customize message for users with the login shell of `nologin`:
```shell
echo "{{declined_login_message}}" > /etc/nologin.txt
```
{% endraw %}