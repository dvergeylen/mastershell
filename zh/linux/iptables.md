---
layout: default
title: "iptables"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="iptables">
  <a href="/zh/linux/iptables.html">iptables</a> <a href="#iptables"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 可用于配置 Linux 内核防火墙提供的过滤表、规则链和规则的程序。
> 更多信息： <https://www.netfilter.org/projects/iptables/>.

#### 查看过滤表的规则链、规则以及数据包/字节计数器：
```shell
sudo iptables -vnL
```
#### 设定规则链策略规则：
```shell
sudo iptables -P {{规则链}} {{规则}}
```
#### 追加规则到 IP 的规则链策略：
```shell
sudo iptables -A {{规则链}} -s {{ip}} -j {{规则}}
```
#### 追加规则到 IP 的规则链策略（考虑协议与端口）：
```shell
sudo iptables -A {{规则链}} -s {{ip}} -p {{协议}} --dport {{端口}} -j {{规则}}
```
#### 删除规则链中的规则：
```shell
sudo iptables -D {{规则链}} {{规则所在行号}}
```
#### 将指定过滤表的 iptables 配置保存到文件中：
```shell
sudo iptables-save -t {{过滤表名}} > {{iptables_文件路径}}
```
#### 从文件中还原 iptables 配置：
```shell
sudo iptables-restore < {{iptables_文件路径}}
```
{% endraw %}