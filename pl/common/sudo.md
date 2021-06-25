---
layout: default
title: "sudo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sudo">
  <a href="/pl/common/sudo.html">sudo</a> <a href="#sudo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wykonuje pojedyncze polecenie jako superuser lub inny użytkownik.

#### Uruchom polecenie jako superuser:
```shell
sudo {{less /var/log/syslog}}
```
#### Edytuj plik jako superuser w domyślnym edytorze:
```shell
sudo -e {{/etc/fstab}}
```
#### Uruchom polecenie jako inny użytkownik i/lub grupa:
```shell
sudo -u {{uzytkownik}} -g {{grupa}} {{id -a}}
```
#### Powtórz ostatnie polecenie poprzedzone `sudo` (tylko w `bash`, `zsh`, etc.):
```shell
sudo !!
```
#### Uruchom domyślną powłokę z uprawnieniami superuser:
```shell
sudo -i
```
{% endraw %}