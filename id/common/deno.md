---
layout: default
title: "deno"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="deno">
  <a href="/id/common/deno.html">deno</a> <a href="#deno"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Runtime aman untuk JavaScript dan TypeScript.
> Informasi lebih lanjut: <https://deno.land/>.

#### Menjalankan berkas JavaScript atau TypeScript:
```shell
deno run {{alamat/ke/berkas.ts}}
```
#### Menjalankan REPL (shell interaktif):
```shell
deno
```
#### Menjalankan berkas dengan memperbolehkan akses jaringan:
```shell
deno run --allow-net {{alamat/ke/berkas.ts}}
```
#### Menjalankan berkas dari URL:
```shell
deno run {{https://deno.land/std/examples/welcome.ts}}
```
#### Memasang skrip yang dapat dieksekusi dari URL:
```shell
deno install {{https://deno.land/std/examples/colors.ts}}
```
{% endraw %}