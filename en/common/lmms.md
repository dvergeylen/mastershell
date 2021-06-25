---
layout: default
title: "lmms"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lmms">
  <a href="/en/common/lmms.html">lmms</a> <a href="#lmms"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Free, open source, cross-platform digital audio workstation.
> Render a `.mmp` or `.mmpz` project file, dump a `.mmpz` as XML, or start the GUI.
> More information: <https://lmms.io>.

#### Start the GUI:
```shell
lmms
```
#### Start the GUI and load external config:
```shell
lmms --config {{path/to/config.xml}}
```
#### Start the GUI and import MIDI or Hydrogen file:
```shell
lmms --import {{path/to/midi/or/hydrogen/file}}
```
#### Start the GUI with a specified window size:
```shell
lmms --geometry {{x_size}}x{{y_size}}+{{x_offset}}+{{y_offset}}
```
#### Dump a `.mmpz` file:
```shell
lmms dump {{path/to/mmpz/file.mmpz}}
```
#### Render a project file:
```shell
lmms render {{path/to/mmpz_or_mmp/file}}
```
#### Render the individual tracks of a project file:
```shell
lmms rendertracks {{path/to/mmpz_or_mmp/file}} {{path/to/dump/directory}}
```
#### Render with custom samplerate, format, and as a loop:
```shell
lmms render --samplerate {{88200}} --format {{ogg}} --loop --output {{path/to/output/file.ogg}}
```
{% endraw %}