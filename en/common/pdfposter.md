---
layout: default
title: "pdfposter"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pdfposter">
  <a href="/en/common/pdfposter.html">pdfposter</a> <a href="#pdfposter"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert a large-sheeted pdf into multiple A4 pages for printing.
> More information: <https://pdfposter.readthedocs.io>.

#### Convert an A2 poster into 4 A4 pages:
```shell
pdfposter --poster-size a2 {{input_file.pdf}} {{output_file.pdf}}
```
#### Scale an A4 poster to A3 and then generate 2 A4 pages:
```shell
pdfposter --scale 2 {{input_file.pdf}} {{output_file.pdf}}
```
{% endraw %}