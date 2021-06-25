---
layout: default
title: "case"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="case">
  <a href="/zh/common/case.html">case</a> <a href="#case"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> case ... esac 与其他语言中的 switch ... case 语句类似，是一种多分枝选择结构.
> 更多信息： <https://manned.org/case>.

#### 通过字符串字面量判断执行分支:
```shell
case {{入参变量}} in {{字符字面量1}} {{执行语句块1}} ;; {{字符字面量2}}) {{执行语句块2}} ;; *) {{默认执行语句块}} ;; esac
```
#### 搭配通配符进行匹配，判断执行分支:
```shell
case {{入参变量}} in {{通配符或者字符字面量}}) {{执行语句块1}} ; ;; {{通配符或者字符字面量}}) {{执行语句块1}}; ;; *) {{echo "what?"}}; ;; esac
```
{% endraw %}