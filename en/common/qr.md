---
layout: default
title: "qr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="qr">
  <a href="/en/common/qr.html">qr</a> <a href="#qr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate QR codes in the terminal with ANSI VT-100 escape codes.
> More information: <https://github.com/lincolnloop/python-qrcode/>.

#### Generate a QR code:
```shell
echo "{{data}}" | qr
```
#### Specify the error correction level (defaults to M):
```shell
echo "{{data}}" | qr --error-correction={{L|M|Q|H}}
```
{% endraw %}