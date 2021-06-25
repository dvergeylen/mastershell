---
layout: default
title: "csc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csc">
  <a href="/it/common/csc.html">csc</a> <a href="#csc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compilatore per Microsoft C#.
> Maggiori informazioni: <https://docs.microsoft.com/dotnet/csharp/language-reference/compiler-options/command-line-building-with-csc-exe>.

#### Compila uno o più file C# in un eseguibile da command-line:
```shell
csc {{percorso/al/file_input_a.cs}} {{percorso/al/file_input_b.cs}}
```
#### Specifica il nome del file output:
```shell
csc /out:{{percorso/al/nome_file_output}} {{percorso/al/file_input.cs}}
```
#### Compila in una libreria `.dll` invece che in un eseguibile:
```shell
csc /target:library {{percorso/al/file_input.cs}}
```
#### Referenzia un altro assembly:
```shell
csc /reference:{{percorso/a/libreria.dll}} {{percorso/al/file_input.cs}}
```
#### Includi una risorsa:
```shell
csc /resource:{{percorso/al/file_risorsa}} {{percorso/al/file_input.cs}}
```
#### Genera una documentazione XML automaticamente:
```shell
csc /doc:{{percorso/alla/documentazione.xml}} {{percorso/al/file_input.cs}}
```
#### Specifica un'icona:
```shell
csc /win32icon:{{percorso/a/icona.ico}} {{percorso/al/file_input.cs}}
```
#### Firma un assembly con un nome sicuro utilizzando una chiave:
```shell
csc /keyfile:{{percorso/a/chiave.snk}} {{percorso/al/file_input.cs}}
```
{% endraw %}