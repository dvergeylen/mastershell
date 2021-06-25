---
layout: default
title: "deno"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="deno">
  <a href="/en/common/deno.html">deno</a> <a href="#deno"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A secure runtime for JavaScript and TypeScript.
> More information: <https://deno.land/>.

#### Run a JavaScript or TypeScript file:
```shell
deno run {{path/to/file.ts}}
```
#### Start a REPL (interactive shell):
```shell
deno
```
#### Run a file with network access enabled:
```shell
deno run --allow-net {{path/to/file.ts}}
```
#### Run a file from a URL:
```shell
deno run {{https://deno.land/std/examples/welcome.ts}}
```
#### Install an executable script from a URL:
```shell
deno install {{https://deno.land/std/examples/colors.ts}}
```
{% endraw %}