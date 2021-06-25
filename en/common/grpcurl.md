---
layout: default
title: "grpcurl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="grpcurl">
  <a href="/en/common/grpcurl.html">grpcurl</a> <a href="#grpcurl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Like cURL, but for gRPC: CLI tool for interacting with gRPC servers.
> More information: <https://github.com/fullstorydev/grpcurl>.

#### Send an empty request:
```shell
grpcurl {{grpc.server.com:443}} {{my.custom.server.Service/Method}}
```
#### Send a request with a header and a body:
```shell
grpcurl -H "{{Authorization: Bearer $token}}" -d {{'{"foo": "bar"}'}} {{grpc.server.com:443}} {{my.custom.server.Service/Method}}
```
#### List all services exposed by a server:
```shell
grpcurl {{grpc.server.com:443}} list
```
#### List all methods in a particular service:
```shell
grpcurl {{grpc.server.com:443}} list {{my.custom.server.Service}}
```
{% endraw %}