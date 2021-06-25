---
layout: default
title: "defaults"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="defaults">
  <a href="/en/osx/defaults.html">defaults</a> <a href="#defaults"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Read and write macOS user configuration for applications.
> More information: <https://ss64.com/osx/defaults.html>.

#### Read system defaults for an application option:
```shell
defaults read {{application}} {{option}}
```
#### Read default values for an application option:
```shell
defaults read -app {{application}} {{option}}
```
#### Search for a keyword in domain names, keys, and values:
```shell
defaults find {{keyword}}
```
#### Write the default value of an application option:
```shell
defaults write {{application}} {{option}} {{-type}} {{value}}
```
#### Speed up Mission Control animations:
```shell
defaults write com.apple.Dock expose-animation-duration -float 0.1
```
#### Delete all defaults of an application:
```shell
defaults delete {{application}}
```
{% endraw %}