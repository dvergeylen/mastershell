---
layout: default
title: "lldb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lldb">
  <a href="/en/common/lldb.html">lldb</a> <a href="#lldb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The LLVM Low-Level Debugger.
> More information: <https://lldb.llvm.org>.

#### Debug an executable:
```shell
lldb {{executable}}
```
#### Attach `lldb` to a running process with a given PID:
```shell
lldb -p {{pid}}
```
#### Wait for a new process to launch with a given name, and attach to it:
```shell
lldb -w -n {{process_name}}
```
{% endraw %}