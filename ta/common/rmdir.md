---
layout: default
title: "rmdir"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rmdir">
  <a href="/ta/common/rmdir.html">rmdir</a> <a href="#rmdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> அடைவை அழி.
> மேலும் தகவல்: <https://www.gnu.org/software/coreutils/rmdir>.

#### அடைவு வெறுமையாகயிருந்தால் அதனை அழி. உள்ளடக்கமுடைய அடைவை நீக்க `rm` யைப் பயன்படுத்தவும்:
```shell
rmdir {{அடைவிற்குப்/பாதை}}
```
#### அடைவுகளை தற்சுருளாக அழி (உட்பொதிவான அடைவுகளை அழிக்கப் பயன்படும்):
```shell
rmdir -p {{அடைவிற்குப்/பாதை}}
```
{% endraw %}