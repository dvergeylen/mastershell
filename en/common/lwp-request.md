---
layout: default
title: "lwp-request"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lwp-request">
  <a href="/en/common/lwp-request.html">lwp-request</a> <a href="#lwp-request"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple command-line HTTP client.
> Built with libwww-perl.
> More information: <https://metacpan.org/pod/lwp-request>.

#### Make a simple GET request:
```shell
lwp-request -m GET {{http://example.com/some/path}}
```
#### Upload a file with a POST request:
```shell
lwp-request -m POST {{http://example.com/some/path}} < {{path/to/file}}
```
#### Make a request with a custom user agent:
```shell
lwp-request -H 'User-Agent: {{user_agent}} -m {{METHOD}} {{http://example.com/some/path}}
```
#### Make a request with HTTP authentication:
```shell
lwp-request -C {{username}}:{{password}} -m {{METHOD}} {{http://example.com/some/path}}
```
#### Make a request and print request headers:
```shell
lwp-request -U -m {{METHOD}} {{http://example.com/some/path}}
```
#### Make a request and print response headers and status chain:
```shell
lwp-request -E -m {{METHOD}} {{http://example.com/some/path}}
```
{% endraw %}