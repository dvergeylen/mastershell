---
layout: default
title: "yesod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="yesod">
  <a href="/en/common/yesod.html">yesod</a> <a href="#yesod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Helper tool for Yesod, a Haskell-based web framework.
> All Yesod commands are invoked through the `stack` project manager.
> More information: <https://github.com/yesodweb/yesod>.

#### Create a new scaffolded site, with sqlite as backend, in the `my-project` directory:
```shell
stack new {{my-project}} {{yesod-sqlite}}
```
#### Install the Yesod CLI tool within a Yesod scaffolded site:
```shell
stack build yesod-bin cabal-install --install-ghc
```
#### Start development server:
```shell
stack exec -- yesod devel
```
#### Touch files with altered Template Haskell dependencies:
```shell
stack exec -- yesod touch
```
#### Deploy application using Keter (Yesod's deployment manager):
```shell
stack exec -- yesod keter
```
{% endraw %}