---
layout: default
title: "sqlmap"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sqlmap">
  <a href="/en/common/sqlmap.html">sqlmap</a> <a href="#sqlmap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Detect and exploit SQL injection flaws.
> More information: <https://sqlmap.org>.

#### Run sqlmap against a single target URL:
```shell
python sqlmap.py -u "{{http://www.target.com/vuln.php?id=1}}"
```
#### Send data in a POST request (`--data` implies POST request):
```shell
python sqlmap.py -u "{{http://www.target.com/vuln.php}}" --data="{{id=1}}"
```
#### Change the parameter delimiter (& is the default):
```shell
python sqlmap.py -u "{{http://www.target.com/vuln.php}}" --data="{{query=foobar;id=1}}" --param-del="{{;}}"
```
#### Select a random `User-Agent` from `./txt/user-agents.txt` and use it:
```shell
python sqlmap.py -u "{{http://www.target.com/vuln.php}}" --random-agent
```
#### Provide user credentials for HTTP protocol authentication:
```shell
python sqlmap.py -u "{{http://www.target.com/vuln.php}}" --auth-type {{Basic}} --auth-cred "{{testuser:testpass}}"
```
{% endraw %}