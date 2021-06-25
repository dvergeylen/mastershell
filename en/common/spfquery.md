---
layout: default
title: "spfquery"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="spfquery">
  <a href="/en/common/spfquery.html">spfquery</a> <a href="#spfquery"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Query Sender Policy Framework records to validate e-mail senders.
> More information: <https://www.libspf2.org/>.

#### Check if an IP address is allowed to send an e-mail from the specified e-mail address:
```shell
spfquery -ip {{8.8.8.8}} -sender {{sender@example.com}}
```
#### Turn on debugging output:
```shell
spfquery -ip {{8.8.8.8}} -sender {{sender@example.com}} --debug
```
{% endraw %}