---
layout: default
title: "curl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="curl">
  <a href="/en/common/curl.html">curl</a> <a href="#curl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Transfers data from or to a server.
> Supports most protocols, including HTTP, FTP, and POP3.
> More information: <https://curl.se>.

#### Download the contents of an URL to a file:
```shell
curl {{http://example.com}} --output {{filename}}
```
#### Download a file, saving the output under the filename indicated by the URL:
```shell
curl --remote-name {{http://example.com/filename}}
```
#### Download a file, following location redirects, and automatically continuing (resuming) a previous file transfer:
```shell
curl --remote-name --location --continue-at - {{http://example.com/filename}}
```
#### Send form-encoded data (POST request of type `application/x-www-form-urlencoded`). Use `--data @file_name` or `--data @'-'` to read from STDIN:
```shell
curl --data {{'name=bob'}} {{http://example.com/form}}
```
#### Send a request with an extra header, using a custom HTTP method:
```shell
curl --header {{'X-My-Header: 123'}} --request {{PUT}} {{http://example.com}}
```
#### Send data in JSON format, specifying the appropriate content-type header:
```shell
curl --data {{'{"name":"bob"}'}} --header {{'Content-Type: application/json'}} {{http://example.com/users/1234}}
```
#### Pass a user name and password for server authentication:
```shell
curl --user myusername:mypassword {{http://example.com}}
```
#### Pass client certificate and key for a resource, skipping certificate validation:
```shell
curl --cert {{client.pem}} --key {{key.pem}} --insecure {{https://example.com}}
```
{% endraw %}