---
layout: default
title: "gitlab-runner"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gitlab-runner">
  <a href="/en/common/gitlab-runner.html">gitlab-runner</a> <a href="#gitlab-runner"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI tool for managing GitLab runners.
> More information: <https://docs.gitlab.com/runner/>.

#### Register a runner:
```shell
sudo gitlab-runner register --url {{https://gitlab.example.com}} --registration-token {{token}} --name {{name}}
```
#### Register a runner with a Docker executor:
```shell
sudo gitlab-runner register --url {{https://gitlab.example.com}} --registration-token {{token}} --name {{name}} --executor {{docker}}
```
#### Unregister a runner:
```shell
sudo gitlab-runner unregister --name {{name}}
```
#### Display the status of the runner service:
```shell
sudo gitlab-runner status
```
#### Restart the runner service:
```shell
sudo gitlab-runner restart
```
#### Check if the registered runners can connect to GitLab:
```shell
sudo gitlab-runner verify
```
{% endraw %}