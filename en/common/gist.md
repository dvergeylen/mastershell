---
layout: default
title: "gist"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gist">
  <a href="/en/common/gist.html">gist</a> <a href="#gist"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Upload code to https://gist.github.com.
> More information: <https://github.com/defunkt/gist>.

#### Log in in gist on this computer:
```shell
gist --login
```
#### Create a gist from any number of text files:
```shell
gist {{file.txt}} {{file2.txt}}
```
#### Create a private gist with a description:
```shell
gist --private --description "{{A meaningful description}}" {{file.txt}} 
```
#### Read contents from stdin and create a gist from it:
```shell
{{echo "hello world"}} | gist
```
#### List your public and private gists:
```shell
gist --list
```
#### List all public gists for any user:
```shell
gist --list {{username}}
```
#### Update a gist using the id from URL:
```shell
gist --update {{GIST_ID}} {{file.txt}}
```
{% endraw %}