---
layout: default
title: "tesseract"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tesseract">
  <a href="/en/common/tesseract.html">tesseract</a> <a href="#tesseract"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> OCR (Optical Character Recognition) engine.
> More information: <https://github.com/tesseract-ocr/tesseract>.

#### Recognize text in an image and save it to `output.txt` (the `.txt` extension is added automatically):
```shell
tesseract {{image.png}} {{output}}
```
#### Specify a custom language (default is English) with an ISO 639-2 code (e.g. deu = Deutsch = German):
```shell
tesseract -l deu {{image.png}} {{output}}
```
#### List the ISO 639-2 codes of available languages:
```shell
tesseract --list-langs
```
#### Specify a custom page segmentation mode (default is 3):
```shell
tesseract -psm {{0_to_10}} {{image.png}} {{output}}
```
#### List page segmentation modes and their descriptions:
```shell
tesseract --help-psm
```
{% endraw %}