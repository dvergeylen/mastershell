---
layout: default
title: "firebase"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="firebase">
  <a href="/en/common/firebase.html">firebase</a> <a href="#firebase"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Test, manage, and deploy Firebase projects from the command-line.
> More information: <https://github.com/firebase/firebase-tools>.

#### Log in to <https://console.firebase.google.com>:
```shell
firebase login
```
#### List existing Firebase projects:
```shell
firebase projects:list
```
#### Start an interactive wizard to create a Firebase project in the current directory:
```shell
firebase init
```
#### Deploy code and assets to the current Firebase project:
```shell
firebase deploy
```
#### Start a local server to statically host the current Firebase project's assets:
```shell
firebase serve
```
#### Start an interactive wizard to open one of many links of the current Firebase project in the default web browser:
```shell
firebase open
```
{% endraw %}