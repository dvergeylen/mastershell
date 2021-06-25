---
layout: default
title: "blackfire"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="blackfire">
  <a href="/en/common/blackfire.html">blackfire</a> <a href="#blackfire"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line profiling tool for PHP.
> More information: <https://blackfire.io>.

#### Initialise and configure the Blackfire client:
```shell
blackfire config
```
#### Launch the Blackfire agent:
```shell
blackfire agent
```
#### Launch the Blackfire agent on a specific socket:
```shell
blackfire agent --socket="{{tcp://127.0.0.1:8307}}"
```
#### Run the profiler on a specific program:
```shell
blackfire run {{php path/to/file.php}}
```
#### Run the profiler and collect 10 samples:
```shell
blackfire --samples={{10}} run {{php path/to/file.php}}
```
#### Run the profiler and output results as JSON:
```shell
blackfire --json run {{php path/to/file.php}}
```
#### Upload a profiler file to the Blackfire web service:
```shell
blackfire upload {{path/to/file}}
```
#### View the status of profiles on the Blackfire web service:
```shell
blackfire status
```
{% endraw %}