---
layout: default
title: "envsubst"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="envsubst">
  <a href="/en/common/envsubst.html">envsubst</a> <a href="#envsubst"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Substitutes environment variables with their value in shell format strings.
> Variables to be replaced should be in either `${var}` or `$var` format.
> More information: <https://www.gnu.org/software/gettext/manual/html_node/envsubst-Invocation.html>.

#### Replace environment variables in stdin and output to stdout:
```shell
echo '{{$HOME}}' | envsubst
```
#### Replace environment variables in an input file and output to stdout:
```shell
envsubst < {{path/to/input_file}}
```
#### Replace environment variables in an input file and output to a file:
```shell
envsubst < {{path/to/input_file}} > {{path/to/output_file}}
```
#### Replace environment variables in an input file from a space-separated list:
```shell
envsubst '{{$USER $SHELL $HOME}}' < {{path/to/input_file}}
```
{% endraw %}