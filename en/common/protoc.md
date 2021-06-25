---
layout: default
title: "protoc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="protoc">
  <a href="/en/common/protoc.html">protoc</a> <a href="#protoc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Parse Google Protobuf `.proto` files and generate output in the specified language.
> More information: <https://developers.google.com/protocol-buffers>.

#### Generate Python code from a `.proto` file:
```shell
protoc --python_out={{path/to/output_directory}} {{input_file.proto}}
```
#### Generate Java code from a `.proto` file that imports other `.proto` files:
```shell
protoc --java_out={{path/to/output_directory}} --proto_path={{path/to/import_search_path}} {{input_file.proto}}
```
#### Generate code for multiple languages:
```shell
protoc --csharp_out={{path/to/c#_output_directory}} --js_out={{path/to/js_output_directory}} {{input_file.proto}}
```
{% endraw %}