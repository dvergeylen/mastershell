---
layout: default
title: "bundle"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bundle">
  <a href="/en/common/bundle.html">bundle</a> <a href="#bundle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Dependency manager for the Ruby programming language.
> More information: <https://bundler.io/man/bundle.1.html>.

#### Install all gems defined in the `Gemfile` expected in the working directory:
```shell
bundle install
```
#### Execute a command in the context of the current bundle:
```shell
bundle exec {{command}} {{arguments}}
```
#### Update all gems by the rules defined in the `Gemfile` and regenerate `Gemfile.lock`:
```shell
bundle update
```
#### Update one or more specific gem(s) defined in the `Gemfile`:
```shell
bundle update {{gem_name}} {{gem_name}}
```
#### Update one or more specific gems(s) defined in the `Gemfile` but only to the next patch version:
```shell
bundle update --patch {{gem_name}} {{gem_name}}
```
#### Update all gems within the given group in the `Gemfile`:
```shell
bundle update --group {{development}}
```
#### List installed gems in the `Gemfile` with newer versions available:
```shell
bundle outdated
```
#### Create a new gem skeleton:
```shell
bundle gem {{gem_name}}
```
{% endraw %}