---
layout: default
title: "matlab"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="matlab">
  <a href="/en/common/matlab.html">matlab</a> <a href="#matlab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Numerical computation environment by MathWorks.
> More information: <https://uk.mathworks.com/help/matlab/>.

#### Run without splash screen during startup:
```shell
matlab -nosplash
```
#### Execute a MATLAB statement:
```shell
matlab -r "{{matlab_statement}}"
```
#### Run a MATLAB script:
```shell
matlab -r "run({{path/to/script.m}})"
```
{% endraw %}