---
layout: default
title: "erl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="erl">
  <a href="/en/common/erl.html">erl</a> <a href="#erl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run and manage programs in the Erlang programming language.
> More information: <https://www.erlang.org>.

#### Compile and run sequential Erlang program as a common script and then exit:
```shell
erlc {{files}} && erl -noshell '{{mymodule:myfunction(arguments)}}, init:stop().'
```
#### Connect to a running Erlang node:
```shell
erl -remsh {{nodename}}@{{hostname}} -sname {{custom_shortname}} -hidden -setcookie {{cookie_of_remote_node}}
```
#### Tell the Erlang shell to load modules from a directory:
```shell
erl -pa {{directory_with_beam_files}}
```
{% endraw %}