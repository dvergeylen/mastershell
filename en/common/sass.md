---
layout: default
title: "sass"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sass">
  <a href="/en/common/sass.html">sass</a> <a href="#sass"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Converts SCSS or Sass files to CSS.
> More information: <https://sass-lang.com/documentation/cli/dart-sass>.

#### Convert a SCSS or Sass file to CSS and print out the result:
```shell
sass {{inputfile.scss|inputfile.sass}}
```
#### Convert a SCSS or Sass file to CSS and save the result to a file:
```shell
sass {{inputfile.scss|inputfile.sass}} {{outputfile.css}}
```
#### Watch a SCSS or Sass file for changes and output or update the CSS file with same filename:
```shell
sass --watch {{inputfile.scss|inputfile.sass}}
```
#### Watch a SCSS or Sass file for changes and output or update the CSS file with the given filename:
```shell
sass --watch {{inputfile.scss|inputfile.sass}}:{{outputfile.css}}
```
{% endraw %}