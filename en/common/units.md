---
layout: default
title: "units"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="units">
  <a href="/en/common/units.html">units</a> <a href="#units"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Provide the conversion between two units of measure.
> More information: <https://www.gnu.org/software/units/>.

#### Run in interactive mode:
```shell
units
```
#### List all units containing a specific string in interactive mode:
```shell
search {{string}}
```
#### Show the conversion between two simple units:
```shell
units {{quarts}} {{tablespoons}}
```
#### Convert between units with quantities:
```shell
units "{{15 pounds}}" {{kilograms}}
```
#### Show the conversion between two compound units:
```shell
units "{{meters / second}}" "{{inches / hour}}"
```
#### Show the conversion between units with different dimensions:
```shell
units "{{acres}}" "{{ft^2}}"
```
#### Show the conversion of byte multipliers:
```shell
units "{{15 megabytes}}" {{bytes}}
```
{% endraw %}