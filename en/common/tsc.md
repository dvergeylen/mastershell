---
layout: default
title: "tsc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tsc">
  <a href="/en/common/tsc.html">tsc</a> <a href="#tsc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> TypeScript compiler.
> More information: <https://www.typescriptlang.org/docs/handbook/compiler-options.html>.

#### Compile a TypeScript file `foobar.ts` into a JavaScript file `foobar.js`:
```shell
tsc {{foobar.ts}}
```
#### Compile a TypeScript file into JavaScript using a specific target syntax (default is `ES3`):
```shell
tsc --target {{ES5|ES2015|ES2016|ES2017|ES2018|ESNEXT}} {{foobar.ts}}
```
#### Compile a TypeScript file into a JavaScript file with a custom name:
```shell
tsc --outFile {{output.js}} {{input.ts}}
```
#### Compile all `.ts` files of a TypeScript project defined in a `tsconfig.json` file:
```shell
tsc --build {{tsconfig.json}}
```
#### Run the compiler using command-line options and arguments fetched from a text file:
```shell
tsc @{{args.txt}}
```
#### Type-check multiple JavaScript files, and output only the errors:
```shell
tsc --allowJs --checkJs --noEmit {{src/**/*.js}}
```
{% endraw %}