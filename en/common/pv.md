---
layout: default
title: "pv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pv">
  <a href="/en/common/pv.html">pv</a> <a href="#pv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Monitor the progress of data through a pipe.

#### Print the contents of the file and display a progress bar:
```shell
pv {{file}}
```
#### Measure the speed and amount of data flow between pipes (`-s` is optional):
```shell
command1 | pv -s {{expected_amount_of_data_for_eta}} | command2
```
#### Filter a file, see both progress and amount of output data:
```shell
pv -cN in {{big_text_file}} | grep {{pattern}} | pv -cN out > {{filtered_file}}
```
#### Attach to an already running process and see its file reading progress:
```shell
pv -d {{PID}}
```
#### Read an erroneous file, skip errors as `dd conv=sync,noerror` would:
```shell
pv -EE {{path/to/faulty_media}} > image.img
```
#### Stop reading after reading specified amount of data, rate limit to 1K/s:
```shell
pv -L 1K -S {{maximum_file_size_to_be_read}}
```
{% endraw %}