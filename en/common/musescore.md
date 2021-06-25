---
layout: default
title: "musescore"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="musescore">
  <a href="/en/common/musescore.html">musescore</a> <a href="#musescore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> MuseScore 3 sheet music editor.
> More information: <https://musescore.org/en/handbook/3/command-line-options>.

#### Use a specific audio driver:
```shell
musescore --audio-driver {{jack|alsa|portaudio|pulse}}
```
#### Set the MP3 output bitrate in kbit/s:
```shell
musescore --bitrate {{bitrate}}
```
#### Start MuseScore in debug mode:
```shell
musescore --debug
```
#### Enable experimental features, such as layers:
```shell
musescore --experimental
```
#### Export the given file to the specified output file. The file type depends on the given extension:
```shell
musescore --export-to {{output_file}} {{input_file}}
```
#### Print a diff between the given scores:
```shell
musescore --diff {{path/to/file1}} {{path/to/file2}}
```
#### Specify a MIDI import operations file:
```shell
musescore --midi-operations {{path/to/file}}
```
{% endraw %}