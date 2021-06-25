---
layout: default
title: "python"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="python">
  <a href="/id/common/python.html">python</a> <a href="#python"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Penerjemah bahasa Python.
> Informasi lebih lanjut: <https://www.python.org>.

#### Menjalankan REPL (shell interaktif):
```shell
python
```
#### Menjalankan skrip pada berkas Python:
```shell
python {{skrip.py}}
```
#### Menjalankan skrip sebagai bagian dari shell interaktif:
```shell
python -i {{skrip.py}}
```
#### Menjalankan ekspresi Python:
```shell
python -c "{{ekspresi}}"
```
#### Menjalankan modul perpustakaan sebagai skrip (diakhiri dengan daftar opsi):
```shell
python -m {{modul}} {{argumen}}
```
#### Mendebug skrip Python secara interaktif:
```shell
python -m pdb {{script.py}}
```
{% endraw %}