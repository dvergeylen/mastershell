---
layout: default
title: "windows"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#assoc">assoc</a>
* <a href="#attrib">attrib</a>
* <a href="#choco">choco</a>
* <a href="#choco-feature">choco feature</a>
* <a href="#choco-info">choco info</a>
* <a href="#choco-install">choco install</a>
* <a href="#choco-list">choco list</a>
* <a href="#choco-new">choco new</a>
* <a href="#choco-outdated">choco outdated</a>
* <a href="#choco-pack">choco pack</a>
* <a href="#choco-pin">choco pin</a>
* <a href="#choco-search">choco search</a>
* <a href="#choco-source">choco source</a>
* <a href="#choco-uninstall">choco uninstall</a>
* <a href="#choco-upgrade">choco upgrade</a>
* <a href="#cipher">cipher</a>
* <a href="#clip">clip</a>
* <a href="#cls">cls</a>
* <a href="#cmd">cmd</a>
* <a href="#cmstp">cmstp</a>
* <a href="#color">color</a>
* <a href="#comp">comp</a>
* <a href="#del">del</a>
* <a href="#dir">dir</a>
* <a href="#doskey">doskey</a>
* <a href="#driverquery">driverquery</a>
* <a href="#eventcreate">eventcreate</a>
* <a href="#exit">exit</a>
* <a href="#expand">expand</a>
* <a href="#explorer">explorer</a>
* <a href="#fc">fc</a>
* <a href="#find">find</a>
* <a href="#findstr">findstr</a>
* <a href="#finger">finger</a>
* <a href="#fondue">fondue</a>
* <a href="#forfiles">forfiles</a>
* <a href="#ftp">ftp</a>
* <a href="#ftype">ftype</a>
* <a href="#getmac">getmac</a>
* <a href="#ipconfig">ipconfig</a>
* <a href="#iscc">iscc</a>
* <a href="#logoff">logoff</a>
* <a href="#mkdir">mkdir</a>
* <a href="#mklink">mklink</a>
* <a href="#more">more</a>
* <a href="#msg">msg</a>
* <a href="#path">path</a>
* <a href="#pathping">pathping</a>
* <a href="#popd">popd</a>
* <a href="#powershell">powershell</a>
* <a href="#print">print</a>
* <a href="#pushd">pushd</a>
* <a href="#pwlauncher">pwlauncher</a>
* <a href="#rdpsign">rdpsign</a>
* <a href="#reg">reg</a>
* <a href="#reg-add">reg add</a>
* <a href="#reg-compare">reg compare</a>
* <a href="#reg-copy">reg copy</a>
* <a href="#reg-delete">reg delete</a>
* <a href="#reg-export">reg export</a>
* <a href="#reg-flags">reg flags</a>
* <a href="#reg-import">reg import</a>
* <a href="#reg-load">reg load</a>
* <a href="#reg-query">reg query</a>
* <a href="#reg-restore">reg restore</a>
* <a href="#reg-save">reg save</a>
* <a href="#reg-unload">reg unload</a>
* <a href="#repair-bde">repair-bde</a>
* <a href="#rmdir">rmdir</a>
* <a href="#scoop">scoop</a>
* <a href="#scoop-bucket">scoop bucket</a>
* <a href="#set">set</a>
* <a href="#sfc">sfc</a>
* <a href="#shutdown">shutdown</a>
* <a href="#subst">subst</a>
* <a href="#systeminfo">systeminfo</a>
* <a href="#takeown">takeown</a>
* <a href="#taskkill">taskkill</a>
* <a href="#tasklist">tasklist</a>
* <a href="#title">title</a>
* <a href="#tree">tree</a>
* <a href="#type">type</a>
* <a href="#tzutil">tzutil</a>
* <a href="#ver">ver</a>
* <a href="#vol">vol</a>
* <a href="#where">where</a>
* <a href="#whoami">whoami</a>
* <a href="#winget">winget</a>
* <a href="#wsl">wsl</a>
* <a href="#xcopy">xcopy</a>

{% raw %}
<h2 id="assoc">
  <a href="/zh/windows/assoc.html">assoc</a> <a href="#assoc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示或修改文件扩展名关联.

#### 显示所有当前文件扩展名关联的列表:
```shell
assoc
```
#### 显示指定扩展名的关联文件类型:
```shell
assoc {{.txt}}
```
#### 将文件扩展名与特定的文件类型关联:
```shell
assoc {{.txt}}={{txtfile}}
```
{% endraw %}{% raw %}
<h2 id="attrib">
  <a href="/zh/windows/attrib.html">attrib</a> <a href="#attrib"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示或修改文件和目录的属性.

#### 显示当前目录下所有文件的属性:
```shell
attrib
```
#### 显示当前目录和其子目录下所有文件的属性:
```shell
attrib /S
```
#### 显示当前目录和其子目录下所有文件和目录的属性:
```shell
attrib /S /D
```
#### 为一个文件增加只读属性:
```shell
attrib +R {{document.txt}}
```
#### 删除一个文件的系统和隐藏属性:
```shell
attrib -S -H {{document.txt}}
```
#### 为一个目录增加隐藏属性:
```shell
attrib +H {{目录的路径}}
```
{% endraw %}{% raw %}
<h2 id="choco-feature">
  <a href="/zh/windows/choco-feature.html">choco feature</a> <a href="#choco-feature"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Chocolatey 的交互功能.

#### 显示可用的功能列表:
```shell
choco feature list
```
#### 启用一个功能:
```shell
choco feature enable --name {{功能名称}}
```
#### 禁用一个功能:
```shell
choco feature disable --name {{功能名称}}
```
{% endraw %}{% raw %}
<h2 id="choco-info">
  <a href="/zh/windows/choco-info.html">choco info</a> <a href="#choco-info"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示有关 Chocolatey 包的详细信息.

#### 显示指定包的信息:
```shell
choco info {{包名}}
```
#### 显示一个本地已安装包的信息:
```shell
choco info {{包名}} --local-only
```
#### 从一个自定义的源来获取包的信息:
```shell
choco info {{包名}} --source {{源 URL|别名}}
```
#### 提供一个用户名和密码来进行验证:
```shell
choco info {{包名}} --user {{用户名}} --password {{密码}}
```
{% endraw %}{% raw %}
<h2 id="choco-install">
  <a href="/zh/windows/choco-install.html">choco install</a> <a href="#choco-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用 Chocolatey 下载一个或多个包.

#### 安装一个或多个用空格分隔的软件包:
```shell
choco install {{包名 包名 ..}}
```
#### 从一个自定义的配置文件中安装包:
```shell
choco install {{配置文件的路径}}
```
#### 安装一个特定的"nuspec"或"nupkg"文件:
```shell
choco install {{文件的路径}}
```
#### 安装一个指定版本的包:
```shell
choco install {{包名}} --version {{版本号}}
```
#### 允许安装一个包的多个版本:
```shell
choco install {{包名}} --allow-multiple
```
#### 自动确认所有提示:
```shell
choco install {{包名}} --yes
```
#### 从自定义的源处获取包:
```shell
choco install {{包名}} --source {{源 URL|别名}}
```
#### 提供一个用户名和密码来进行验证:
```shell
choco install {{包名}} --user {{用户名}} --password {{密码}}
```
{% endraw %}{% raw %}
<h2 id="choco-list">
  <a href="/zh/windows/choco-list.html">choco list</a> <a href="#choco-list"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用 Chocolatey 显示包列表.

#### 列出所有可用的包:
```shell
choco list
```
#### 列出所有本地已安装的包:
```shell
choco list --local-only
```
#### 显示包含本地程序的列表:
```shell
choco list --include-programs
```
#### 只显示已批准的包:
```shell
choco list --approved-only
```
#### Specify a custom source to display packages from 指定一个源来显示包列表:
```shell
choco list --source {{源 URL|别名}}
```
#### 提供一个用户名和密码来进行验证:
```shell
choco list --user {{用户名}} --password {{密码}}
```
{% endraw %}{% raw %}
<h2 id="choco-new">
  <a href="/zh/windows/choco-new.html">choco new</a> <a href="#choco-new"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用 Chocolatey 生成新的包规范文件.

#### 创建一个新的包框架:
```shell
choco new {{包名}}
```
#### 创建一个新的指定版本的包:
```shell
choco new {{包名}} --version {{版本号}}
```
#### 创建一个新的包并指定维护者的名字:
```shell
choco new {{包名}} --maintainer {{维护者名字}}
```
#### 在指定目录下创建新的包:
```shell
choco new {{包名}} --output-directory {{指定的目录路径}}
```
#### 创建一个新的包并指定其 32 位版和 64 位版的安装 URL:
```shell
choco new {{package_name}} url="{{url}}" url64="{{url}}"
```
{% endraw %}{% raw %}
<h2 id="choco-outdated">
  <a href="/zh/windows/choco-outdated.html">choco outdated</a> <a href="#choco-outdated"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用 Chocolatey 检查过时的包.

#### 用表格的形式列出过时的包:
```shell
choco outdated
```
#### 忽略输出中的固定包:
```shell
choco outdated --ignore-pinned
```
#### 从自定义的源处检查过时的包:
```shell
choco outdated --source {{源 URL|别名}}
```
#### 提供一个用户名和密码来进行验证:
```shell
choco outdated --user {{用户名}} --password {{密码}}
```
{% endraw %}{% raw %}
<h2 id="choco-pack">
  <a href="/zh/windows/choco-pack.html">choco pack</a> <a href="#choco-pack"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将 nuspec 打包到已编译的 nupkg.

#### 将 nuspec 打包到已编译的 nupkg:
```shell
choco pack {{nuspec 的路径}}
```
#### 将 nuspec 打包到已编译的 nupkg, 并指定生成的版本:
```shell
choco pack {{nuspec 的路径}} --version {{版本号}}
```
#### 将 nuspec 打包到已编译的 nupkg, 并输出到指定的目录:
```shell
choco pack {{nuspec 的路径}} --output-directory {{输出目录的路径}}
```
{% endraw %}{% raw %}
<h2 id="choco-pin">
  <a href="/zh/windows/choco-pin.html">choco pin</a> <a href="#choco-pin"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用 Chocolatey 将一个包固定到指定的版本.
> 被固定版本的包会在更新时自动忽略.

#### 显示被固定的包以及他们对应的版本号:
```shell
choco pin list
```
#### 将一个包固定至当前版本:
```shell
choco pin add --name {{包名}}
```
#### 将一个包固定直指定的版本:
```shell
choco pin add --name {{包名}} --version {{版本号}}
```
#### 移除指定包的固定状态:
```shell
choco pin remove --name {{包名}}
```
{% endraw %}{% raw %}
<h2 id="choco-search">
  <a href="/zh/windows/choco-search.html">choco search</a> <a href="#choco-search"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用 Chocolatey 搜索一个本地或远程的包.

#### 搜索一个包:
```shell
choco search {{查询语句}}
```
#### 搜索一个本地的包:
```shell
choco search {{查询语句}} --local-only
```
#### 只显示包含完全匹配的结果:
```shell
choco search {{查询语句}} --exact
```
#### 自动确认所有提示:
```shell
choco search {{查询语句}} --yes
```
#### 从自定义的源处搜索包:
```shell
choco search {{查询语句}} --source {{源 URL|别名}}
```
#### 提供一个用户名和密码来进行验证:
```shell
choco search {{查询语句}} --user {{用户名}} --password {{密码}}
```
{% endraw %}{% raw %}
<h2 id="choco-source">
  <a href="/zh/windows/choco-source.html">choco source</a> <a href="#choco-source"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用 Chocolatey 管理包的源.

#### 列出当前可用的源:
```shell
choco source list
```
#### 添加一个新的包源:
```shell
choco source add --name {{名称}} --source {{url}}
```
#### 添加包含凭据的新包源:
```shell
choco source add --name {{名称}} --source {{url}} --user {{用户名}} --password {{密码}}
```
#### 使用客户端证书添加新的包源:
```shell
choco source add --name {{名称}} --source {{url}} --cert {{证书的路径}}
```
#### 启用一个包源:
```shell
choco source enable --name {{名称}}
```
#### 禁用一个包源:
```shell
choco source disable --name {{名称}}
```
#### 移除一个包源:
```shell
choco source remove --name {{名称}}
```
{% endraw %}{% raw %}
<h2 id="choco-uninstall">
  <a href="/zh/windows/choco-uninstall.html">choco uninstall</a> <a href="#choco-uninstall"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用 Chocolatey 卸载一个或多个包.

#### 卸载一个或多个用空格分隔的软件包:
```shell
choco uninstall {{包名 『包名』 ..}}
```
#### 卸载一个指定版本的包:
```shell
choco uninstall {{包名}} --version {{版本号}}
```
#### 自动确认所有提示:
```shell
choco uninstall {{包名}} --yes
```
#### 卸载时同时删除其所有的依赖:
```shell
choco uninstall {{包名}} --remove-dependencies
```
#### 卸载全部包:
```shell
choco uninstall all
```
{% endraw %}{% raw %}
<h2 id="choco-upgrade">
  <a href="/zh/windows/choco-upgrade.html">choco upgrade</a> <a href="#choco-upgrade"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用 Chocolatey 升级一个或多个包.

#### 升级一个或多个用空格分隔的软件包:
```shell
choco upgrade {{包名 包名 ..}}
```
#### 将一个包升级到指定版本:
```shell
choco upgrade {{包名}} --version {{版本号}}
```
#### 升级全部包:
```shell
choco upgrade all
```
#### 升级除指定的用逗号分隔的包之外的所有包:
```shell
choco upgrade all --except "{{包名 , 包名 ..}}"
```
#### 自动确认所有提示:
```shell
choco upgrade {{包名}} --yes
```
#### 从自定义源处升级包:
```shell
choco upgrade {{包名}} --source {{源 URL|别名}}
```
#### 提供一个用户名和密码来进行验证:
```shell
choco upgrade {{包}} --user {{用户名}} --password {{密码}}
```
{% endraw %}{% raw %}
<h2 id="choco">
  <a href="/zh/windows/choco.html">choco</a> <a href="#choco"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Chocolatey 包管理器的命令行界面.
> 参见 `choco install`, `choco upgrade` 和其他的页面来获取额外的信息.

#### 执行 Chocolatey 命令:
```shell
choco {{命令}}
```
#### 显示基本的帮助页面:
```shell
choco -?
```
#### 显示指定命令的帮助页面:
```shell
choco {{命令}} -?
```
#### 显示 Chocolatey 的版本:
```shell
choco --version
```
{% endraw %}{% raw %}
<h2 id="cipher">
  <a href="/zh/windows/cipher.html">cipher</a> <a href="#cipher"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 加密或解密 NTFS 驱动器上的文件.

#### 加密文件或目录:
```shell
cipher /e:{{路径/文件或目录}}
```
#### 解密文件或目录:
```shell
cipher /d:{{路径/文件或目录}}
```
#### 安全地删除文件或目录:
```shell
cipher /w:{{路径/文件或目录}}
```
{% endraw %}{% raw %}
<h2 id="clip">
  <a href="/zh/windows/clip.html">clip</a> <a href="#clip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将输入的内容复制到 Windows 的剪贴板.

#### 用管道将命令的输出内容复制到 Windows 剪贴板:
```shell
{{dir}} | clip
```
#### 将一个文件中的内容复制到 Windows 剪贴板:
```shell
clip < {{文件的路径}}
```
{% endraw %}{% raw %}
<h2 id="cls">
  <a href="/zh/windows/cls.html">cls</a> <a href="#cls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 清屏.

#### 清屏:
```shell
cls
```
{% endraw %}{% raw %}
<h2 id="cmd">
  <a href="/zh/windows/cmd.html">cmd</a> <a href="#cmd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Windows 命令解释器.

#### 开启一个新的命令行实例:
```shell
cmd
```
#### 运行指定的命令然后退出:
```shell
cmd /c "{{命令}}"
```
#### 执行一个指定的命令，之后进入一个交互式 shell:
```shell
cmd /k "{{命令}}"
```
#### 不显示命令的输出结果:
```shell
cmd /q
```
#### 启用或禁用命令扩展:
```shell
cmd /e:{{on|off}}
```
#### 启用或禁用文件和目录名的自动补全:
```shell
cmd /f:{{on|off}}
```
#### 启用或禁用环境变量扩展:
```shell
cmd /v:{{on|off}}
```
#### 强制输出内容使用 Unicode 编码:
```shell
cmd /u
```
{% endraw %}{% raw %}
<h2 id="cmstp">
  <a href="/zh/windows/cmstp.html">cmstp</a> <a href="#cmstp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于管理连接服务配置文件的命令行工具.

#### 安装指定的配置文件:
```shell
cmstp "{{配置文件的路径}}"
```
#### 安装时不创建桌面快捷方式:
```shell
cmstp /ns "{{配置文件的路径}}"
```
#### 安装时不检查依赖:
```shell
cmstp /nf "{{配置文件的路径}}"
```
#### 仅为当前用户安装:
```shell
cmstp /su "{{配置文件的路径}}"
```
#### 为所有用户安装 （需要管理员权限）:
```shell
cmstp /au "{{配置文件的路径}}"
```
#### 静默安装:
```shell
cmstp /s "{{配置文件的路径}}"
```
#### 卸载一个指定的配置文件:
```shell
cmstp /u "{{配置文件的路径}}"
```
#### 静默删除:
```shell
cmstp /u /s "{{配置文件的路径}}"
```
{% endraw %}{% raw %}
<h2 id="color">
  <a href="/zh/windows/color.html">color</a> <a href="#color"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 设置控制台的前景色和背景色.

#### 将控制台颜色恢复至默认值:
```shell
color
```
#### 列出可用的颜色值和详细信息:
```shell
color /?
```
#### 将控制台前景色和背景色设置为指定颜色:
```shell
color {{前景色值}}{{背景色值}}
```
{% endraw %}{% raw %}
<h2 id="comp">
  <a href="/zh/windows/comp.html">comp</a> <a href="#comp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 比较两个文件或文件集的内容.
> 使用通配符 (*) 来比较文件集.

#### 交互式比较文件:
```shell
comp
```
#### 比较两个指定的文件:
```shell
comp {{文件 1 的路径}} {{文件 2 的路径}}
```
#### 比较两个文件集:
```shell
comp {{目录 1/*}} {{目录 2/*}}
```
#### 以十进制格式显示差异:
```shell
comp /d {{文件 1 的路径}} {{文件 2 的路径}}
```
#### 以 ASCII 字符显示差异:
```shell
comp /a {{文件 1 的路径}} {{文件 2 的路径}}
```
#### 显示不同的行数:
```shell
comp /l {{文件 1 的路径}} {{文件 2 的路径}}
```
#### 比较文件时不区分大小写:
```shell
comp /c {{文件 1 的路径}} {{文件 2 的路径}}
```
#### 只比较每个文件前 5 行的内容:
```shell
comp /n={{5}} {{文件 1 的路径}} {{文件 2 的路径}}
```
{% endraw %}{% raw %}
<h2 id="del">
  <a href="/zh/windows/del.html">del</a> <a href="#del"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 删除一个或多个文件.

#### 删除一个或多个以空格分隔的文件:
```shell
del {{文件 文件 ..}}
```
#### 在删除每个文件之前提示确认:
```shell
del {{文件}} /p
```
#### 强制删除只读文件:
```shell
del {{文件}} /f
```
#### 递归删除所有子目录中的文件:
```shell
del {{文件}} /s
```
#### 在基于全局通配符删除文件时不提示确认:
```shell
del {{文件}} /q
```
#### 显示帮助和所有的属性列表:
```shell
del /?
```
#### 根据指定的属性删除文件:
```shell
del {{文件}} /a {{属性}}
```
{% endraw %}{% raw %}
<h2 id="dir">
  <a href="/zh/windows/dir.html">dir</a> <a href="#dir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 列出目录的内容.

#### 显示当前目录的内容:
```shell
dir
```
#### 显示指定目录的内容:
```shell
dir {{目录的路径}}
```
#### 显示当前目录的内容，包括隐藏的文件:
```shell
dir /A
```
#### 显示指定目录的内容，包括隐藏的文件:
```shell
dir {{目录的路径}} /A
```
{% endraw %}{% raw %}
<h2 id="doskey">
  <a href="/zh/windows/doskey.html">doskey</a> <a href="#doskey"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 管理宏，Windows 命令和命令行.

#### 列出可用的宏:
```shell
doskey /macros
```
#### 创建一个新的宏:
```shell
doskey {{宏的名称}} = "{{命令}}"
```
#### 为指定可执行文件创建新的宏:
```shell
doskey /exename={{可执行文件名}} {{宏的名称}} = "{{命令}}"
```
#### 删除一个宏:
```shell
doskey {{宏的名称}} =
```
#### 列出所有储存在内存中的命令:
```shell
doskey /history
```
#### 将宏保存到文件以便于移植:
```shell
doskey /macros > {{保存宏的文件名}}
```
#### 从文件中加载宏:
```shell
doskey /macrofile = {{保存宏的文件名}}
```
{% endraw %}{% raw %}
<h2 id="driverquery">
  <a href="/zh/windows/driverquery.html">driverquery</a> <a href="#driverquery"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示已安装设备驱动程序的信息.

#### 显示所有已安装设备驱动程序的列表:
```shell
driverquery
```
#### 以指定格式显示驱动程序的列表:
```shell
driverquery /fo {{table|list|csv}}
```
#### 显示带有列的驱动程序列表，以表明它们是否已签名:
```shell
driverquery /si
```
#### 排除输出列表中的标题:
```shell
driverquery /nh
```
#### 显示远程计算机的驱动程序列表:
```shell
driverquery /s {{主机名}} /u {{用户名}} /p {{密码}}
```
#### 显示详细信息的驱动程序列表
```shell
driverquery /v
```
#### 显示详细的使用信息:
```shell
driverquery /?
```
{% endraw %}{% raw %}
<h2 id="eventcreate">
  <a href="/zh/windows/eventcreate.html">eventcreate</a> <a href="#eventcreate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在事件日志中创建自定义条目.
> 事件 ID 可以是 1 到 1000 之间的任意数值.

#### 在日志中创建一个具有给定 id（1-1000）的新事件:
```shell
eventcreate /t {{success|error|warning|information}} /id {{id}} /d "{{消息}}"
```
#### 在特定事件日志中创建事件:
```shell
eventcreate /l {{日志名}} /t {{类型}} /id {{id}} /d "{{消息}}"
```
#### 为新创建的事件指定来源:
```shell
eventcreate /so {{来源名}} /t {{类型}} /id {{id}} /d "{{消息}}"
```
#### 在远程计算机的事件日志中创建事件:
```shell
eventcreate /s {{主机名}} /u {{用户名}} /p {{密码}} /t {{类型}} /id {{id}} /d "{{消息}}"
```
{% endraw %}{% raw %}
<h2 id="exit">
  <a href="/zh/windows/exit.html">exit</a> <a href="#exit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 退出当前的命令行实例或 bat 脚本.

#### 退出当前的命令行实例:
```shell
exit
```
#### 退出当前的 bat 脚本:
```shell
exit /b
```
#### 使用一个指定的退出码退出:
```shell
exit {{退出码}}
```
{% endraw %}{% raw %}
<h2 id="expand">
  <a href="/zh/windows/expand.html">expand</a> <a href="#expand"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 解压一个或多个 cab 文件.

#### 将单文件 cab 文件解压到指定目录:
```shell
expand {{cab 文件路径}} {{指定的目录}}
```
#### 列出 cab 文件中的所有文件:
```shell
expand {{cab 文件路径}} {{指定的目录}} -d
```
#### 从 cab 文件中解压所有的文件:
```shell
expand {{cab 文件路径}} {{指定的目录}} -f:*
```
#### 从 cab 文件中解压一个特定的文件:
```shell
expand {{cab 文件路径}} {{指定的目录}} -f:{{文件名}}
```
#### 解压缩时忽略目录结构，并将它们添加到单个目录中:
```shell
expand {{cab 文件路径}} {{指定的目录}} -i
```
{% endraw %}{% raw %}
<h2 id="explorer">
  <a href="/zh/windows/explorer.html">explorer</a> <a href="#explorer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Windows 文件资源管理器.
> 更多信息： <https://ss64.com/nt/explorer.html>.

#### 打开 Windows 文件资源管理器:
```shell
explorer
```
#### 在当前目录打开 Windows 文件资源管理器:
```shell
explorer .
```
#### 在指定目录打开 Windows 文件资源管理器:
```shell
explorer {{path/to/directory}}
```
{% endraw %}{% raw %}
<h2 id="fc">
  <a href="/zh/windows/fc.html">fc</a> <a href="#fc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 比较两个文件或文件集之间的差异.
> 使用通配符 (*) 来比较文件集.

#### 比较两个指定的文件:
```shell
fc {{文件 1 的路径}} {{文件 2 的路径}}
```
#### 比较时不区分大小写:
```shell
fc /c {{文件 1 的路径}} {{文件 2 的路径}}
```
#### 将文件作为 Unicode 文本来进行比较:
```shell
fc /u {{文件 1 的路径}} {{文件 2 的路径}}
```
#### 将文件作为 ASCII 文本来进行比较:
```shell
fc /l {{文件 1 的路径}} {{文件 2 的路径}}
```
#### 将文件作为二进制来比较:
```shell
fc /b {{文件 1 的路径}} {{文件 2 的路径}}
```
#### 禁用制表符到空格的扩展:
```shell
fc /t {{文件 1 的路径}} {{文件 2 的路径}}
```
#### 压缩空格（制表符和空格）进行比较:
```shell
fc /w {{文件 1 的路径}} {{文件 2 的路径}}
```
{% endraw %}{% raw %}
<h2 id="find">
  <a href="/zh/windows/find.html">find</a> <a href="#find"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在一个或多个文件里查找指定字符串.

#### 查找包含指定字符串的行:
```shell
find {{字符串}} {{文件或目录的路径}}
```
#### 查找不包含指定字符串的行:
```shell
find {{字符串}} {{文件或目录的路径}} /v
```
#### 显示包含指定字符串的行的总数:
```shell
find {{字符串}} {{文件或目录的路径}} /c
```
#### 显示匹配的行的行数:
```shell
find {{字符串}} {{文件或目录的路径}} /n
```
{% endraw %}{% raw %}
<h2 id="findstr">
  <a href="/zh/windows/findstr.html">findstr</a> <a href="#findstr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在一个或多个文件中查找指定的文本.

#### 在所有文件中查找以空格分隔的字符串:
```shell
findstr "{{查询语句 查询语句 ..}}" *
```
#### 以递归方式在所有文件中查找以空格分隔的字符串:
```shell
findstr /s "{{查询语句 查询语句 ..}}" *
```
#### 查找时不区分大小写:
```shell
findstr /i "{{查询语句}}" *"
```
#### 使用正则表达式搜索:
```shell
findstr /r "{{正则表达式}}" *
```
#### 在所有文本文件中查找文字字符串（包含空格）:
```shell
findstr /c:"{{查询语句}}" *.txt
```
#### 只查找完全匹配的行:
```shell
findstr /x "{{查询语句}}" *
```
#### 显示匹配的行的行数:
```shell
findstr /n "{{查询语句}}" *
```
#### 只显示匹配的文件名:
```shell
findstr /m "{{查询语句}}" *
```
{% endraw %}{% raw %}
<h2 id="finger">
  <a href="/zh/windows/finger.html">finger</a> <a href="#finger"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 返回有关指定系统上的一个或多个用户的信息.
> 远程系统必须运行 Finger 服务.

#### 显示有关特定用户的信息:
```shell
finger {{用户名}}@{{主机名}}
```
#### 在指定的主机上显示所有用户的信息:
```shell
finger @{{主机名}}
```
#### 以更长的格式显示信息:
```shell
finger {{用户名}}@{{主机名}} -l
```
#### 显示帮助信息:
```shell
finger /?
```
{% endraw %}{% raw %}
<h2 id="fondue">
  <a href="/zh/windows/fondue.html">fondue</a> <a href="#fondue"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 可选 Windows 功能的命令行安装程序.

#### 启用一个指定的 Windows 功能:
```shell
fondue /enable-feature:{{功能}}
```
#### 向用户隐藏所有输出信息:
```shell
fondue /enable-feature:{{功能}} /hide-ux:all
```
#### 为错误报告指定调用者进程名称:
```shell
fondue /enable-feature:{{功能}} /caller-name:{{名称}}
```
{% endraw %}{% raw %}
<h2 id="forfiles">
  <a href="/zh/windows/forfiles.html">forfiles</a> <a href="#forfiles"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 选择一个或多个文件以执行指定的命令.

#### 在当前的目录中寻找文件:
```shell
forfiles
```
#### 在一个指定目录中寻找文件:
```shell
forfiles /p {{目录的路径}}
```
#### 为每个文件执行指定的命令:
```shell
forfiles /c "{{命令}}"
```
#### 使用通配符来寻找指定的文件:
```shell
forfiles /m {{通配符}}
```
#### 递归寻找文件:
```shell
forfiles /s
```
#### 搜索超过 5 天的文件:
```shell
forfiles /d {{+5}}
```
{% endraw %}{% raw %}
<h2 id="ftp">
  <a href="/zh/windows/ftp.html">ftp</a> <a href="#ftp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在本地和远程 FTP 服务器之间交互式传输文件.

#### 交互式连接一个远程的 FTP 服务:
```shell
ftp {{主机名}}
```
#### 匿名登录:
```shell
ftp -A {{主机名}}
```
#### 初始连接时禁用自动登录:
```shell
ftp -n {{主机名}}
```
#### 运行包含 FTP 命令列表的文件:
```shell
ftp -s:{{文件的路径}} {{主机名}}
```
#### 下载多个文件 （通配符表达式）:
```shell
mget {{*.png}}
```
#### 上传多个文件 （通配符表达式）:
```shell
mput {{*.zip}}
```
#### 在远程服务器上删除多个文件:
```shell
mdelete {{*.txt}}
```
#### 显示详细的帮助:
```shell
ftp --help
```
{% endraw %}{% raw %}
<h2 id="ftype">
  <a href="/zh/windows/ftype.html">ftype</a> <a href="#ftype"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示或修改用于文件扩展名关联的文件类型.

#### 显示所有文件类型的列表:
```shell
ftype
```
#### 显示特定文件类型的关联程序:
```shell
ftype {{文件类型}}
```
#### 设置特定文件类型的关联程序:
```shell
ftype {{文件类型}}="{{可执行命令的路径}}"
```
{% endraw %}{% raw %}
<h2 id="getmac">
  <a href="/zh/windows/getmac.html">getmac</a> <a href="#getmac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示系统的 MAC 地址.

#### 显示当前系统的 MAC 地址:
```shell
getmac
```
#### 以特定格式显示详细信息:
```shell
getmac /fo {{table|list|csv}}
```
#### 排除输出列表中的标题:
```shell
getmac /nh
```
#### 显示一个远程主机的 MAC 地址:
```shell
getmac /s {{主机名}} /u {{用户名}} /p {{密码}}
```
#### 详细显示 MAC 地址信息:
```shell
getmac /v
```
#### 显示详细的帮助信息:
```shell
getmac /?
```
{% endraw %}{% raw %}
<h2 id="ipconfig">
  <a href="/zh/windows/ipconfig.html">ipconfig</a> <a href="#ipconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示和管理 Windows 的网络配置.

#### 显示网络适配器列表:
```shell
ipconfig
```
#### 显示网络适配器的详细列表:
```shell
ipconfig /all
```
#### 为一个网络适配器重新获取 IP 地址:
```shell
ipconfig /renew {{适配器}}
```
#### 为一个网络适配器释放 IP 地址:
```shell
ipconfig /release {{适配器}}
```
#### 清除所有 DNS 缓存:
```shell
ipconfig /flushdns
```
{% endraw %}{% raw %}
<h2 id="iscc">
  <a href="/zh/windows/iscc.html">iscc</a> <a href="#iscc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Inno Setup 安装程序的编译器.
> 它将 Inno Setup 脚本编译为 Windows 安装程序可执行文件.
> 更多信息： <https://jrsoftware.org/isinfo.php>.

#### 编译一个 Inno Setup 脚本:
```shell
iscc {{脚本路径.iss}}
```
#### 静默编译一个 Inno Setup 安装程序:
```shell
iscc /Q {{脚本路径.iss}}
```
#### 编译已签名的 Inno Setup 安装程序:
```shell
iscc /S={{名称}}={{命令}} {{脚本路径.iss}}
```
{% endraw %}{% raw %}
<h2 id="logoff">
  <a href="/zh/windows/logoff.html">logoff</a> <a href="#logoff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 注销登录会话.

#### 注销当前会话:
```shell
logoff
```
#### 通过名称和 id 注销会话:
```shell
logoff {{会话名|会话 id}}
```
#### 在通过 RDP 连接的特定服务器上注销会话:
```shell
logoff {{会话名|会话 id}} /server:{{服务器名}}
```
{% endraw %}{% raw %}
<h2 id="mkdir">
  <a href="/zh/windows/mkdir.html">mkdir</a> <a href="#mkdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 创建一个目录.

#### 创建一个目录:
```shell
mkdir {{目录名}}
```
#### 递归创建目录及子目录:
```shell
mkdir {{子目录名}}
```
{% endraw %}{% raw %}
<h2 id="mklink">
  <a href="/zh/windows/mklink.html">mklink</a> <a href="#mklink"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 创建符号链接.

#### 创建指向文件的符号链接:
```shell
mklink {{链接文件的路径}} {{源文件路径}}
```
#### 创建指向目录的符号链接:
```shell
mklink /d {{链接文件的路径}} {{源目录路径}}
```
#### 创建指向文件的硬链接:
```shell
mklink /h {{链接文件的路径}} {{源目录路径}}
```
#### 创建目录链接:
```shell
mklink /j {{链接文件的路径}} {{源目录路径}}
```
{% endraw %}{% raw %}
<h2 id="more">
  <a href="/zh/windows/more.html">more</a> <a href="#more"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 分页显示标准输入或文件的输出.

#### 分页显示标准输入的输出:
```shell
{{echo test}} | more
```
#### 分页显示一个或多个文件的内容:
```shell
more {{文件的路径}}
```
#### 将制表符转换为指定的空格数:
```shell
more {{文件的路径}} /t{{空格数}}
```
#### 显示内容前先清屏:
```shell
more {{文件的路径}} /c
```
#### 从第 5 行开始显示输出:
```shell
more {{文件的路径}} +{{5}}
```
#### 启用扩展交互模式（请参阅使用帮助）:
```shell
more {{文件的路径}} /e
```
#### 显示全部帮助信息:
```shell
more /?
```
{% endraw %}{% raw %}
<h2 id="msg">
  <a href="/zh/windows/msg.html">msg</a> <a href="#msg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 向指定的用户或会话发送信息.

#### 向指定的用户或会话发送信息:
```shell
msg {{用户名|会话名|会话 id}} {{信息}}
```
#### 从标准输入发送信息:
```shell
echo "{{信息}}" | msg {{用户名|会话名|会话 id}}
```
#### 向指定的服务器发送消息:
```shell
msg /server:{{服务器名称}} {{用户名|会话名|会话 id}}
```
#### 向当前计算机的所有用户发送消息:
```shell
msg *
```
#### 设置发送消息的延迟:
```shell
msg /time:{{秒}}
```
{% endraw %}{% raw %}
<h2 id="path">
  <a href="/zh/windows/path.html">path</a> <a href="#path"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示或设置可执行文件的搜索路径.

#### 显示当前的路径:
```shell
path
```
#### 将路径设置为一个或多个以分号分隔的目录:
```shell
path {{目录的路径 1[; 目录的路径 2]}}
```
#### 将新的目录添加到源路径后:
```shell
path {{目录的路径}};%path%
```
#### 将命令提示符设置为仅搜索当前目录中的可执行文件:
```shell
path ;
```
{% endraw %}{% raw %}
<h2 id="pathping">
  <a href="/zh/windows/pathping.html">pathping</a> <a href="#pathping"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一种结合了`ping`和`tracert`功能的跟踪路由工具.

#### Ping 并追踪主机的路由:
```shell
pathping {{主机名}}
```
#### 不要对主机名执行 IP 地址的反向查找:
```shell
pathping {{主机名}} -n
```
#### 指定要搜索目标的最大跃点数（默认值为 30）:
```shell
pathping {{主机名}} -h {{最大跃点数}}
```
#### 指定 ping 之间等待的毫秒数（默认值为 240）:
```shell
pathping {{主机名}} -p {{时间}}
```
#### 指定每跳的查询数（默认值为 100）:
```shell
pathping {{主机名}} -q {{查询语句}}
```
#### 强制使用 IPV4:
```shell
pathping {{主机名}} -4
```
#### 强制使用 IPV6:
```shell
pathping {{主机名}} -6
```
#### 显示详细的使用帮助:
```shell
pathping /?
```
{% endraw %}{% raw %}
<h2 id="popd">
  <a href="/zh/windows/popd.html">popd</a> <a href="#popd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将当前目录切换到`pushd`命令存储的目录.

#### 切换到储存在栈顶的目录:
```shell
popd
```
{% endraw %}{% raw %}
<h2 id="powershell">
  <a href="/zh/windows/powershell.html">powershell</a> <a href="#powershell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 专为系统管理而设计的命令行 shell 和脚本语言.
> 更多信息: <https://docs.microsoft.com/windows-server/administration/windows-commands/powershell>.

#### 在命令提示符窗口中启动 Windows PowerShell 会话:
```shell
powershell
```
#### 加载一个特定的 PowerShell 控制台文件:
```shell
powershell -PSConsoleFile {{路径/file}}
```
#### 用指定版本的 PowerShell 启动会话:
```shell
powershell -Version {{版本}}
```
#### 防止运行启动命令后 shell 退出:
```shell
powershell -NoExit
```
#### 描述发送到 PowerShell 的数据格式:
```shell
powershell -InputFormat {{Text|XML}}
```
#### 设定 PowerShell 输出的格式:
```shell
powershell -OutputFormat {{Text|XML}}
```
#### 显示帮助:
```shell
powershell -Help
```
{% endraw %}{% raw %}
<h2 id="print">
  <a href="/zh/windows/print.html">print</a> <a href="#print"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将文本文件打印到打印机.

#### 将文本文件打印到默认的打印机:
```shell
print {{文件的路径}}
```
#### 将文本文件打印到指定的打印机:
```shell
print /d:{{打印机}} {{文件的路径}}
```
{% endraw %}{% raw %}
<h2 id="pushd">
  <a href="/zh/windows/pushd.html">pushd</a> <a href="#pushd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将目录储存在栈顶以便稍后访问.
> 参考`popd`命令来切换到原目录.

#### 切换目录并将它放至栈:
```shell
pushd {{目录}}
```
{% endraw %}{% raw %}
<h2 id="pwlauncher">
  <a href="/zh/windows/pwlauncher.html">pwlauncher</a> <a href="#pwlauncher"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于管理 Windows To Go 启动选项的命令行工具.

#### 显示当前 Windows To Go 的状态:
```shell
pwlauncher
```
#### 启用或禁用 Windows To Go 的启动选项:
```shell
pwlauncher /{{enable|disable}}
```
{% endraw %}{% raw %}
<h2 id="rdpsign">
  <a href="/zh/windows/rdpsign.html">rdpsign</a> <a href="#rdpsign"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于签名远程桌面协议（RDP）文件的工具.

#### 为一个 RDP 文件签名:
```shell
rdpsign {{文件路径.rdp}}
```
#### 使用一个指定的 sha256 哈希值为 RDP 文件签名:
```shell
rdpsign {{文件路径.rdp}} /sha265 {{哈希值}}
```
#### 启用静默输出:
```shell
rdpsign {{文件路径.rdp}} /q
```
#### 显示详细的信息、警告和状态:
```shell
rdpsign {{文件路径.rdp}} /v
```
#### 在不更新文件的情况下将输出显示到标准输出来测试签名:
```shell
rdpsign {{文件路径.rdp}} /l
```
{% endraw %}{% raw %}
<h2 id="reg-add">
  <a href="/zh/windows/reg-add.html">reg add</a> <a href="#reg-add"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将新的键值添加到注册表中.

#### 添加一个新的注册表键:
```shell
reg add {{键名}}
```
#### 在指定的键下添加新值:
```shell
reg add {{键名}} /v {{值}}
```
#### Add a new value with specific data:
```shell
reg add {{键名}} /d {{数据}}
```
#### 向具有特定数据类型的键添加新值:
```shell
reg add {{键名}} /t {{类型}}
```
#### 在没有提示的情况下强制覆盖现有的注册表值:
```shell
reg add {{键名}} /f
```
{% endraw %}{% raw %}
<h2 id="reg-compare">
  <a href="/zh/windows/reg-compare.html">reg compare</a> <a href="#reg-compare"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 比较注册表中的键和值.

#### 比较两个键中的所有值:
```shell
reg compare {{第一个键名}} {{第二个键名}}
```
#### 比较两个键中指定的值:
```shell
reg compare {{第一个键名}} {{第二个键名}} /v {{值}}
```
#### 比较两个键中的所有子键和值:
```shell
reg compare {{第一个键名}} {{第二个键名}} /s
```
#### 仅输出指定键之间匹配的结果:
```shell
reg compare {{第一个键名}} {{第二个键名}} /os
```
#### 输出两个键之间的匹配和差异:
```shell
reg compare {{第一个键名}} {{第二个键名}} /oa
```
{% endraw %}{% raw %}
<h2 id="reg-copy">
  <a href="/zh/windows/reg-copy.html">reg copy</a> <a href="#reg-copy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 复制注册表中的键和值.

#### 将注册表键复制到新的注册表位置:
```shell
reg copy {{旧键名}} {{新键名}}
```
#### 递归将注册表键复制到新的注册表位置:
```shell
reg copy {{旧键名}} {{新键名}} /s
```
#### 在没有提示的情况下强制复制注册表键:
```shell
reg copy {{旧键名}} {{新键名}} /f
```
{% endraw %}{% raw %}
<h2 id="reg-delete">
  <a href="/zh/windows/reg-delete.html">reg delete</a> <a href="#reg-delete"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 从注册表中删除键和值.

#### 删除一个指定的键:
```shell
reg delete {{键名}}
```
#### 删除键中指定的值:
```shell
reg delete {{键名}} /v {{值}}
```
#### 递归删除指定键下所有的值:
```shell
reg delete {{键名}} /va
```
#### 在没有提示的情况下递归删除键中所有的值:
```shell
reg delete {{键名}} /f /va
```
{% endraw %}{% raw %}
<h2 id="reg-export">
  <a href="/zh/windows/reg-export.html">reg export</a> <a href="#reg-export"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将指定的子键和值导出到文件中.

#### 导出指定键下所有的子键和值:
```shell
reg export {{键名}} {{导出文件的路径.reg}}
```
#### 在没有提示的情况下强制覆盖现有文件:
```shell
reg export {{键名}} {{导出文件的路径.reg}} /y
```
{% endraw %}{% raw %}
<h2 id="reg-flags">
  <a href="/zh/windows/reg-flags.html">reg flags</a> <a href="#reg-flags"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示或设置注册表键的标志.

#### 显示当前指定键的标志:
```shell
reg flags {{键名}} query
```
#### 显示帮助和可用的标志类型:
```shell
reg flags /?
```
#### 为特定键设置指定以空格分隔的标志，并取消设置未提及的标志:
```shell
reg flags {{键名}} set {{标志 1 标志 2 ..}}
```
#### 为指定的键和其子键设置标志:
```shell
reg flags {{键名}} set {{标志}} /s
```
{% endraw %}{% raw %}
<h2 id="reg-import">
  <a href="/zh/windows/reg-import.html">reg import</a> <a href="#reg-import"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 从一个文件导入所有可用的键、子键和值.

#### 从一个文件导入所有可用的键、子键和值:
```shell
reg import {{reg 文件的路径}}
```
{% endraw %}{% raw %}
<h2 id="reg-load">
  <a href="/zh/windows/reg-load.html">reg load</a> <a href="#reg-load"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将保存的子键加载到不同的子键中.
> This is intended for troubleshooting and temporary keys.

#### 将备份文件加载到指定的键中:
```shell
reg load {{键名}} {{文件的路径}}
```
{% endraw %}{% raw %}
<h2 id="reg-query">
  <a href="/zh/windows/reg-query.html">reg query</a> <a href="#reg-query"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示注册表中键和子键的值.

#### 显示一个键中的所有值:
```shell
reg query {{键名}}
```
#### 显示键中指定的值:
```shell
reg query {{键名}} /v {{值}}
```
#### 显示指定键和其子键中的所有的值:
```shell
reg query {{键名}} /s
```
#### 搜索与特定模式匹配的键和值:
```shell
reg query {{键名}} /f "{{查询语句}}"
```
#### 显示与指定数据类型匹配的键的值:
```shell
reg query {{键名}} /t {{类型}}
```
{% endraw %}{% raw %}
<h2 id="reg-restore">
  <a href="/zh/windows/reg-restore.html">reg restore</a> <a href="#reg-restore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 从备份文件中恢复键和值.
> 参见 `reg-save` 来获取更多的信息.

#### 使用备份文件中的数据覆盖指定的键:
```shell
reg restore {{键名}} {{文件路径}}
```
{% endraw %}{% raw %}
<h2 id="reg-save">
  <a href="/zh/windows/reg-save.html">reg save</a> <a href="#reg-save"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将注册表键、子键的所有值保存到一个文件中.

#### 将注册表键、子键的所有值保存到一个文件中:
```shell
reg save {{键名}} {{文件的路径}}
```
#### 在没有提示的情况下强制覆盖现有文件:
```shell
reg save {{键名}} {{文件的路径}} /y
```
{% endraw %}{% raw %}
<h2 id="reg-unload">
  <a href="/zh/windows/reg-unload.html">reg unload</a> <a href="#reg-unload"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 从使用`reg load`命令加载的注册表中删除数据.

#### 从使用`reg load`命令加载的注册表中删除数据:
```shell
reg unload {{键名}}
```
{% endraw %}{% raw %}
<h2 id="reg">
  <a href="/zh/windows/reg.html">reg</a> <a href="#reg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于在 Windows 注册表中管理键及其值的命令行界面.
> 参见 `reg-query`, `reg-add` 和其他的页面来获取额外的信息.

#### 执行注册表命令:
```shell
reg {{命令}}
```
#### 显示常规信息并列出所有可用命令:
```shell
reg /?
```
#### 显示指定命令的帮助信息:
```shell
reg {{命令}} /?
```
{% endraw %}{% raw %}
<h2 id="repair-bde">
  <a href="/zh/windows/repair-bde.html">repair-bde</a> <a href="#repair-bde"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 尝试修复或解密损坏的 BitLocker 加密卷.

#### 尝试修复一个指定的卷:
```shell
repair-bde {{C:}}
```
#### 尝试修复指定的卷并输出到另一个卷:
```shell
repair-bde {{C:}} {{D:}}
```
#### 尝试使用提供的恢复密钥文件修复指定的卷:
```shell
repair-bde {{C:}} -RecoveryKey {{bek 文件的路径}}
```
#### 尝试使用提供的数字恢复密码修复指定的卷:
```shell
repair-bde {{C:}} -RecoveryPassword {{密码}}
```
#### 尝试使用提供的密码修复指定的卷:
```shell
repair-bde {{C:}} -Password {{密码}}
```
#### 尝试使用提供的密钥包修复指定的卷:
```shell
repair-bde {{C:}} -KeyPackage {{目录的路径}}
```
#### 将日志输出到指定的文件:
```shell
repair-bde {{C:}} -LogFile {{文件的路径}}
```
#### 显示所有可用的选项:
```shell
repair-bde /?
```
{% endraw %}{% raw %}
<h2 id="rmdir">
  <a href="/zh/windows/rmdir.html">rmdir</a> <a href="#rmdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 删除一个目录和其中的内容.

#### 删除一个空目录:
```shell
rmdir {{目录的路径}}
```
#### 递归删除一个目录及其中的内容:
```shell
rmdir {{目录的路径}} /s
```
#### 在没有提示的情况下递归删除目录及其内容:
```shell
rmdir {{path/to/directory}} /s /q
```
{% endraw %}{% raw %}
<h2 id="scoop-bucket">
  <a href="/zh/windows/scoop-bucket.html">scoop bucket</a> <a href="#scoop-bucket"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 管理 bucket: 包含描述 scoop 应如何安装应用程序的文件的 Git 存储库。
> 如果 Scoop 不知道 bucket 在哪里，则必须指定其存储库位置。
> 更多信息: <https://github.com/lukesampson/scoop/wiki/Buckets>.

#### 列出所有正在使用的 bucket:
```shell
scoop bucket list
```
#### 列出所有已知 bucket:
```shell
scoop bucket known
```
#### 按名称添加一个已知 bucket:
```shell
scoop bucket add {{名称}}
```
#### 通过名称和 Git 存储库 URL 添加未知 bucket:
```shell
scoop bucket add {{名称}} {{https://example.com/repository.git}}
```
#### 按名称删除 bucket:
```shell
scoop bucket rm {{名称}}
```
{% endraw %}{% raw %}
<h2 id="scoop">
  <a href="/zh/windows/scoop.html">scoop</a> <a href="#scoop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Windows 的命令行安装程序.

#### 安装一个包:
```shell
scoop install {{包名}}
```
#### 删除一个包:
```shell
scoop uninstall {{包名}}
```
#### 更新所有已安装的包:
```shell
scoop update *
```
#### 列出所有已安装的包:
```shell
scoop list
```
#### 显示一个包的信息:
```shell
scoop info {{包名}}
```
#### 搜索一个包:
```shell
scoop search {{包名}}
```
#### 列出所有已知的桶 (“桶”代表程序的仓库）:
```shell
scoop bucket known
```
#### 通过别名或 Git 存储库 URL 添加存储桶:
```shell
scoop bucket add {{bucket}}
```
{% endraw %}{% raw %}
<h2 id="set">
  <a href="/zh/windows/set.html">set</a> <a href="#set"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示或设置当前命令行实例的环境变量.

#### 列出当前所有环境变量:
```shell
set
```
#### 为一个环境变量设置指定的值:
```shell
set {{变量名}}={{值}}
```
#### 列出以指定字符串开头的环境变量:
```shell
set {{变量名}}
```
#### 提示用户输入指定变量的值:
```shell
set /p {{变量名}}={{提示信息}}
```
{% endraw %}{% raw %}
<h2 id="sfc">
  <a href="/zh/windows/sfc.html">sfc</a> <a href="#sfc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 扫描 Windows 系统文件的完整性.

#### 显示命令的使用方法:
```shell
sfc
```
#### 扫描所有的系统文件，如果可能的话，修复所有出现的问题:
```shell
sfc /scannow
```
#### 扫描系统文件，但不修复出现的问题:
```shell
sfc /verifyonly
```
#### 扫描指定的文件，如果可能的话，修复所有出现的问题:
```shell
sfc /scanfile={{文件的路径}}
```
#### 扫描指定的文件，但不修复出现的问题:
```shell
sfc /verifyfile={{文件的路径}}
```
#### 当离线修复时，指定引导目录:
```shell
sfc /offbootdir={{目录的路径}}
```
#### 当离线修复时，指定 Windows 目录:
```shell
sfc /offwindir={{文件的路径}}
```
{% endraw %}{% raw %}
<h2 id="shutdown">
  <a href="/zh/windows/shutdown.html">shutdown</a> <a href="#shutdown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于关闭，重新启动或注销计算机的工具.

#### 关闭当前的计算机:
```shell
shutdown /s
```
#### 重启当前的计算机:
```shell
shutdown /r
```
#### 休眠当前的计算机:
```shell
shutdown /h
```
#### 注销当前的计算机:
```shell
shutdown /l
```
#### 指定在关闭之前等待的时间（以秒为单位）:
```shell
shutdown /s /t {{秒}}
```
#### 指定一个关机的理由:
```shell
shutdown /s /c "{{理由}}"
```
#### 在超时之前取消关机指令:
```shell
shutdown /a
```
#### 关闭远程的计算机:
```shell
shutdown /m {{\\ 主机名}}
```
{% endraw %}{% raw %}
<h2 id="subst">
  <a href="/zh/windows/subst.html">subst</a> <a href="#subst"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将路径与虚拟驱动器号关联.

#### 列出已激活的关联:
```shell
subst
```
#### 添加一个关联:
```shell
subst {{Z:}} {{C:\Python2.7}}
```
#### 删除一个关联:
```shell
subst {{Z:}} /d
```
{% endraw %}{% raw %}
<h2 id="systeminfo">
  <a href="/zh/windows/systeminfo.html">systeminfo</a> <a href="#systeminfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示本地或远程计算机的操作系统配置.

#### 显示本地计算机的操作系统配置:
```shell
systeminfo
```
#### 以指定的输出格式显示系统配置:
```shell
systeminfo /fo {{table|list|csv}}
```
#### 显示远程计算机的系统配置:
```shell
systeminfo /s {{远程主机名}} /u {{用户名}} /p {{密码}}
```
#### 显示详细的帮助信息:
```shell
systeminfo /?
```
{% endraw %}{% raw %}
<h2 id="takeown">
  <a href="/zh/windows/takeown.html">takeown</a> <a href="#takeown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 取得文件或目录的所有权.
> 更多信息: <https://docs.microsoft.com/windows-server/administration/windows-commands/takeown>.

#### 取得指定文件的所有权:
```shell
takeown /f {{路径/文件}}
```
#### 取得指定目录的所有权:
```shell
takeown /d {{路径/目录}}
```
#### 取得指定目录和所有子目录的所有权:
```shell
takeown /r /d {{路径/目录}}
```
#### 将所有权更改为管理员组，而不是当前用户:
```shell
takeown /a /f {{路径/文件}}
```
{% endraw %}{% raw %}
<h2 id="taskkill">
  <a href="/zh/windows/taskkill.html">taskkill</a> <a href="#taskkill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 按进程 id 或进程名终止进程.

#### 通过进程 id 终止进程:
```shell
taskkill /pid {{进程 id}}
```
#### 通过进程名终止进程:
```shell
taskkill /im {{进程名}}
```
#### 强制终止一个指定的进程:
```shell
taskkill /pid {{进程名}} /f
```
#### 终止一个进程及其子进程:
```shell
taskkill /im {{进程名}} /t
```
#### 终止远程计算机上的进程:
```shell
taskkill /pid {{进程 id}} /s {{远程主机名}}
```
#### 显示命令的帮助信息:
```shell
taskkill /?
```
{% endraw %}{% raw %}
<h2 id="tasklist">
  <a href="/zh/windows/tasklist.html">tasklist</a> <a href="#tasklist"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示本地或远程计算机上当前正在运行的进程的列表.

#### 显示当前正在运行的进程:
```shell
tasklist
```
#### 使用指定的格式显示当前进程列表:
```shell
tasklist /fo {{table|list|csv}}
```
#### 已匹配的方式 (.exe, .dll) 显示当前运行的进程:
```shell
tasklist /m {{匹配模式}}
```
#### 显示在远程计算机上运行的进程:
```shell
tasklist /s {{远程主机名}} /u {{用户名}} /p {{密码}}
```
#### 显示每个进程中的服务信息:
```shell
tasklist /svc
```
{% endraw %}{% raw %}
<h2 id="title">
  <a href="/zh/windows/title.html">title</a> <a href="#title"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 设置命令提示符窗口的标题.

#### 设置当前的命令提示符窗口的标题:
```shell
title {{新标题}}
```
{% endraw %}{% raw %}
<h2 id="tree">
  <a href="/zh/windows/tree.html">tree</a> <a href="#tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 以目录树的形式显示指定目录的所有文件夹和文件.

#### 显示当前目录的目录树:
```shell
tree
```
#### 显示指定目录的目录树:
```shell
tree {{目录的路径}}
```
#### 显示目录中文件的目录树:
```shell
tree {{目录的路径}} /f
```
#### 使用 ASCII 字符而不是扩展字符显示目录树:
```shell
tree {{目录的路径}} /a
```
{% endraw %}{% raw %}
<h2 id="type">
  <a href="/zh/windows/type.html">type</a> <a href="#type"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示文件的内容.

#### 显示特定文件的内容:
```shell
type {{文件的路径}}
```
{% endraw %}{% raw %}
<h2 id="tzutil">
  <a href="/zh/windows/tzutil.html">tzutil</a> <a href="#tzutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于显示或配置系统时区的工具.

#### 获取当前的时区:
```shell
tzutil /g
```
#### 显示可用的时区列表:
```shell
tzutil /l
```
#### 将系统时区设置为特定值:
```shell
tzutil /s {{时区 id}}
```
{% endraw %}{% raw %}
<h2 id="ver">
  <a href="/zh/windows/ver.html">ver</a> <a href="#ver"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示当前 Windows 或 MS-DOS 的版本号.

#### Display the current version number:
```shell
ver
```
{% endraw %}{% raw %}
<h2 id="vol">
  <a href="/zh/windows/vol.html">vol</a> <a href="#vol"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示有关卷的信息.

#### 显示当前驱动器的标签和序列号:
```shell
vol
```
#### 显示指定驱动器的标签和序列号:
```shell
vol {{D:}}
```
{% endraw %}{% raw %}
<h2 id="where">
  <a href="/zh/windows/where.html">where</a> <a href="#where"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示与搜索模式匹配的文件的位置.
> 在默认情况下，搜索是在当前目录和 PATH 环境变量指定的路径中执行的.

#### 显示匹配的文件的位置:
```shell
where {{文件模式}}
```
#### 显示匹配的文件的位置、大小和日期:
```shell
where /T {{文件模式}}
```
#### 在指定的路径下递归搜索要匹配的文件:
```shell
where /R {{目录的路径}} {{文件模式}}
```
#### 只返回退出代码，不显示匹配文件列表:
```shell
where /Q {{文件模式}}
```
{% endraw %}{% raw %}
<h2 id="whoami">
  <a href="/zh/windows/whoami.html">whoami</a> <a href="#whoami"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示有关当前用户的详细信息.

#### 显示当前用户的用户名:
```shell
whoami
```
#### 显示当前用户所属的组:
```shell
whoami /groups
```
#### 显示当前用户的权限:
```shell
whoami /priv
```
#### 显示当前用户的用户主体名称 (UPN):
```shell
whoami /upn
```
#### 显示当前用户的登录 id:
```shell
whoami /logonid
```
{% endraw %}{% raw %}
<h2 id="winget">
  <a href="/zh/windows/winget.html">winget</a> <a href="#winget"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Windows 软件包管理器命令行工具.
> 更多信息: <https://docs.microsoft.com/windows/package-manager/winget>.

#### 安装一个软件包:
```shell
winget install {{package}}
```
#### 显示关于一个软件包的信息:
```shell
winget show {{package}}
```
#### 查找一个软件包:
```shell
winget search {{package}}
```
{% endraw %}{% raw %}
<h2 id="wsl">
  <a href="/zh/windows/wsl.html">wsl</a> <a href="#wsl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 从命令行管理适用于 Linux 的 Windows 子系统.
> 更多信息: <https://docs.microsoft.com/windows/wsl/reference>.

#### 启动 Linux Shell（在默认发行版中）:
```shell
wsl {{shell_命令}}
```
#### 在不使用 Shell 的情况下运行 Linux 命令:
```shell
wsl --exec {{命令}} {{命令参数}}
```
#### 指定特定的发行版:
```shell
wsl --distribution {{发行版}} {{shell_命令}}
```
#### 列出所有可用发行版:
```shell
wsl --list
```
#### 将发行版导出到 .tar 文件:
```shell
wsl --export {{发行版}} {{路径/distro_fs.tar}}
```
#### 从 .tar 文件导入发行版:
```shell
wsl --import {{发行版}} {{路径/安装位置}} {{路径/distro_fs.tar}}
```
#### 更改指定发行版的版本:
```shell
wsl --set-version {{发行版}} {{版本}}
```
#### 关闭适用于 Linux 的 Windows 子系统:
```shell
wsl --shutdown
```
{% endraw %}{% raw %}
<h2 id="xcopy">
  <a href="/zh/windows/xcopy.html">xcopy</a> <a href="#xcopy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 复制文件和目录树.

#### 复制文件到指定的路径:
```shell
xcopy {{被复制的目录路径}} {{目标路径}}
```
#### 列出在复制前将要被复制的文件:
```shell
xcopy {{文件或目录的路径}} {{目标路径}} /p
```
#### 仅复制目录结构，不包括文件:
```shell
xcopy {{文件或目录的路径}} {{目标路径}} /t
```
#### 复制时包含空目录:
```shell
xcopy {{文件或目录的路径}} {{目标路径}} /e
```
#### 复制文件时保留 ACL 信息:
```shell
xcopy {{文件或目录的路径}} {{目标路径}} /o
```
#### 网络连接丢失时允许恢复:
```shell
xcopy {{文件或目录的路径}} {{目标路径}} /z
```
#### 当文件存在于目标路径中时禁用提示
```shell
xcopy {{文件或目录的路径}} {{目标路径}} /y
```
#### 显示详细的使用帮助:
```shell
xcopy /?
```
{% endraw %}