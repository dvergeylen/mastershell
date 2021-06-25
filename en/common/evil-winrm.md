---
layout: default
title: "evil-winrm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="evil-winrm">
  <a href="/en/common/evil-winrm.html">evil-winrm</a> <a href="#evil-winrm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Windows Remote Management (WinRM) shell for pentesting.
> Once connected, we get a PowerShell prompt on the target host.
> More information: <https://github.com/Hackplayers/evil-winrm>.

#### Connect to a host:
```shell
evil-winrm --ip {{ip}} --user {{user}} --password {{password}}
```
#### Connect to a host, passing the password hash:
```shell
evil-winrm --ip {{ip}} --user {{user}} --hash {{nt_hash}}
```
#### Connect to a host, specifying directories for scripts and executables:
```shell
evil-winrm --ip {{ip}} --user {{user}} --password {{password}} --scripts {{path/to/scripts}} --executables {{path/to/executables}}
```
#### Connect to a host, using SSL:
```shell
evil-winrm --ip {{ip}} --user {{user}} --password {{password}} --ssl --pub-key {{path/to/pubkey}} --priv-key {{path/to/privkey}}
```
#### Upload a file to the host:
```shell
PS > upload {{path/to/local/file}} {{path/to/remote/file}}
```
#### Get a list of loaded PowerShell functions:
```shell
PS > menu
```
#### Load a PowerShell script from the `--scripts` directory:
```shell
PS > {{script.ps1}}
```
#### Invoke a binary on the host from the `--executables` directory:
```shell
PS > Invoke-Binary {{binary.exe}}
```
{% endraw %}