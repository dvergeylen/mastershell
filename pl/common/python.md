---
layout: default
title: "python"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="python">
  <a href="/pl/common/python.html">python</a> <a href="#python"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interpreter języka Python.
> Więcej informacji: <https://www.python.org>.

#### Wywołaj interaktywną powłokę Pythona (REPL):
```shell
python
```
#### Wykonaj skrypt w danym pliku Python:
```shell
python {{skrypt.py}}
```
#### Wykonaj skrypt jako część interaktywnej powłoki:
```shell
python -i {{skrypt.py}}
```
#### Wykonaj wyrażenie w języku Python:
```shell
python -c "{{wyrazenie}}"
```
#### Uruchom moduł biblioteki jako skrypt (kończy listę opcji):
```shell
python -m {{moduł}} {{argumenty}}
```
#### Interaktywnie debuguj skrypt w języku Python:
```shell
python -m pdb {{skrypt.py}}
```
{% endraw %}