---
layout: default
title: "Stormlock"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="stormlock">
  <a href="/en/common/stormlock.html">Stormlock</a> <a href="#stormlock"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Centralized locking system.
> More information: <https://github.com/tmccombs/stormlock>.

#### Acquire a lease for resource:
```shell
stormlock aquire {{resource}}
```
#### Release the given lease for the given resource:
```shell
stormlock release {{resource}} {{lease_id}}
```
#### Show information on the current lease for a resource, if any:
```shell
stormlock current {{resource}}
```
#### Test if a lease for given resource is currently active:
```shell
stormlock is-held {{resource}} {{lease_id}}
```
{% endraw %}