---
layout: default
title: "groff"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="groff">
  <a href="/en/common/groff.html">groff</a> <a href="#groff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Typesetting program that reads plain text mixed with formatting commands and produces formatted output.
> It is the GNU replacement for the `troff` and `nroff` Unix commands for text formatting.
> More information: <https://www.gnu.org/software/groff>.

#### Render a man page as plain text, and display the result:
```shell
groff -man -T utf8 {{manpage.1}}
```
#### Render a man page using the ASCII output device, and display it using a pager:
```shell
groff -man -T ascii {{manpage.1}} | less
```
#### Render a man page into an HTML file:
```shell
groff -man -T html {{manpage.1}} > {{page.html}}
```
#### Process a roff file using the `tbl` and `pic` preprocessors, and the `me` macro set:
```shell
groff -t -p -me -T utf8 {{foo.me}}
```
#### Run a `groff` command with preprocessor and macro options guessed by the `grog` utility:
```shell
eval "$(grog -T utf8 {{foo.me}})"
```
{% endraw %}