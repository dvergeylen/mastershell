---
layout: default
title: "cpdf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cpdf">
  <a href="/en/common/cpdf.html">cpdf</a> <a href="#cpdf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI to manipulate existing PDF files in a variety of ways.
> More information: <https://www.coherentpdf.com/cpdfmanual/cpdfmanual.html>.

#### Select pages 1, 2, 3 and 6 from a source document and write those to a destination document:
```shell
cpdf {{path/to/source_document.pdf}} {{1-3,6}} -o {{path/to/destination_document.pdf}}
```
#### Merge two documents into a new one:
```shell
cpdf -merge {{path/to/source_document_one.pdf}} {{path/to/source_document_two.pdf}} -o {{path/to/destination_document.pdf}}
```
#### Show the bookmarks of a document:
```shell
cpdf -list-bookmarks {{path/to/document.pdf}}
```
#### Split a document into ten-page chunks, writing them to `chunk001.pdf`, `chunk002.pdf`, etc:
```shell
cpdf -split {{path/to/document.pdf}} -o {{path/to/chunk%%%.pdf}} -chunk {{10}}
```
#### Encrypt a document using 128bit encryption, providing `fred` as owner password and `joe` as user password:
```shell
cpdf -encrypt {{128bit}} {{fred}} {{joe}} {{path/to/source_document.pdf}} -o {{path/to/encrypted_document.pdf}}
```
#### Decrypt a document using the owner password `fred`:
```shell
cpdf -decrypt {{path/to/encrypted_document.pdf}} owner={{fred}} -o {{path/to/decrypted_document.pdf}}
```
#### Show the annotations of a document:
```shell
cpdf -list-annotations {{path/to/document.pdf}}
```
#### Create a new document from an existing one with additional metadata:
```shell
cpdf -set-metadata {{path/to/metadata.xml}} {{path/to/source_document.pdf}} -o {{path/to/destination_document.pdf}}
```
{% endraw %}