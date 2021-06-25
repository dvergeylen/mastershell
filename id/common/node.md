---
layout: default
title: "node"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="node">
  <a href="/id/common/node.html">node</a> <a href="#node"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Platform JavaScript sisi server (Node.js).
> Informasi lebih lanjut: <https://nodejs.org>.

#### Menjalankan berkas JavaScript:
```shell
node {{alamat/ke/berkas}}
```
#### Memulai sebuah REPL (shell interaktif):
```shell
node
```
#### Mengevaluasi kode JavaScript dengan memberikanya sebagai sebuah argument:
```shell
node -e "{{kode}}"
```
#### Mengevaluasi dan mencetak hasil, berguna untuk melihat versi dependesni node:
```shell
node -p "{{process.versions}}"
```
#### Mengaktifkan inspector, menjeda eksekusi sampai debugger terhubung segera setelah kode sumber sepenuhnya terparser:
```shell
node --no-lazy --inspect-brk {{alamat/ke/berkas}}
```
{% endraw %}