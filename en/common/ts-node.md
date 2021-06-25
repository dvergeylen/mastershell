---
layout: default
title: "ts-node"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ts-node">
  <a href="/en/common/ts-node.html">ts-node</a> <a href="#ts-node"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run TypeScript code directly, without any compiling.
> More information: <https://www.npmjs.com/package/ts-node>.

#### Execute a TypeScript file without compiling (`node` + `tsc`):
```shell
ts-node {{path/to/file.ts}}
```
#### Execute a TypeScript file without loading `tsconfig.json`:
```shell
ts-node --skip-project {{path/to/file.ts}}
```
#### Evaluate TypeScript code passed as a literal on the command-line:
```shell
ts-node --eval '{{console.log("Hello World")}}'
```
#### Execute a TypeScript file in script mode:
```shell
ts-node --script-mode {{path/to/file.ts}}
```
#### Transpile a TypeScript file to JavaScript without executing it:
```shell
ts-node --transpile-only {{path/to/file.ts}}
```
#### Display TS-Node help:
```shell
ts-node --help
```
{% endraw %}