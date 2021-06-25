---
layout: default
title: "bash"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bash">
  <a href="/en/common/bash.html">bash</a> <a href="#bash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bourne-Again SHell, an `sh`-compatible command-line interpreter.
> See also `histexpand` for history expansion.
> More information: <https://gnu.org/software/bash/>.

#### Start an interactive shell session:
```shell
bash
```
#### Execute a command and then exit:
```shell
bash -c "{{command}}"
```
#### Execute a script:
```shell
bash {{path/to/script.sh}}
```
#### Execute a script, printing each command before executing it:
```shell
bash -x {{path/to/script.sh}}
```
#### Execute commands from a script, stopping at the first error:
```shell
bash -e {{path/to/script.sh}}
```
#### Read and execute commands from stdin:
```shell
bash -s
```
#### Print the Bash version (`$BASH_VERSION` contains the version without license information):
```shell
bash --version
```
{% endraw %}