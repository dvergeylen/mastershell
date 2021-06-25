---
layout: default
title: "tldr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tldr">
  <a href="/th/common/tldr.html">tldr</a> <a href="#tldr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> แสดงตัวอย่างแบบง่ายสำหรับเครื่องมือบน command-line จากโปรเจคท์ tldr-pages.
> ดูเพิ่มเติม: <https://tldr.sh>.

#### แสดงตัวอย่างการใช้งานคำสั่งที่ใช้บ่อย (บอกใบ้นิดนึง: นี่คือเหตุผลที่คุณสนใจใช้บริการของเราใช่ไหมล่ะ!):
```shell
tldr {{command}}
```
#### แสดงหน้า tldr ของคำสั่ง tar สำหรับระบบปฏิบัติการ Linux:
```shell
tldr -p {{linux}} {{tar}}
```
#### ขอความช่วยเหลือการใช้งานคำสั่งย่อยของ Git:
```shell
tldr {{git-checkout}}
```
#### ปรับปรุงข้อมูล tldr บนเครื่องของคุณให้ทันสมัย (ถ้าเครื่องของคุณรองรับการ caching):
```shell
tldr -u
```
{% endraw %}