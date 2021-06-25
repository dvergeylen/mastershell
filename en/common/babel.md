---
layout: default
title: "babel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="babel">
  <a href="/en/common/babel.html">babel</a> <a href="#babel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A transpiler which converts code from JavaScript ES6/ES7 syntax to ES5 syntax.
> More information: <https://babeljs.io/>.

#### Transpile a specified input file and output to stdout:
```shell
babel {{path/to/file}}
```
#### Transpile a specified input file and output to a specific file:
```shell
babel {{path/to/input_file}} --out-file {{path/to/output_file}}
```
#### Transpile the input file every time it is changed:
```shell
babel {{path/to/input_file}} --watch
```
#### Transpile a whole directory of files:
```shell
babel {{path/to/input_directory}}
```
#### Ignore specified comma-separated files in a directory:
```shell
babel {{path/to/input_directory}} --ignore {{ignored_files}}
```
#### Transpile and output as minified JavaScript:
```shell
babel {{path/to/input_file}} --minified
```
#### Choose a set of presets for output formatting:
```shell
babel {{path/to/input_file}} --presets {{presets}}
```
#### Output all available options:
```shell
babel --help
```
{% endraw %}