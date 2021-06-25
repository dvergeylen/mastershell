---
layout: default
title: "docker build"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-build">
  <a href="/en/common/docker-build.html">docker build</a> <a href="#docker-build"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Build an image from a Dockerfile.
> More information: <https://docs.docker.com/engine/reference/commandline/build/>.

#### Build a docker image using the Dockerfile in the current directory:
```shell
docker build .
```
#### Build a docker image from a Dockerfile at a specified URL:
```shell
docker build {{github.com/creack/docker-firefox}}
```
#### Build a docker image and tag it:
```shell
docker build --tag {{name:tag}} .
```
#### Do not use the cache when building the image:
```shell
docker build --no-cache --tag {{name:tag}} .
```
#### Build a docker image using a specific Dockerfile:
```shell
docker build --file {{Dockerfile}} .
```
#### Build with custom build-time variables:
```shell
docker build --build-arg {{HTTP_PROXY=http://10.20.30.2:1234}} --build-arg {{FTP_PROXY=http://40.50.60.5:4567}} .
```
{% endraw %}