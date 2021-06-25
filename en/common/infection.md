---
layout: default
title: "infection"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="infection">
  <a href="/en/common/infection.html">infection</a> <a href="#infection"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A mutation testing framework for PHP.
> More information: <https://infection.github.io>.

#### Analyse code using the configuration file (or create one if it does not exist):
```shell
infection
```
#### Use a specific number of threads:
```shell
infection --threads {{number_of_threads}}
```
#### Specify a minimum Mutation Score Indicator (MSI):
```shell
infection --min-msi {{percentage}}
```
#### Specify a minimum covered code MSI:
```shell
infection --min-covered-msi {{percentage}}
```
#### Use a specific test framework (defaults to phpunit):
```shell
infection --test-framework {{phpunit|phpspec}}
```
#### Only mutate lines of code that are covered by tests:
```shell
infection --only-covered
```
#### Display the mutation code that has been applied:
```shell
infection --show-mutations
```
#### Specify the log verbosity:
```shell
infection --log-verbosity {{default|all|none}}
```
{% endraw %}