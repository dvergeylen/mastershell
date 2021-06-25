---
layout: default
title: "micro"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="micro">
  <a href="/ru/common/micro.html">micro</a> <a href="#micro"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Micro - это современный и интуитивно понятный консольный текстовый редактор.
> Micro поддерживает клавиатуру и мышь для навигации и/или выделения текста.
> Больше информации: <https://micro-editor.github.io>.

#### Открыть файл:
```shell
micro {{файл}}
```
#### Вырезать всю строку:
```shell
Ctrl + K
```
#### Искать в файле (используйте `Ctrl + N`/`Ctrl + P` чтобы перейти к следующему/предыдущему совпадению):
```shell
Ctrl + F "{{паттерн}}" <Ввод>
```
#### Выполнить команду:
```shell
Ctrl + E {{команда}} <Ввод>
```
#### Выполнить замену во всем файле:
```shell
Ctrl + E replaceall "{{строка}}" "{{замена}}" <Ввод>
```
#### Выход:
```shell
Ctrl + Q
```
{% endraw %}