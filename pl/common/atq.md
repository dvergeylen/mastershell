---
layout: default
title: "atq"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="atq">
  <a href="/pl/common/atq.html">atq</a> <a href="#atq"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pokaż oczekujące zadania użytkownika wprowadzone wcześniej przez polecenia `at` lub `batch`.
> Więcej informacji: <https://man.archlinux.org/man/at.1>.

#### Pokaż zaplanowane zadania:
```shell
atq
```
#### Pokaż zadania z kolejki oznaczonej 'a' (kolejki mają jednoznakowe identyfikatory):
```shell
atq -q {{a}}
```
#### Pokaż zadania wszystkich użytkowników (uruchom jako superużytkownik):
```shell
sudo atq
```
{% endraw %}