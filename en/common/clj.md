---
layout: default
title: "clj"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="clj">
  <a href="/en/common/clj.html">clj</a> <a href="#clj"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Clojure tool to start a REPL or invoke a specific function with data.
> All options can be defined in a `deps.edn` file.
> More information: <https://clojure.org/guides/deps_and_cli>.

#### Start a REPL:
```shell
clj
```
#### Execute a function:
```shell
clj -X {{namespace/function_name}}
```
#### Run the main function of a specified namespace:
```shell
clj -M -m {{namespace}} {{args}}
```
#### Prepare a project by resolving dependencies, downloading libraries, and making / caching classpaths:
```shell
clj -P
```
#### Start an nREPL server with the CIDER middleware:
```shell
clj -Sdeps '{:deps {nrepl {:mvn/version "0.7.0"} cider/cider-nrepl {:mvn/version "0.25.2"}}}' -m nrepl.cmdline --middleware '["cider.nrepl/cider-middleware"]' --interactive
```
#### Start a REPL for ClojureScript and open a web browser:
```shell
clj -Sdeps '{:deps {org.clojure/clojurescript {:mvn/version "1.10.758"}}}' --main cljs.main --repl
```
{% endraw %}