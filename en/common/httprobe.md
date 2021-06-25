---
layout: default
title: "httprobe"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="httprobe">
  <a href="/en/common/httprobe.html">httprobe</a> <a href="#httprobe"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Take a list of domains and probe for working HTTP and HTTPS servers.
> More information: <https://github.com/tomnomnom/httprobe>.

#### Probe a list of domains from a text file:
```shell
cat {{input_file}} | httprobe
```
#### Only check for HTTP if HTTPS is not working:
```shell
cat {{input_file}} | httprobe --prefer-https
```
#### Probe additional ports with a given protocol:
```shell
cat {{input_file}} | httprobe -p {{https:2222}}
```
#### Output all available options:
```shell
httprobe --help
```
{% endraw %}