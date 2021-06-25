---
layout: default
title: "clj"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="clj">
  <a href="/pt_br/common/clj.html">clj</a> <a href="#clj"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta de Clojure para iniciar um REPL ou invocar uma função com argumentos.
> Todas as opções podem ser definidas em um arquivo `deps.edn`.
> Mais informações: <https://clojure.org/guides/deps_and_cli>.

#### Inicia um REPL:
```shell
clj
```
#### Executa uma função:
```shell
clj -X {{namespace/function_name}}
```
#### Executa a função principal (*main*) do *namespace* especificado:
```shell
clj -M -m {{namespace}} {{args}}
```
#### Prepara um projeto resolvendo dependências, baixando bibliotecas, e criando / cacheando *classpaths*:
```shell
clj -P
```
#### Inicia um servidor nREPL com o *middleware* CIDER:
```shell
clj -Sdeps '{:deps {nrepl {:mvn/version "0.7.0"} cider/cider-nrepl {:mvn/version "0.25.2"}}}' -m nrepl.cmdline --middleware '["cider.nrepl/cider-middleware"]' --interactive
```
#### Inicia um REPL para ClojureScript e abre um navegador web:
```shell
clj -Sdeps '{:deps {org.clojure/clojurescript {:mvn/version "1.10.758"}}}' --main cljs.main --repl
```
{% endraw %}