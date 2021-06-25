---
layout: default
title: "peludna-prognoza"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="peludna-prognoza">
  <a href="/en/common/peludna-prognoza.html">peludna-prognoza</a> <a href="#peludna-prognoza"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fetch pollen measurement data for Croatian cities from your terminal using Pliva's allergies data API.
> More information: <https://github.com/vladimyr/peludna-prognoza>.

#### Start an interactive search for a city and fetch data for it:
```shell
peludna-prognoza
```
#### Fetch data for a city:
```shell
peludna-prognoza "{{city}}"
```
#### Display data in a machine-readable format:
```shell
peludna-prognoza "{{city}}" --{{json|xml}}
```
#### Display the pollen measurement page for a city at <https://plivazdravlje.hr> in the default web browser:
```shell
peludna-prognoza "{{city}}" --web
```
{% endraw %}