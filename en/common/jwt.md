---
layout: default
title: "jwt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jwt">
  <a href="/en/common/jwt.html">jwt</a> <a href="#jwt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line tool to work with JSON Web Tokens (JWTs).
> Encryption algorithms available are HS256, HS384, HS512, RS256, RS384, RS512, ES256, ES384.
> More information: <https://github.com/mike-engel/jwt-cli>.

#### Decode a JWT:
```shell
jwt decode {{jwt_string}}
```
#### Decode a JWT as a JSON string:
```shell
jwt decode -j {{jwt_string}}
```
#### Encode a JSON string to a JWT:
```shell
jwt encode --alg {{HS256}} --secret {{1234567890}} '{{json_string}}'
```
#### Encode key pair payload to JWT:
```shell
jwt encode --alg {{HS256}} --secret {{1234567890}} -P key=value
```
{% endraw %}