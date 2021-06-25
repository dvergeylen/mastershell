---
layout: default
title: "gitlab-ctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gitlab-ctl">
  <a href="/en/common/gitlab-ctl.html">gitlab-ctl</a> <a href="#gitlab-ctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI tool for managing the GitLab omnibus.
> More information: <https://docs.gitlab.com/omnibus/maintenance/>.

#### Display the status of every service:
```shell
sudo gitlab-ctl status
```
#### Display the status of a specific service:
```shell
sudo gitlab-ctl status {{nginx}}
```
#### Restart every service:
```shell
sudo gitlab-ctl restart
```
#### Restart a specific service:
```shell
sudo gitlab-ctl restart {{nginx}}
```
#### Display the logs of every service and keep reading until `Ctrl + C` is pressed:
```shell
sudo gitlab-ctl tail
```
#### Display the logs of a specific service:
```shell
sudo gitlab-ctl tail {{nginx}}
```
{% endraw %}