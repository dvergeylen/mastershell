---
layout: default
title: "pio test"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pio-test">
  <a href="/en/common/pio-test.html">pio test</a> <a href="#pio-test"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run local tests on a PlatformIO project.
> More information: <https://docs.platformio.org/en/latest/core/userguide/cmd_test.html>.

#### Run all tests in all environments of the current PlatformIO project:
```shell
pio test
```
#### Test only specific environments:
```shell
pio test --environment {{environment1}} --environment {{environment2}}
```
#### Run only tests whose name matches a specific glob pattern:
```shell
pio test --filter "{{pattern}}"
```
#### Ignore tests whose name matches a specific glob pattern:
```shell
pio test --ignore "{{pattern}}"
```
#### Specify a port for firmware uploading:
```shell
pio test --upload-port {{upload_port}}
```
#### Specify a custom configuration file for running the tests:
```shell
pio test --project-conf {{path/to/platformio.ini}}
```
{% endraw %}