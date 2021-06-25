---
layout: default
title: "xkcdpass"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xkcdpass">
  <a href="/pl/common/xkcdpass.html">xkcdpass</a> <a href="#xkcdpass"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Konfigurowalny generator haseł tworzący mocne hasła.
> Zainspirowane przez XKCD 936.
> Więcej informacji: <https://github.com/redacted/XKCD-password-generator>.

#### Stwórz hasło z domyślną konfiguracją:
```shell
xkcdpass
```
#### Stwórz hasło w którym pierwsze litery każdego słowa układają się w podany argument:
```shell
xkcdpass -a {{acrostic}}
```
#### Interaktywnie stwórz hasło:
```shell
xkcdpass -i
```
{% endraw %}