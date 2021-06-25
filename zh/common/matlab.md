---
layout: default
title: "matlab"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="matlab">
  <a href="/zh/common/matlab.html">matlab</a> <a href="#matlab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> MathWorks 制作的数值计算环境。
> 更多信息: <https://uk.mathworks.com/help/matlab/>.

#### 在启动过程中，运行时不出现闪屏:
```shell
matlab -nosplash
```
#### 执行 MATLAB 语句:
```shell
matlab -r "{{matlab_语句}}"
```
#### 运行 MATLAB 脚本:
```shell
matlab -r "run({{路径/script.m}})"
```
{% endraw %}