---
layout: default
title: "hyperfine"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hyperfine">
  <a href="/en/common/hyperfine.html">hyperfine</a> <a href="#hyperfine"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line benchmarking tool.
> More information: <https://github.com/sharkdp/hyperfine/>.

#### Run a basic benchmark, performing at least 10 runs:
```shell
hyperfine '{{make}}'
```
#### Run a comparative benchmark:
```shell
hyperfine '{{make target1}}' '{{make target2}}'
```
#### Change minimum number of benchmarking runs:
```shell
hyperfine --min-runs {{7}} '{{make}}'
```
#### Perform benchmark with warmup:
```shell
hyperfine --warmup {{5}} '{{make}}'
```
#### Run a command before each benchmark run (to clear caches, etc.):
```shell
hyperfine --prepare '{{make clean}}' '{{make}}'
```
#### Run a benchmark where a single parameter changes for each run:
```shell
hyperfine --prepare '{{make clean}}' --parameter-scan {{num_threads}} {{1}} {{10}} '{{make -j {num_threads}}}'
```
{% endraw %}