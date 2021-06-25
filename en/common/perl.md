---
layout: default
title: "perl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="perl">
  <a href="/en/common/perl.html">perl</a> <a href="#perl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Perl 5 language interpreter.
> More information: <https://www.perl.org>.

#### Parse and execute a Perl script:
```shell
perl {{script.pl}}
```
#### Check syntax errors on a Perl script:
```shell
perl -c {{script.pl}}
```
#### Parse and execute a Perl statement:
```shell
perl -e {{perl_statement}}
```
#### Run a Perl script in debug mode, using `perldebug`:
```shell
perl -d {{script.pl}}
```
#### Loo[p] over all lines of a file, editing them [i]n-place using a find/replace [e]xpression:
```shell
perl -p -i -e 's/{{find}}/{{replace}}/g' {{filename}}
```
#### Run a find/replace expression on a file, saving the original file with a given extension:
```shell
perl -p -i'.old' -e 's/{{find}}/{{replace}}/g' {{filename}}
```
#### Run a multiline find/replace expression on a file, and save the result in another file:
```shell
perl -p0e 's/{{foo\nbar}}/{{foobar}}/g' {{input_file}} > {{output_file}}
```
#### Run a regular expression on stdin, printing out the first capture group for each line:
```shell
cat {{path/to/input_file}} | perl -nle 'if (/.*({{foo}}).*/) {print "$1"; last;}'
```
{% endraw %}