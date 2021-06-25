---
layout: default
title: "tree"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tree">
  <a href="/tr/linux/tree.html">tree</a> <a href="#tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mevcut dizinin içeriğini ağaç biçiminde göster.
> Daha fazla bilgi için: <http://mama.indstate.edu/users/ice/tree/>.

#### Dosya ve dizinleri `num` değeri kadar derinlikte göster (1 olması durumunda mevcut dizin gösterilir):
```shell
tree -L {{num}}
```
#### Yalnızca dizinleri göster:
```shell
tree -d
```
#### Renklendirme açık olacak şekilde gizli dosyaları dahi göster:
```shell
tree -a -C
```
#### Ağacın satırlarını girintiler yerine tüm yolu belirterek göster:
```shell
tree -i -f
```
#### Tüm dosyaların ve dizinlerin eklenerek artan boyutlarını, insanların okuyabileceği bir biçimde göster:
```shell
tree -s -h --du
```
#### Ağaç hiyerarşisi içindeki dosyaları bir wildcard (glob) kalıbı kullanarak ve aranan özellikteki dosyalara sahip olmayan dizinleri yoksayarak göster:
```shell
tree -P '{{*.txt}}' --prune
```
#### Ağaç hiyerarşisi içindeki dizinleri bir wildcard (glob) kalıbı kullanarak ve istenen dizine atalığı olmayan dizinleri yoksayarak göster:
```shell
tree -P {{dizin_ismi}} --matchdirs --prune
```
#### Ağacı belirtilen dizinleri yoksayarak göster:
```shell
tree -I '{{dizin_ismi1|dizin_ismi2}}'
```
{% endraw %}