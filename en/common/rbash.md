---
layout: default
title: "rbash"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rbash">
  <a href="/en/common/rbash.html">rbash</a> <a href="#rbash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Restricted Bash shell, equivalent to `bash --restricted`.
> Does not permit changing the working directory, redirecting command output, or modifying environment variables, among other things.
> See also `histexpand` for history expansion.
> More information: <https://www.gnu.org/software/bash/manual/html_node/The-Restricted-Shell>.

#### Start an interactive shell session:
```shell
rbash
```
#### Execute a command and then exit:
```shell
rbash -c "{{command}}"
```
#### Execute a script:
```shell
rbash {{path/to/script.sh}}
```
#### Execute a script, printing each command before executing it:
```shell
rbash -x {{path/to/script.sh}}
```
#### Execute commands from a script, stopping at the first error:
```shell
rbash -e {{path/to/script.sh}}
```
#### Read and execute commands from stdin:
```shell
rbash -s
```
{% endraw %}