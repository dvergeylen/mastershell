---
layout: default
title: "windows"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#get-content">Get-Content</a>
* <a href="#assoc">assoc</a>
* <a href="#attrib">attrib</a>
* <a href="#azcopy">azcopy</a>
* <a href="#cd">cd</a>
* <a href="#chkdsk">chkdsk</a>
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
* <a href="#choco-apikey">choco-apikey</a>
* <a href="#choice">choice</a>
* <a href="#cinst">cinst</a>
* <a href="#cipher">cipher</a>
* <a href="#clip">clip</a>
* <a href="#clist">clist</a>
* <a href="#cls">cls</a>
* <a href="#cmd">cmd</a>
* <a href="#cmstp">cmstp</a>
* <a href="#color">color</a>
* <a href="#comp">comp</a>
* <a href="#cuninst">cuninst</a>
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
* <a href="#gpupdate">gpupdate</a>
* <a href="#ipconfig">ipconfig</a>
* <a href="#iscc">iscc</a>
* <a href="#logoff">logoff</a>
* <a href="#mkdir">mkdir</a>
* <a href="#mklink">mklink</a>
* <a href="#more">more</a>
* <a href="#mount">mount</a>
* <a href="#msg">msg</a>
* <a href="#nfsstat">nfsstat</a>
* <a href="#octo">octo</a>
* <a href="#path">path</a>
* <a href="#pathping">pathping</a>
* <a href="#popd">popd</a>
* <a href="#powershell">powershell</a>
* <a href="#print">print</a>
* <a href="#psping">psping</a>
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
* <a href="#replace">replace</a>
* <a href="#rmdir">rmdir</a>
* <a href="#robocopy">robocopy</a>
* <a href="#rpcinfo">rpcinfo</a>
* <a href="#scoop">scoop</a>
* <a href="#scoop-bucket">scoop bucket</a>
* <a href="#set">set</a>
* <a href="#sfc">sfc</a>
* <a href="#showmount">showmount</a>
* <a href="#shutdown">shutdown</a>
* <a href="#subst">subst</a>
* <a href="#systeminfo">systeminfo</a>
* <a href="#takeown">takeown</a>
* <a href="#taskkill">taskkill</a>
* <a href="#tasklist">tasklist</a>
* <a href="#title">title</a>
* <a href="#tree">tree</a>
* <a href="#tskill">tskill</a>
* <a href="#type">type</a>
* <a href="#tzutil">tzutil</a>
* <a href="#ver">ver</a>
* <a href="#virtualboxvm">virtualboxvm</a>
* <a href="#vol">vol</a>
* <a href="#where">where</a>
* <a href="#whoami">whoami</a>
* <a href="#winget">winget</a>
* <a href="#wmic">wmic</a>
* <a href="#wsl">wsl</a>
* <a href="#xcopy">xcopy</a>

{% raw %}
<h2 id="assoc">
  <a href="/en/windows/assoc.html">assoc</a> <a href="#assoc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display or modify file extension associations.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/assoc>.

#### Display all associated filetypes:
```shell
assoc
```
#### Display the associated filetype for a specific extension:
```shell
assoc {{.txt}}
```
#### Modify the associated filetype for a specific extension:
```shell
assoc {{.txt}}={{txtfile}}
```
{% endraw %}{% raw %}
<h2 id="attrib">
  <a href="/en/windows/attrib.html">attrib</a> <a href="#attrib"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Displays or changes file and directory attributes.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/attrib>.

#### Display the attributes of the files in the current directory:
```shell
attrib
```
#### Display the attributes of the files in the current directory and sub-directories:
```shell
attrib /S
```
#### Display the attributes of the files and directories in the current directory and sub-directories:
```shell
attrib /S /D
```
#### Add the read-only attribute to a file:
```shell
attrib +R {{document.txt}}
```
#### Remove the system and hidden attributes of a file:
```shell
attrib -S -H {{document.txt}}
```
#### Add the hidden attribute to a directory:
```shell
attrib +H {{path\to\directory}}
```
{% endraw %}{% raw %}
<h2 id="azcopy">
  <a href="/en/windows/azcopy.html">azcopy</a> <a href="#azcopy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A file transfer tool for uploading to Azure Cloud Storage Accounts.
> More information: <https://docs.microsoft.com/azure/storage/common/storage-use-azcopy-v10>.

#### Log in to an Azure Tenant:
```shell
azopy login
```
#### Upload a local file:
```shell
azcopy copy '{{path/to/source/file}}' 'https://{{storage_account_name}}.blob.core.windows.net/{{container_name}}/{{blob_name}}'
```
#### Upload files with `.txt` and `.jpg` extensions:
```shell
azcopy copy '{{path/to/source}}' 'https://{{storage_account_name}}.blob.core.windows.net/{{container_name}}' --include-pattern '{{*.txt;*.jpg}}'
```
#### Copy a container directly between two Azure storage accounts:
```shell
azcopy copy 'https://{{source_storage_account_name}}.blob.core.windows.net/{{container_name}}' 'https://{{destination_storage_account_name}}.blob.core.windows.net/{{container_name}}'
```
#### Synchronize a local directory and delete files in the destination if they no longer exist in the source:
```shell
azcopy sync '{{path/to/source}}' 'https://{{storage_account_name}}.blob.core.windows.net/{{container_name}}' --recursive --delete-destination=true
```
#### Display detailed usage information:
```shell
azcopy --help
```
{% endraw %}{% raw %}
<h2 id="cd">
  <a href="/en/windows/cd.html">cd</a> <a href="#cd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Displays the name of or changes the current working directory.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/cd>.

#### Go to a directory in the same drive:
```shell
cd {{path/to/directory}}
```
#### Display the name of the current directory:
```shell
cd
```
#### Go up to the parent of the current directory:
```shell
cd ..
```
#### Go to a directory in a different drive:
```shell
cd {{path/to/directory}} /d
```
{% endraw %}{% raw %}
<h2 id="chkdsk">
  <a href="/en/windows/chkdsk.html">chkdsk</a> <a href="#chkdsk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Check file system and volume metadata for errors.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/chkdsk>.

#### Specify the drive letter (followed by a colon), mount point, or volume name to check:
```shell
chkdsk {{volume}}
```
#### Fix errors on a specific volume:
```shell
chkdsk {{volume}} /f
```
#### Dismount a specific volume before checking:
```shell
chkdsk {{volume}} /x
```
#### Change the log file size to the specified size (only for NTFS):
```shell
chkdsk /l{{size}}
```
{% endraw %}{% raw %}
<h2 id="choco-apikey">
  <a href="/en/windows/choco-apikey.html">choco-apikey</a> <a href="#choco-apikey"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage API keys for Chocolatey sources.
> More information: <https://chocolatey.org/docs/commands-apikey>.

#### Display a list of sources and their API keys:
```shell
choco apikey
```
#### Display a specific source and its API key:
```shell
choco apikey --source "{{source_url}}"
```
#### Set an API key for a source:
```shell
choco apikey --source "{{source_url}}" --key "{{api_key}}"
```
#### Remove an API key for a source:
```shell
choco apikey --source "{{source_url}}" --remove
```
{% endraw %}{% raw %}
<h2 id="choco-feature">
  <a href="/en/windows/choco-feature.html">choco feature</a> <a href="#choco-feature"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interact with features with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-feature>.

#### Display a list of available features:
```shell
choco feature list
```
#### Enable a feature:
```shell
choco feature enable --name {{name}}
```
#### Disable a feature:
```shell
choco feature disable --name {{name}}
```
{% endraw %}{% raw %}
<h2 id="choco-info">
  <a href="/en/windows/choco-info.html">choco info</a> <a href="#choco-info"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display detailed information about a package with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-info>.

#### Display information on a specific package:
```shell
choco info {{package}}
```
#### Display information for a local package only:
```shell
choco info {{package}} --local-only
```
#### Specify a custom source to receive packages information from:
```shell
choco info {{package}} --source {{source_url|alias}}
```
#### Provide a username and password for authentication:
```shell
choco info {{package}} --user {{username}} --password {{password}}
```
{% endraw %}{% raw %}
<h2 id="choco-install">
  <a href="/en/windows/choco-install.html">choco install</a> <a href="#choco-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Install one or more packages with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-install>.

#### Install one or more space-separated packages:
```shell
choco install {{package(s)}}
```
#### Install packages from a custom configuration file:
```shell
choco install {{path/to/packages.config}}
```
#### Install a specific nuspec or nupkg file:
```shell
choco install {{path/to/file}}
```
#### Install a specific version of a package:
```shell
choco install {{package}} --version {{version}}
```
#### Allow installing multiple versions of a package:
```shell
choco install {{package}} --allow-multiple
```
#### Confirm all prompts automatically:
```shell
choco install {{package}} --yes
```
#### Specify a custom source to receive packages from:
```shell
choco install {{package}} --source {{source_url|alias}}
```
#### Provide a username and password for authentication:
```shell
choco install {{package}} --user {{username}} --password {{password}}
```
{% endraw %}{% raw %}
<h2 id="choco-list">
  <a href="/en/windows/choco-list.html">choco list</a> <a href="#choco-list"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display a list of packages with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-list>.

#### Display all available packages:
```shell
choco list
```
#### Display all locally installed packages:
```shell
choco list --local-only
```
#### Display a list including local programs:
```shell
choco list --include-programs
```
#### Display only approved packages:
```shell
choco list --approved-only
```
#### Specify a custom source to display packages from:
```shell
choco list --source {{source_url|alias}}
```
#### Provide a username and password for authentication:
```shell
choco list --user {{username}} --password {{password}}
```
{% endraw %}{% raw %}
<h2 id="choco-new">
  <a href="/en/windows/choco-new.html">choco new</a> <a href="#choco-new"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate new package specification files with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-new>.

#### Create a new package skeleton:
```shell
choco new {{package_name}}
```
#### Create a new package with a specific version:
```shell
choco new {{package_name}} --version {{version}}
```
#### Create a new package with a specific maintainer name:
```shell
choco new {{package_name}} --maintainer {{maintainer_name}}
```
#### Create a new package in a custom output directory:
```shell
choco new {{package_name}} --output-directory {{path/to/directory}}
```
#### Create a new package with specific 32-bit and 64-bit installer URLs:
```shell
choco new {{package_name}} url="{{url}}" url64="{{url}}"
```
{% endraw %}{% raw %}
<h2 id="choco-outdated">
  <a href="/en/windows/choco-outdated.html">choco outdated</a> <a href="#choco-outdated"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Check for outdated packages with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-outdated>.

#### Display a list of outdated packages in table format:
```shell
choco outdated
```
#### Ignore pinned packages in the output:
```shell
choco outdated --ignore-pinned
```
#### Specify a custom source to check packages from:
```shell
choco outdated --source {{source_url|alias}}
```
#### Provide a username and password for authentication:
```shell
choco outdated --user {{username}} --password {{password}}
```
{% endraw %}{% raw %}
<h2 id="choco-pack">
  <a href="/en/windows/choco-pack.html">choco pack</a> <a href="#choco-pack"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Package a NuGet specification into a nupkg file.
> More information: <https://chocolatey.org/docs/commands-pack>.

#### Package a NuGet specification to a nupkg file:
```shell
choco pack {{path/to/specification}}
```
#### Package a NuGet specification specifying the version of the resulting file:
```shell
choco pack {{path/to/specification}} --version {{version}}
```
#### Package a NuGet specification to a specific directory:
```shell
choco pack {{path/to/specification}} --output-directory {{path/to/output_directory}}
```
{% endraw %}{% raw %}
<h2 id="choco-pin">
  <a href="/en/windows/choco-pin.html">choco pin</a> <a href="#choco-pin"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pin a package at a specific version with Chocolatey.
> Pinned packages are skipped automatically when upgrading.
> More information: <https://chocolatey.org/docs/commands-pin>.

#### Display a list of pinned packages and their versions:
```shell
choco pin list
```
#### Pin a package at its current version:
```shell
choco pin add --name {{package}}
```
#### Pin a package at a specific version:
```shell
choco pin add --name {{package}} --version {{version}}
```
#### Remove a pin for a specific package:
```shell
choco pin remove --name {{package}}
```
{% endraw %}{% raw %}
<h2 id="choco-search">
  <a href="/en/windows/choco-search.html">choco search</a> <a href="#choco-search"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Search for a local or remote package with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-search>.

#### Search for a package:
```shell
choco search {{query}}
```
#### Search for a package locally:
```shell
choco search {{query}} --local-only
```
#### Only include exact matches in the results:
```shell
choco search {{query}} --exact
```
#### Confirm all prompts automatically:
```shell
choco search {{query}} --yes
```
#### Specify a custom source to search for packages in:
```shell
choco search {{query}} --source {{source_url|alias}}
```
#### Provide a username and password for authentication:
```shell
choco search {{query}} --user {{username}} --password {{password}}
```
{% endraw %}{% raw %}
<h2 id="choco-source">
  <a href="/en/windows/choco-source.html">choco source</a> <a href="#choco-source"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage sources for packages with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-source>.

#### List currently available sources:
```shell
choco source list
```
#### Add a new package source:
```shell
choco source add --name {{name}} --source {{url}}
```
#### Add a new package source with credentials:
```shell
choco source add --name {{name}} --source {{url}} --user {{username}} --password {{password}}
```
#### Add a new package source with a client certificate:
```shell
choco source add --name {{name}} --source {{url}} --cert {{path/to/certificate}}
```
#### Enable a package source:
```shell
choco source enable --name {{name}}
```
#### Disable a package source:
```shell
choco source disable --name {{name}}
```
#### Remove a package source:
```shell
choco source remove --name {{name}}
```
{% endraw %}{% raw %}
<h2 id="choco-uninstall">
  <a href="/en/windows/choco-uninstall.html">choco uninstall</a> <a href="#choco-uninstall"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Uninstall one or more packages with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-uninstall>.

#### Uninstall one or more space-separated packages:
```shell
choco uninstall {{package(s)}}
```
#### Uninstall a specific version of a package:
```shell
choco uninstall {{package}} --version {{version}}
```
#### Confirm all prompts automatically:
```shell
choco uninstall {{package}} --yes
```
#### Remove all dependencies when uninstalling:
```shell
choco uninstall {{package}} --remove-dependencies
```
#### Uninstall all packages:
```shell
choco uninstall all
```
{% endraw %}{% raw %}
<h2 id="choco-upgrade">
  <a href="/en/windows/choco-upgrade.html">choco upgrade</a> <a href="#choco-upgrade"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Upgrade one or more packages with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-upgrade>.

#### Upgrade one or more space-separated packages:
```shell
choco upgrade {{package(s)}}
```
#### Upgrade to a specific version of a package:
```shell
choco upgrade {{package}} --version {{version}}
```
#### Upgrade all packages:
```shell
choco upgrade all
```
#### Upgrade all except specified comma-separated packages:
```shell
choco upgrade all --except "{{package(s)}}"
```
#### Confirm all prompts automatically:
```shell
choco upgrade {{package}} --yes
```
#### Specify a custom source to receive packages from:
```shell
choco upgrade {{package}} --source {{source_url|alias}}
```
#### Provide a username and password for authentication:
```shell
choco upgrade {{package}} --user {{username}} --password {{password}}
```
{% endraw %}{% raw %}
<h2 id="choco">
  <a href="/en/windows/choco.html">choco</a> <a href="#choco"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line interface for the Chocolatey package manager.
> See `choco install`, `choco upgrade` and other pages for additional information.
> More information: <https://chocolatey.org>.

#### Execute Chocolatey command:
```shell
choco {{command}}
```
#### Call general help:
```shell
choco -?
```
#### Call help on a specific command:
```shell
choco {{command}} -?
```
#### Check the Chocolatey version:
```shell
choco --version
```
{% endraw %}{% raw %}
<h2 id="choice">
  <a href="/en/windows/choice.html">choice</a> <a href="#choice"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Prompts the user to select one item from a list of single-character choices in a batch program, and then returns the index of the selected choice.
> If used without parameters, choice displays the default choices Y and N.
> More information: <https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/choice>.

#### A,B and C as list of choices to be used:
```shell
choice /c {{ABC}}
```
#### Use the default [Y,N] list of choices:
```shell
choice
```
#### Specify that the choices are case-sensitive:
```shell
choice /CS {{AaBb}}
```
#### Specify the number of seconds to pause before using the default choice specified by `/d`:
```shell
choice /C {{AaBb}} /t {{3}} /d {{b}}
```
#### Specify a message to display before the list of choices. If `/m` is not specified, only the choice prompt is displayed:
```shell
choice /m {{message}} /C {{ABC}}
```
#### Display help message:
```shell
choice /?
```
{% endraw %}{% raw %}
<h2 id="cinst">
  <a href="/en/windows/cinst.html">cinst</a> <a href="#cinst"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> This command is an alias of `choco install`.

#### View documentation for the original command:
```shell
tldr choco install
```
{% endraw %}{% raw %}
<h2 id="cipher">
  <a href="/en/windows/cipher.html">cipher</a> <a href="#cipher"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Encrypt or decrypt files on NTFS drives.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/cipher>.

#### Encrypt a file or directory:
```shell
cipher /e:{{path/to/file_or_directory}}
```
#### Decrypt a file or directory:
```shell
cipher /d:{{path/to/file_or_directory}}
```
#### Securely remove a file or directory:
```shell
cipher /w:{{path/to/file_or_directory}}
```
{% endraw %}{% raw %}
<h2 id="clip">
  <a href="/en/windows/clip.html">clip</a> <a href="#clip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copy input content to the Windows clipboard.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/clip>.

#### Pipe command-line output to the Windows clipboard:
```shell
{{dir}} | clip
```
#### Copy the contents of a file to the Windows clipboard:
```shell
clip < {{path/to/file.ext}}
```
#### Copy text with a trailing newline to the Windows clipboard:
```shell
echo {{some text}} | clip
```
#### Copy text without a trailing newline to the Windows clipboard:
```shell
echo | set /p="some text" | clip
```
{% endraw %}{% raw %}
<h2 id="clist">
  <a href="/en/windows/clist.html">clist</a> <a href="#clist"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> This command is an alias of `choco list`.

#### View documentation for the original command:
```shell
tldr choco list
```
{% endraw %}{% raw %}
<h2 id="cls">
  <a href="/en/windows/cls.html">cls</a> <a href="#cls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Clears the screen.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/cls>.

#### Clear the screen:
```shell
cls
```
{% endraw %}{% raw %}
<h2 id="cmd">
  <a href="/en/windows/cmd.html">cmd</a> <a href="#cmd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Windows command interpreter.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/cmd>.

#### Start a new instance of the command interpreter:
```shell
cmd
```
#### Run the specified command and then exit:
```shell
cmd /c "{{command}}"
```
#### Run the specified command and then enter an interactive shell:
```shell
cmd /k "{{command}}"
```
#### Disable the usage of `echo` in command output:
```shell
cmd /q
```
#### Enable or disable command extensions:
```shell
cmd /e:{{on|off}}
```
#### Enable or disable file or directory autocompletion:
```shell
cmd /f:{{on|off}}
```
#### Enable or disable environment variable expansion:
```shell
cmd /v:{{on|off}}
```
#### Force output to use Unicode encoding:
```shell
cmd /u
```
{% endraw %}{% raw %}
<h2 id="cmstp">
  <a href="/en/windows/cmstp.html">cmstp</a> <a href="#cmstp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line tool for managing connection service profiles.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/cmstp>.

#### Install a specific profile:
```shell
cmstp "{{path/to/profile}}"
```
#### Install without creating a desktop shortcut:
```shell
cmstp /ns "{{path/to/profile}}"
```
#### Install without checking for dependencies:
```shell
cmstp /nf "{{path/to/profile}}"
```
#### Only install for the current user:
```shell
cmstp /su "{{path/to/profile}}"
```
#### Install for all users (requires administrator privileges):
```shell
cmstp /au "{{path/to/profile}}"
```
#### Install silently without any prompts:
```shell
cmstp /s "{{path/to/profile}}"
```
#### Uninstall a specific profile:
```shell
cmstp /u "{{path/to/profile}}"
```
#### Uninstall silently without a confirmation prompt:
```shell
cmstp /u /s "{{path/to/profile}}"
```
{% endraw %}{% raw %}
<h2 id="color">
  <a href="/en/windows/color.html">color</a> <a href="#color"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set the console foreground and background colors.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/color>.

#### Set the console colors to the default values:
```shell
color
```
#### List available color values and detailed information:
```shell
color /?
```
#### Set the console foreground and background to a specific color:
```shell
color {{foreground_code}}{{background_code}}
```
{% endraw %}{% raw %}
<h2 id="comp">
  <a href="/en/windows/comp.html">comp</a> <a href="#comp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compare the contents of two files or sets of files.
> Use wildcards (*) to compare sets of files.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/comp>.

#### Compare files interactively:
```shell
comp
```
#### Compare two specified files:
```shell
comp {{path/to/file_1}} {{path/to/file_2}}
```
#### Compare two sets of files:
```shell
comp {{path/to/directory_1/*}} {{path/to/directory_2/*}}
```
#### Display differences in decimal format:
```shell
comp /d {{path/to/file_1}} {{path/to/file_2}}
```
#### Display differences in ASCII format:
```shell
comp /a {{path/to/file_1}} {{path/to/file_2}}
```
#### Display line numbers for differences:
```shell
comp /l {{path/to/file_1}} {{path/to/file_2}}
```
#### Compare files case-insensitively:
```shell
comp /c {{path/to/file_1}} {{path/to/file_2}}
```
#### Compare only the first 5 lines of each file:
```shell
comp /n={{5}} {{path/to/file_1}} {{path/to/file_2}}
```
{% endraw %}{% raw %}
<h2 id="cuninst">
  <a href="/en/windows/cuninst.html">cuninst</a> <a href="#cuninst"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> This command is an alias of `choco uninstall`.

#### View documentation for the original command:
```shell
tldr choco uninstall
```
{% endraw %}{% raw %}
<h2 id="del">
  <a href="/en/windows/del.html">del</a> <a href="#del"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Delete one or more files.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/del>.

#### Delete one or more space-separated files or patterns:
```shell
del {{file_pattern}}
```
#### Prompt for confirmation before deleting each file:
```shell
del {{file_pattern}} /p
```
#### Force the deletion of read-only files:
```shell
del {{file_pattern}} /f
```
#### Recursively delete file(s) from all subdirectories:
```shell
del {{file_pattern}} /s
```
#### Do not prompt when deleting files based on a global wildcard:
```shell
del {{file_pattern}} /q
```
#### Display the help and list available attributes:
```shell
del /?
```
#### Delete files based on specified attributes:
```shell
del {{file_pattern}} /a {{attribute}}
```
{% endraw %}{% raw %}
<h2 id="dir">
  <a href="/en/windows/dir.html">dir</a> <a href="#dir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List directory contents.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/dir>.

#### Show the contents of the current directory:
```shell
dir
```
#### Show the contents of a given directory:
```shell
dir {{path/to/directory}}
```
#### Show the contents of the current directory, including hidden ones:
```shell
dir /A
```
#### Show the contents of a given directory, including hidden ones:
```shell
dir {{path/to/directory}} /A
```
{% endraw %}{% raw %}
<h2 id="doskey">
  <a href="/en/windows/doskey.html">doskey</a> <a href="#doskey"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage macros, windows commands and command-lines.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/doskey>.

#### List available macros:
```shell
doskey /macros
```
#### Create a new macro:
```shell
doskey {{name}} = "{{command}}"
```
#### Create a new macro for a specific executable:
```shell
doskey /exename={{executable}} {{name}} = "{{command}}"
```
#### Remove a macro:
```shell
doskey {{name}} =
```
#### Display all commands that are stored in memory:
```shell
doskey /history
```
#### Save macros to a file for portability:
```shell
doskey /macros > {{macinit}}
```
#### Load macros from a file:
```shell
doskey /macrofile = {{macinit}}
```
{% endraw %}{% raw %}
<h2 id="driverquery">
  <a href="/en/windows/driverquery.html">driverquery</a> <a href="#driverquery"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about installed device drivers.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/driverquery>.

#### Display a list of all installed device drivers:
```shell
driverquery
```
#### Display a list of drivers in the specified format:
```shell
driverquery /fo {{table|list|csv}}
```
#### Display a list of drivers with a column to indicate if they are signed:
```shell
driverquery /si
```
#### Exclude the header in the output list:
```shell
driverquery /nh
```
#### Display a list of drivers for a remote machine:
```shell
driverquery /s {{hostname}} /u {{username}} /p {{password}}
```
#### Display a list of drivers with verbose information:
```shell
driverquery /v
```
#### Display detailed usage information:
```shell
driverquery /?
```
{% endraw %}{% raw %}
<h2 id="eventcreate">
  <a href="/en/windows/eventcreate.html">eventcreate</a> <a href="#eventcreate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create custom entries in the event log.
> Event IDs can be any number between 1 and 1000.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/eventcreate>.

#### Create a new event with a given id (1-1000) in the log:
```shell
eventcreate /t {{success|error|warning|information}} /id {{id}} /d "{{message}}"
```
#### Create an event in a specific event log:
```shell
eventcreate /l {{log_name}} /t {{type}} /id {{id}} /d "{{message}}"
```
#### Create an event with a specific source:
```shell
eventcreate /so {{source_name}} /t {{type}} /id {{id}} /d "{{message}}"
```
#### Create an event in a remote machine's event log:
```shell
eventcreate /s {{hostname}} /u {{username}} /p {{password}} /t {{type}} /id {{id}} /d "{{message}}"
```
{% endraw %}{% raw %}
<h2 id="exit">
  <a href="/en/windows/exit.html">exit</a> <a href="#exit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Quit the current CMD instance or the current batch file.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/exit>.

#### Quit the current CMD instance:
```shell
exit
```
#### Quit the current batch script:
```shell
exit /b
```
#### Quit using a specific exit code:
```shell
exit {{exit_code}}
```
{% endraw %}{% raw %}
<h2 id="expand">
  <a href="/en/windows/expand.html">expand</a> <a href="#expand"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Uncompress one or more Windows Cabinet files.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/expand>.

#### Uncompress a single-file Cabinet file to the specified directory:
```shell
expand {{path/to/file.cab}} {{path/to/directory}}
```
#### Display the list of files in a source Cabinet file:
```shell
expand {{path/to/file.cab}} {{path/to/directory}} -d
```
#### Uncompress all files from the Cabinet file:
```shell
expand {{path/to/file.cab}} {{path/to/directory}} -f:*
```
#### Uncompress a specific file from a Cabinet file:
```shell
expand {{path/to/file.cab}} {{path/to/directory}} -f:{{file}}
```
#### Ignore the directory structure when uncompressing, and add them to a single directory:
```shell
expand {{path/to/file.cab}} {{path/to/directory}} -i
```
{% endraw %}{% raw %}
<h2 id="explorer">
  <a href="/en/windows/explorer.html">explorer</a> <a href="#explorer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Windows File Explorer.
> More information: <https://ss64.com/nt/explorer.html>.

#### Open Windows Explorer:
```shell
explorer
```
#### Open Windows Explorer in the current directory:
```shell
explorer .
```
#### Open Windows Explorer in a specific directory:
```shell
explorer {{path/to/directory}}
```
{% endraw %}{% raw %}
<h2 id="fc">
  <a href="/en/windows/fc.html">fc</a> <a href="#fc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compare the differences between two files or sets of files.
> Use wildcards (*) to compare sets of files.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/fc>.

#### Compare 2 specified files:
```shell
fc {{path/to/file_1}} {{path/to/file_2}}
```
#### Perform a case-insensitive comparison:
```shell
fc /c {{path/to/file_1}} {{path/to/file_2}}
```
#### Compare files as Unicode text:
```shell
fc /u {{path/to/file_1}} {{path/to/file_2}}
```
#### Compare files as ASCII text:
```shell
fc /l {{path/to/file_1}} {{path/to/file_2}}
```
#### Compare files as binary:
```shell
fc /b {{path/to/file_1}} {{path/to/file_2}}
```
#### Disable tab-to-space expansion:
```shell
fc /t {{path/to/file_1}} {{path/to/file_2}}
```
#### Compress whitespace (tabs and spaces) for comparisons:
```shell
fc /w {{path/to/file_1}} {{path/to/file_2}}
```
{% endraw %}{% raw %}
<h2 id="find">
  <a href="/en/windows/find.html">find</a> <a href="#find"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Find a specified string in one or more files.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/find>.

#### Find lines that contain a specified string:
```shell
find {{string}} {{path/to/file_or_directory}}
```
#### Display lines that do not contain the specified string:
```shell
find {{string}} {{path/to/file_or_directory}} /v
```
#### Display the count of lines that contain the specified string:
```shell
find {{string}} {{path/to/file_or_directory}} /c
```
#### Display line numbers with the list of lines:
```shell
find {{string}} {{path/to/file_or_directory}} /n
```
{% endraw %}{% raw %}
<h2 id="findstr">
  <a href="/en/windows/findstr.html">findstr</a> <a href="#findstr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Find specified text within one or more files.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/findstr>.

#### Find space-separated string(s) in all files:
```shell
findstr "{{query}}" *
```
#### Find space-separated string(s) in a piped command's output:
```shell
{{dir}} | findstr "{{query}}"
```
#### Find space-separated string(s) in all files recur[s]ively:
```shell
findstr /s "{{query}}" *
```
#### Find strings using a case-insensitive search:
```shell
findstr /i "{{query}}" *"
```
#### Find strings in all files using regular expressions:
```shell
findstr /r "{{expression}}" *
```
#### Find a literal string (containing spaces) in all text files:
```shell
findstr /c:"{{query}}" *.txt
```
#### Display the line number before each matching line:
```shell
findstr /n "{{query}}" *
```
#### Display only the filenames that contain a match:
```shell
findstr /m "{{query}}" *
```
{% endraw %}{% raw %}
<h2 id="finger">
  <a href="/en/windows/finger.html">finger</a> <a href="#finger"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Return information about one or more users on a specified system.
> The remote system must be running the Finger service.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/finger>.

#### Display information about a specific user:
```shell
finger {{user}}@{{host}}
```
#### Display information about all users on the specified host:
```shell
finger @{{host}}
```
#### Display information in a longer format:
```shell
finger {{user}}@{{host}} -l
```
#### Display help information:
```shell
finger /?
```
{% endraw %}{% raw %}
<h2 id="fondue">
  <a href="/en/windows/fondue.html">fondue</a> <a href="#fondue"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line installer for optional Windows features.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/fondue>.

#### Enable a specific Windows feature:
```shell
fondue /enable-feature:{{feature}}
```
#### Hide all output messages to the user:
```shell
fondue /enable-feature:{{feature}} /hide-ux:all
```
#### Specify a caller process name for error reporting:
```shell
fondue /enable-feature:{{feature}} /caller-name:{{name}}
```
{% endraw %}{% raw %}
<h2 id="forfiles">
  <a href="/en/windows/forfiles.html">forfiles</a> <a href="#forfiles"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Select one or more files to execute a specified command on.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/forfiles>.

#### Search for files in the current directory:
```shell
forfiles
```
#### Search for files in a specific directory:
```shell
forfiles /p {{path/to/directory}}
```
#### Run the specified command for each file:
```shell
forfiles /c "{{command}}"
```
#### Search for files using a specific glob mask:
```shell
forfiles /m {{glob_pattern}}
```
#### Search for files recursively:
```shell
forfiles /s
```
#### Search for files older than 5 days:
```shell
forfiles /d {{+5}}
```
{% endraw %}{% raw %}
<h2 id="ftp">
  <a href="/en/windows/ftp.html">ftp</a> <a href="#ftp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interactively transfer files between a local and remote FTP server.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/ftp>.

#### Connect to a remote FTP server interactively:
```shell
ftp {{host}}
```
#### Log in as an anonymous user:
```shell
ftp -A {{host}}
```
#### Disable automatic login upon initial connection:
```shell
ftp -n {{host}}
```
#### Run a file containing a list of FTP commands:
```shell
ftp -s:{{path/to/file}} {{host}}
```
#### Download multiple files (glob expression):
```shell
mget {{*.png}}
```
#### Upload multiple files (glob expression):
```shell
mput {{*.zip}}
```
#### Delete multiple files on the remote server:
```shell
mdelete {{*.txt}}
```
#### Display detailed help:
```shell
ftp --help
```
{% endraw %}{% raw %}
<h2 id="ftype">
  <a href="/en/windows/ftype.html">ftype</a> <a href="#ftype"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display or modify file types used for file extension association.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/ftype>.

#### Display a list of all file types:
```shell
ftype
```
#### Display the associated program for a specific file type:
```shell
ftype {{file_type}}
```
#### Set the associated program for a specific file type:
```shell
ftype {{file_type}}="{{path/to/executable_command}}"
```
{% endraw %}{% raw %}
<h2 id="get-content">
  <a href="/en/windows/get-content.html">Get-Content</a> <a href="#get-content"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get the content of the item at the specified location.
> More information: <https://docs.microsoft.com/powershell/module/microsoft.powershell.management/get-content>.

#### Display the content of a file:
```shell
Get-Content -Path {{path/to/file}}
```
#### Display the first few lines of a file:
```shell
Get-Content -Path {{path/to/file}} -TotalCount {{count}}
```
#### Display the content of the file and keep reading from it until `Ctrl + C` is pressed:
```shell
Get-Content -Path {{path/to/file}} -Wait
```
{% endraw %}{% raw %}
<h2 id="getmac">
  <a href="/en/windows/getmac.html">getmac</a> <a href="#getmac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the MAC addresses of a system.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/getmac>.

#### Display the MAC addresses for the current system:
```shell
getmac
```
#### Display the details in a specific format:
```shell
getmac /fo {{table|list|csv}}
```
#### Exclude the header in the output list:
```shell
getmac /nh
```
#### Display the MAC addresses for a remote machine:
```shell
getmac /s {{hostname}} /u {{username}} /p {{password}}
```
#### Display the MAC addresses with verbose information:
```shell
getmac /v
```
#### Display detailed usage information:
```shell
getmac /?
```
{% endraw %}{% raw %}
<h2 id="gpupdate">
  <a href="/en/windows/gpupdate.html">gpupdate</a> <a href="#gpupdate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to check and apply Windows Group Policy settings.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/gpupdate>.

#### Check and apply updated Group Policy settings:
```shell
gpupdate
```
#### Specify the target Group Policy settings to check for update:
```shell
gpupdate /target=:{{computer|user}}
```
#### Force all Group Policy settings to be reapplied:
```shell
gpupdate /force
```
#### Display detailed usage information:
```shell
gpupdate /?
```
{% endraw %}{% raw %}
<h2 id="ipconfig">
  <a href="/en/windows/ipconfig.html">ipconfig</a> <a href="#ipconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display and manage the network configuration of Windows.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/ipconfig>.

#### Show a list of network adapters:
```shell
ipconfig
```
#### Show a detailed list of network adapters:
```shell
ipconfig /all
```
#### Renew the IP addresses for a network adapter:
```shell
ipconfig /renew {{adapter}}
```
#### Free up the IP addresses for a network adapter:
```shell
ipconfig /release {{adapter}}
```
#### Remove all data from the DNS cache:
```shell
ipconfig /flushdns
```
{% endraw %}{% raw %}
<h2 id="iscc">
  <a href="/en/windows/iscc.html">iscc</a> <a href="#iscc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compiler for Inno Setup installers.
> It compiles an Inno Setup scripts into an Windows installer executable.
> More information: <https://jrsoftware.org/isinfo.php>.

#### Compile an Inno Setup script:
```shell
iscc {{path/to/file.iss}}
```
#### Quietly compile an Inno Setup installer:
```shell
iscc /Q {{path/to/file.iss}}
```
#### Compile a signed Inno Setup installer:
```shell
iscc /S={{name}}={{command}} {{path/to/file.iss}}
```
{% endraw %}{% raw %}
<h2 id="logoff">
  <a href="/en/windows/logoff.html">logoff</a> <a href="#logoff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Terminate a login session.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/logoff>.

#### Terminate the current session:
```shell
logoff
```
#### Terminate a session by its name or id:
```shell
logoff {{session_name|session_id}}
```
#### Terminate a session on a specific server connected through RDP:
```shell
logoff {{session_name|session_id}} /server:{{servername}}
```
{% endraw %}{% raw %}
<h2 id="mkdir">
  <a href="/en/windows/mkdir.html">mkdir</a> <a href="#mkdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates a directory.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/mkdir>.

#### Create a directory:
```shell
mkdir {{directory_name}}
```
#### Recursively create a nested directory tree:
```shell
mkdir {{path/to/sub_directory_name}}
```
{% endraw %}{% raw %}
<h2 id="mklink">
  <a href="/en/windows/mklink.html">mklink</a> <a href="#mklink"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create symbolic links.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/mklink>.

#### Create a symbolic link to a file:
```shell
mklink {{path/to/link}} {{path/to/source_file}}
```
#### Create a symbolic link to a directory:
```shell
mklink /d {{path/to/link}} {{path/to/source_directory}}
```
#### Create a hard link to a file:
```shell
mklink /h {{path/to/link}} {{path/to/source_file}}
```
#### Create a directory junction:
```shell
mklink /j {{path/to/link}} {{path/to/source_file}}
```
{% endraw %}{% raw %}
<h2 id="more">
  <a href="/en/windows/more.html">more</a> <a href="#more"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display paginated output from stdin or a file.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/more>.

#### Display paginated output from stdin:
```shell
{{echo test}} | more
```
#### Display paginated output from one or more files:
```shell
more {{path/to/file}}
```
#### Convert tabs to the specified number of spaces:
```shell
more {{path/to/file}} /t{{spaces}}
```
#### Clear the screen before displaying the page:
```shell
more {{path/to/file}} /c
```
#### Display the output starting at line 5:
```shell
more {{path/to/file}} +{{5}}
```
#### Enable extended interactive mode (see help for usage):
```shell
more {{path/to/file}} /e
```
#### Display full usage information:
```shell
more /?
```
{% endraw %}{% raw %}
<h2 id="mount">
  <a href="/en/windows/mount.html">mount</a> <a href="#mount"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mount Network File System (NFS) network shares.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/mount>.

#### Mount a share to the "Z" drive letter:
```shell
mount \\{{computer_name}}\{{share_name}} {{Z:}}
```
#### Mount a share to the next available drive letter:
```shell
mount \\{{computer_name}}\{{share_name}} *
```
#### Mount a share with a read timeout in seconds (defaults to 0.8, can be 0.9 or 1 to 60):
```shell
mount -o timeout={{seconds}} \\{{computer_name}}\{{share_name}} {{Z:}}
```
#### Mount a share and retry up to 10 times if it fails:
```shell
mount -o retry={{retries}} \\{{computer_name}}\{{share_name}} {{Z:}}
```
#### Mount a share with forced case sensitivity:
```shell
mount -o casesensitive \\{{computer_name}}\{{share_name}} {{Z:}}
```
#### Mount a share as an anonymous user:
```shell
mount -o anon \\{{computer_name}}\{{share_name}} {{Z:}}
```
#### Mount a share using a specific mount type:
```shell
mount -o mtype={{soft|hard}} \\{{computer_name}}\{{share_name}} {{Z:}}
```
{% endraw %}{% raw %}
<h2 id="msg">
  <a href="/en/windows/msg.html">msg</a> <a href="#msg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Send a message to a specific user or session.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/msg>.

#### Send a message to a specified user or session:
```shell
msg {{username|session_name|session_id}} {{message}}
```
#### Send a message from stdin:
```shell
echo "{{message}}" | msg {{username|session_name|session_id}}
```
#### Send a message to a specific server:
```shell
msg /server:{{server_name}} {{username|session_name|session_id}}
```
#### Send a message to all users of the current machine:
```shell
msg *
```
#### Set a delay in seconds for a message:
```shell
msg /time:{{seconds}}
```
{% endraw %}{% raw %}
<h2 id="nfsstat">
  <a href="/en/windows/nfsstat.html">nfsstat</a> <a href="#nfsstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display or reset the number of calls made to the NFS server.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/nfsstat>.

#### Display the recorded number of calls made to the NFS server:
```shell
nfsstat
```
#### Reset the recorded number of calls made to the NFS server:
```shell
nfsstat -z
```
{% endraw %}{% raw %}
<h2 id="octo">
  <a href="/en/windows/octo.html">octo</a> <a href="#octo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line tools for Octopus Deploy.
> More information: <https://octopus.com/docs/octopus-rest-api/octo.exe-command-line>.

#### Create a package:
```shell
octo pack --id={{package_name}}
```
#### Push a package to a repository on the Octopus server:
```shell
octo push --package={{package_name}}
```
#### Create a release:
```shell
octo create-release --project={{project_name}} --packageversion={{version}}
```
#### Deploy a release:
```shell
octo deploy-release --project={{project_name}} --packageversion={{version}} --deployto={{environment_name}} --tenant={{deployment_target}}
```
{% endraw %}{% raw %}
<h2 id="path">
  <a href="/en/windows/path.html">path</a> <a href="#path"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display or set the search path for executable files.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/path>.

#### Display the current path:
```shell
path
```
#### Set the path to one or more semicolon-separated directories:
```shell
path {{path/to/directory(s)}}
```
#### Append a new directory to the original path:
```shell
path {{path/to/directory}};%path%
```
#### Set command prompt to only search the current directory for executables:
```shell
path ;
```
{% endraw %}{% raw %}
<h2 id="pathping">
  <a href="/en/windows/pathping.html">pathping</a> <a href="#pathping"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A trace route tool combining features of `ping` and `tracert`.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/pathping>.

#### Ping and trace the route to a host:
```shell
pathping {{hostname}}
```
#### Do not perform reverse lookup of ip-address to hostname:
```shell
pathping {{hostname}} -n
```
#### Specify the maximum number of hops to search for the target (the default is 30):
```shell
pathping {{hostname}} -h {{max_hops}}
```
#### Specify the milliseconds to wait between pings (the default is 240):
```shell
pathping {{hostname}} -p {{time}}
```
#### Specify the number of queries per hop (the default is 100):
```shell
pathping {{hostname}} -q {{queries}}
```
#### Force IPV4 usage:
```shell
pathping {{hostname}} -4
```
#### Force IPV6 usage:
```shell
pathping {{hostname}} -6
```
#### Display detailed usage information:
```shell
pathping /?
```
{% endraw %}{% raw %}
<h2 id="popd">
  <a href="/en/windows/popd.html">popd</a> <a href="#popd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Changes the current directory to the directory stored by the `pushd` command.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/popd>.

#### Switch to directory at the top of the stack:
```shell
popd
```
{% endraw %}{% raw %}
<h2 id="powershell">
  <a href="/en/windows/powershell.html">powershell</a> <a href="#powershell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line shell and scripting language designed especially for system administration.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/powershell>.

#### Start a Windows PowerShell session in a Command Prompt window:
```shell
powershell
```
#### Load a specific PowerShell console file:
```shell
powershell -PSConsoleFile {{path/to/file}}
```
#### Start a session with a specified version of PowerShell:
```shell
powershell -Version {{version}}
```
#### Prevent the shell from exit after running startup commands:
```shell
powershell -NoExit
```
#### Describe the format of data sent to PowerShell:
```shell
powershell -InputFormat {{Text|XML}}
```
#### Determine how output from PowerShell is formatted:
```shell
powershell -OutputFormat {{Text|XML}}
```
#### Display help:
```shell
powershell -Help
```
{% endraw %}{% raw %}
<h2 id="print">
  <a href="/en/windows/print.html">print</a> <a href="#print"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print a text file to a printer.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/print>.

#### Print a text file to the default printer:
```shell
print {{path/to/file}}
```
#### Print a text file to a specific printer:
```shell
print /d:{{printer}} {{path/to/file}}
```
{% endraw %}{% raw %}
<h2 id="psping">
  <a href="/en/windows/psping.html">psping</a> <a href="#psping"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A ping tool that includes TCP ping, latency and bandwidth measurement.
> More information: <https://docs.microsoft.com/sysinternals/downloads/psping>.

#### Ping a host using ICMP:
```shell
psping {{hostname}}
```
#### Ping a host over a TCP port:
```shell
psping {{hostname}}:{{port}}
```
#### Specify the number of pings and perform it quietly:
```shell
psping {{hostname}} -n {{pings}} -q
```
#### Ping the target over TCP 50 times and produce a histogram of the results:
```shell
psping {{hostname}}:{{port}} -q -n {{50}} -h
```
#### Display usage information:
```shell
psping /?
```
{% endraw %}{% raw %}
<h2 id="pushd">
  <a href="/en/windows/pushd.html">pushd</a> <a href="#pushd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Place a directory on a stack so it can be accessed later.
> See also `popd` to switch back to original directory.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/pushd>.

#### Switch to directory and push it on the stack:
```shell
pushd {{directory}}
```
{% endraw %}{% raw %}
<h2 id="pwlauncher">
  <a href="/en/windows/pwlauncher.html">pwlauncher</a> <a href="#pwlauncher"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line tool for managing the Windows To Go startup options.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/pwlauncher>.

#### Display the current Windows To Go status:
```shell
pwlauncher
```
#### Enable or disable the Windows To Go startup options:
```shell
pwlauncher /{{enable|disable}}
```
{% endraw %}{% raw %}
<h2 id="rdpsign">
  <a href="/en/windows/rdpsign.html">rdpsign</a> <a href="#rdpsign"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool for signing Remote Desktop Protocol (RDP) files.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/rdpsign>.

#### Sign an RDP file:
```shell
rdpsign {{path/to/file.rdp}}
```
#### Sign an RDP file using a specific sha256 hash:
```shell
rdpsign {{path/to/file.rdp}} /sha265 {{hash}}
```
#### Enable quiet output:
```shell
rdpsign {{path/to/file.rdp}} /q
```
#### Display verbose warnings, messages and statuses:
```shell
rdpsign {{path/to/file.rdp}} /v
```
#### Test the signing by displaying the output to stdout without updating the file:
```shell
rdpsign {{path/to/file.rdp}} /l
```
{% endraw %}{% raw %}
<h2 id="reg-add">
  <a href="/en/windows/reg-add.html">reg add</a> <a href="#reg-add"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Add new keys and their values to the registry.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-add>.

#### Add a new registry key:
```shell
reg add {{key_name}}
```
#### Add a new value under a specific key:
```shell
reg add {{key_name}} /v {{value}}
```
#### Add a new value with specific data:
```shell
reg add {{key_name}} /d {{data}}
```
#### Add a new value to a key with a specific data type:
```shell
reg add {{key_name}} /t {{type}}
```
#### Forcefully overwrite the existing registry value without a prompt:
```shell
reg add {{key_name}} /f
```
{% endraw %}{% raw %}
<h2 id="reg-compare">
  <a href="/en/windows/reg-compare.html">reg compare</a> <a href="#reg-compare"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compare keys and their values in the registry.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-compare>.

#### Compare all values under a specific key with a second key:
```shell
reg compare {{first_key_name}} {{second_key_name}}
```
#### Compare a specific value under two keys:
```shell
reg compare {{first_key_name}} {{second_key_name}} /v {{value}}
```
#### Compare all sub keys and values for two keys:
```shell
reg compare {{first_key_name}} {{second_key_name}} /s
```
#### Only output the matches between the specified keys:
```shell
reg compare {{first_key_name}} {{second_key_name}} /os
```
#### Output the differences and matches between the specified keys:
```shell
reg compare {{first_key_name}} {{second_key_name}} /oa
```
{% endraw %}{% raw %}
<h2 id="reg-copy">
  <a href="/en/windows/reg-copy.html">reg copy</a> <a href="#reg-copy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copy keys and their values in the registry.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-copy>.

#### Copy a registry key to a new registry location:
```shell
reg copy {{old_key_name}} {{new_key_name}}
```
#### Copy a registry key recursively to a new registry location:
```shell
reg copy {{old_key_name}} {{new_key_name}} /s
```
#### Forcefully copy a registry key without a prompt:
```shell
reg copy {{old_key_name}} {{new_key_name}} /f
```
{% endraw %}{% raw %}
<h2 id="reg-delete">
  <a href="/en/windows/reg-delete.html">reg delete</a> <a href="#reg-delete"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Delete keys or their values from the registry.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-delete>.

#### Delete a specific registry key:
```shell
reg delete {{key_name}}
```
#### Delete a value under a specific key:
```shell
reg delete {{key_name}} /v {{value}}
```
#### Delete all values recursively under the specified key:
```shell
reg delete {{key_name}} /va
```
#### Forcefully delete all values recursively under a key without a prompt:
```shell
reg delete {{key_name}} /f /va
```
{% endraw %}{% raw %}
<h2 id="reg-export">
  <a href="/en/windows/reg-export.html">reg export</a> <a href="#reg-export"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Export the specified sub keys and values into a file.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-export>.

#### Export all sub keys and values of a specific key:
```shell
reg export {{key_name}} {{path/to/file.reg}}
```
#### Force overwriting of an existing file without prompt:
```shell
reg export {{key_name}} {{path/to/file.reg}} /y
```
{% endraw %}{% raw %}
<h2 id="reg-flags">
  <a href="/en/windows/reg-flags.html">reg flags</a> <a href="#reg-flags"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display or set flags on registry keys.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-flags>.

#### Display current flags for a specific key:
```shell
reg flags {{key_name}} query
```
#### Display help and available flag types:
```shell
reg flags /?
```
#### Set specified space-separated flags, and unset unmentioned flags, for a specific key:
```shell
reg flags {{key_name}} set {{flag_names}}
```
#### Set specified flags for a specific key and its sub keys:
```shell
reg flags {{key_name}} set {{flag_names}} /s
```
{% endraw %}{% raw %}
<h2 id="reg-import">
  <a href="/en/windows/reg-import.html">reg import</a> <a href="#reg-import"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Import all available keys, subkeys, and values from a file.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-import>.

#### Import all keys, subkeys and values from a file:
```shell
reg import {{path/to/file.reg}}
```
{% endraw %}{% raw %}
<h2 id="reg-load">
  <a href="/en/windows/reg-load.html">reg load</a> <a href="#reg-load"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Load saved sub keys into a different sub key in the registry.
> This is intended for troubleshooting and temporary keys.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-load>.

#### Load a backup file into the specified key:
```shell
reg load {{key_name}} {{path/to/file}}
```
{% endraw %}{% raw %}
<h2 id="reg-query">
  <a href="/en/windows/reg-query.html">reg query</a> <a href="#reg-query"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the values of keys and sub keys in the registry.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-query>.

#### Display all values of a key:
```shell
reg query {{key_name}}
```
#### Display a specific value of a key:
```shell
reg query {{key_name}} /v {{value}}
```
#### Display all values of a key and its sub keys:
```shell
reg query {{key_name}} /s
```
#### Search for keys and values matching a specific pattern:
```shell
reg query {{key_name}} /f "{{query_pattern}}"
```
#### Display a value of a key matching a specified data type:
```shell
reg query {{key_name}} /t {{type}}
```
{% endraw %}{% raw %}
<h2 id="reg-restore">
  <a href="/en/windows/reg-restore.html">reg restore</a> <a href="#reg-restore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Restore a key and its values from a backup file.
> See `reg-save` for more information.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-restore>.

#### Overwrite a specified key with data from a backup file:
```shell
reg restore {{key_name}} {{path/to/file}}
```
{% endraw %}{% raw %}
<h2 id="reg-save">
  <a href="/en/windows/reg-save.html">reg save</a> <a href="#reg-save"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Save a registry key, its sub keys and values to a file.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-save>.

#### Save a registry key, its sub keys and values to a specific file:
```shell
reg save {{key_name}} {{path/to/file}}
```
#### Forcefully overwrite an existing file without a prompt:
```shell
reg save {{key_name}} {{path/to/file}} /y
```
{% endraw %}{% raw %}
<h2 id="reg-unload">
  <a href="/en/windows/reg-unload.html">reg unload</a> <a href="#reg-unload"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove data from the registry that was loaded using the `reg load` command.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-unload>.

#### Remove data from the registry for a specified key:
```shell
reg unload {{key_name}}
```
{% endraw %}{% raw %}
<h2 id="reg">
  <a href="/en/windows/reg.html">reg</a> <a href="#reg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line interface for managing keys and their values in the Windows registry.
> See `reg-query`, `reg-add` and other pages for additional information.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg>.

#### Execute registry commands:
```shell
reg {{command}}
```
#### Display general information and list all available commands:
```shell
reg /?
```
#### Call help on a specific command:
```shell
reg {{command}} /?
```
{% endraw %}{% raw %}
<h2 id="repair-bde">
  <a href="/en/windows/repair-bde.html">repair-bde</a> <a href="#repair-bde"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Attempt to repair or decrypt a damaged BitLocker-encrypted volume.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/repair-bde>.

#### Attempt to repair a specified volume:
```shell
repair-bde {{C:}}
```
#### Attempt to repair a specified volume and output to another volume:
```shell
repair-bde {{C:}} {{D:}}
```
#### Attempt to repair a specified volume using the provided recovery key file:
```shell
repair-bde {{C:}} -RecoveryKey {{path/to/file.bek}}
```
#### Attempt to repair a specified volume using the provided numerical recovery password:
```shell
repair-bde {{C:}} -RecoveryPassword {{password}}
```
#### Attempt to repair a specified volume using the provided password:
```shell
repair-bde {{C:}} -Password {{password}}
```
#### Attempt to repair a specified volume using the provided key package:
```shell
repair-bde {{C:}} -KeyPackage {{path/to/directory}}
```
#### Log all output to a specific file:
```shell
repair-bde {{C:}} -LogFile {{path/to/file}}
```
#### Display all available options:
```shell
repair-bde /?
```
{% endraw %}{% raw %}
<h2 id="replace">
  <a href="/en/windows/replace.html">replace</a> <a href="#replace"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Replace files.
> See also: `robocopy`, `move`, `copy`, and `del`.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/replace>.

#### Replace the destination file with the one from the source directory:
```shell
replace {{path/to/file_or_directory}} {{path/to/destination}}
```
#### Add files to the destination directory instead of replacing existing files:
```shell
replace {{path/to/file_or_directory}} {{path/to/destination}} /a
```
#### Interactively copy multiple files, with a prompt before replacing or adding a destination file:
```shell
replace {{path/to/file_or_directory}} {{path/to/destination}} /p
```
#### Replace even read only files:
```shell
replace {{path/to/file_or_directory}} {{path/to/destination}} /r
```
#### Wait for you to insert a disk before it replaces files (originally to allow inserting a floppy disk):
```shell
replace {{path/to/file_or_directory}} {{path/to/destination}} /w
```
#### Replace all files in subdirectories of the destination:
```shell
replace {{path/to/file_or_directory}} {{path/to/destination}} /s
```
#### Replace only files in the destination directory which are older than the files in the source directory:
```shell
replace {{path/to/file_or_directory}} {{path/to/destination}} /u
```
#### Display detailed usage information:
```shell
replace /?
```
{% endraw %}{% raw %}
<h2 id="rmdir">
  <a href="/en/windows/rmdir.html">rmdir</a> <a href="#rmdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove a directory and its contents.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/rmdir>.

#### Remove an empty directory:
```shell
rmdir {{path/to/directory}}
```
#### Remove a directory and its contents recursively:
```shell
rmdir {{path/to/directory}} /s
```
#### Remove a directory and its contents recursively without prompting:
```shell
rmdir {{path/to/directory}} /s /q
```
{% endraw %}{% raw %}
<h2 id="robocopy">
  <a href="/en/windows/robocopy.html">robocopy</a> <a href="#robocopy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Robust File and Folder Copy.
> By default files will only be copied if the source and destination have different time stamps or different file sizes.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/robocopy>.

#### Copy all `.jpg` and `.bmp` files from one directory to another:
```shell
robocopy {{path/to/source}} {{path/to/destination}} {{*.jpg}} {{*.bmp}}
```
#### Copy all files and subdirectories, including empty ones:
```shell
robocopy {{path/to/source}} {{path/to/destination}} /E
```
#### Mirror/Sync a directory, deleting anything not in source and include all attributes and permissions:
```shell
robocopy {{path/to/source}} {{path/to/destination}} /MIR /COPYALL
```
#### Copy all files and subdirectories, excluding source files that are older than destination files:
```shell
robocopy {{path/to/source}} {{path/to/destination}} /E /XO
```
#### List all files 50 MBytes or larger in size instead of copying them:
```shell
robocopy {{path/to/source}} {{path/to/destination}} /MIN:52428800 /L
```
#### Allow resuming if network connection is lost and limit retries to 5 and wait time to 15 sec:
```shell
robocopy {{path/to/source}} {{path/to/destination}} /Z /R:5 /W:15
```
#### Display detailed usage information:
```shell
robocopy /?
```
{% endraw %}{% raw %}
<h2 id="rpcinfo">
  <a href="/en/windows/rpcinfo.html">rpcinfo</a> <a href="#rpcinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List programs via RPC on remote computers.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/rpcinfo>.

#### List all programs registered on the local computer:
```shell
rpcinfo
```
#### List all programs registered on a remote computer:
```shell
rpcinfo /p {{computer_name}}
```
#### Call a specific program on a remote computer using TCP:
```shell
rpcinfo /t {{computer_name}} {{program_name}}
```
#### Call a specific program on a remote computer using UDP:
```shell
rpcinfo /u {{computer_name}} {{program_name}}
```
{% endraw %}{% raw %}
<h2 id="scoop-bucket">
  <a href="/en/windows/scoop-bucket.html">scoop bucket</a> <a href="#scoop-bucket"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage buckets: Git repositories containing files which describe how scoop installs applications.
> If Scoop doesn't know where the bucket is located its repository location must be specified.
> More information: <https://github.com/lukesampson/scoop/wiki/Buckets>.

#### List all buckets currently in use:
```shell
scoop bucket list
```
#### List all known buckets:
```shell
scoop bucket known
```
#### Add a known bucket by its name:
```shell
scoop bucket add {{name}}
```
#### Add an unknown bucket by its name and Git repository URL:
```shell
scoop bucket add {{name}} {{https://example.com/repository.git}}
```
#### Remove a bucket by its name:
```shell
scoop bucket rm {{name}}
```
{% endraw %}{% raw %}
<h2 id="scoop">
  <a href="/en/windows/scoop.html">scoop</a> <a href="#scoop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line installer for Windows.
> More information: <https://scoop.sh>.

#### Install a package:
```shell
scoop install {{package}}
```
#### Remove a package:
```shell
scoop uninstall {{package}}
```
#### Update all installed packages:
```shell
scoop update *
```
#### List installed packages:
```shell
scoop list
```
#### Display information about a package:
```shell
scoop info {{package}}
```
#### Search for a package:
```shell
scoop search {{package}}
```
#### Remove old versions of all packages and clear the download cache:
```shell
scoop cleanup -k *
```
{% endraw %}{% raw %}
<h2 id="set">
  <a href="/en/windows/set.html">set</a> <a href="#set"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display or set environment variables for the current instance of CMD.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/set>.

#### List all current environment variables:
```shell
set
```
#### Set an environment variable to a specific value:
```shell
set {{name}}={{value}}
```
#### List environment variables starting with the specified string:
```shell
set {{name}}
```
#### Prompt the user for a value for the specified variable:
```shell
set /p {{name}}={{prompt_string}}
```
{% endraw %}{% raw %}
<h2 id="sfc">
  <a href="/en/windows/sfc.html">sfc</a> <a href="#sfc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Scans the integrity of Windows system files.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/sfc>.

#### Display information about the usage of the command:
```shell
sfc
```
#### Scan all system files and, if possible, repair any problems:
```shell
sfc /scannow
```
#### Scan all system files without attempting to repair any:
```shell
sfc /verifyonly
```
#### Scan a specific file and, if possible, repair any problems:
```shell
sfc /scanfile={{path/to/file}}
```
#### Scan a specific file without attempting to repair it:
```shell
sfc /verifyfile={{path/to/file}}
```
#### When repairing offline, specify the boot directory:
```shell
sfc /offbootdir={{path/to/directory}}
```
#### When repairing offline, specify the Windows directory:
```shell
sfc /offwindir={{path/to/directory}}
```
{% endraw %}{% raw %}
<h2 id="showmount">
  <a href="/en/windows/showmount.html">showmount</a> <a href="#showmount"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about NFS filesystems on Windows Server.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/showmount>.

#### Display all exported filesystems:
```shell
showmount -e
```
#### Display all NFS clients and their mounted directories:
```shell
showmount -a
```
#### Display all NFS mounted directories:
```shell
showmount -d
```
#### Display all exported filesystems for a remote server:
```shell
showmount -e {{server_address}}
```
{% endraw %}{% raw %}
<h2 id="shutdown">
  <a href="/en/windows/shutdown.html">shutdown</a> <a href="#shutdown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool for shutting down, restarting or logging off a machine.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/shutdown>.

#### Shutdown the current machine:
```shell
shutdown /s
```
#### Shutdown the current machine force-closing all apps:
```shell
shutdown /s /f
```
#### Restart the current machine immediately:
```shell
shutdown /r /t 0
```
#### Hibernate the current machine:
```shell
shutdown /h
```
#### Log off the current machine:
```shell
shutdown /l
```
#### Specify a timeout in seconds to wait before shutting down:
```shell
shutdown /s /t {{seconds}}
```
#### Abort a shutdown sequence whose timeout is yet to expire:
```shell
shutdown /a
```
#### Shutdown a remote machine:
```shell
shutdown /m {{\\hostname}}
```
{% endraw %}{% raw %}
<h2 id="subst">
  <a href="/en/windows/subst.html">subst</a> <a href="#subst"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Associates a path with a virtual drive letter.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/subst>.

#### List active associations:
```shell
subst
```
#### Add an association:
```shell
subst {{Z:}} {{C:\Python2.7}}
```
#### Remove an association:
```shell
subst {{Z:}} /d
```
{% endraw %}{% raw %}
<h2 id="systeminfo">
  <a href="/en/windows/systeminfo.html">systeminfo</a> <a href="#systeminfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display operating system configuration for a local or remote machine.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/systeminfo>.

#### Display system configuration for the local machine:
```shell
systeminfo
```
#### Display system configuration in a specified output format:
```shell
systeminfo /fo {{table|list|csv}}
```
#### Display system configuration for a remote machine:
```shell
systeminfo /s {{remote_name}} /u {{username}} /p {{password}}
```
#### Display detailed usage information:
```shell
systeminfo /?
```
{% endraw %}{% raw %}
<h2 id="takeown">
  <a href="/en/windows/takeown.html">takeown</a> <a href="#takeown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Take ownership of a file or directory.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/takeown>.

#### Take ownership of the specified file:
```shell
takeown /f {{path/to/file}}
```
#### Take ownership of the specified directory:
```shell
takeown /d {{path/to/directory}}
```
#### Take ownership of the specified directory and all subdirectories:
```shell
takeown /r /d {{path/to/directory}}
```
#### Change ownership to the Administrator group instead of the current user:
```shell
takeown /a /f {{path/to/file}}
```
{% endraw %}{% raw %}
<h2 id="taskkill">
  <a href="/en/windows/taskkill.html">taskkill</a> <a href="#taskkill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Terminate a process by its process id or name.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/taskkill>.

#### Terminate a process by its id:
```shell
taskkill /pid {{process_id}}
```
#### Terminate a process by its name:
```shell
taskkill /im {{process_name}}
```
#### Forcefully terminate a specified process:
```shell
taskkill /pid {{process_id}} /f
```
#### Terminate a process and its child processes:
```shell
taskkill /im {{process_name}} /t
```
#### Terminate a process on a remote machine:
```shell
taskkill /pid {{process_id}} /s {{remote_name}}
```
#### Display information about the usage of the command:
```shell
taskkill /?
```
{% endraw %}{% raw %}
<h2 id="tasklist">
  <a href="/en/windows/tasklist.html">tasklist</a> <a href="#tasklist"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display a list of currently running processes on a local or remote machine.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/tasklist>.

#### Display currently running processes:
```shell
tasklist
```
#### Display running processes in a specified output format:
```shell
tasklist /fo {{table|list|csv}}
```
#### Display running processes using the specified `.exe` or `.dll` file name:
```shell
tasklist /m {{module_pattern}}
```
#### Display processes running on a remote machine:
```shell
tasklist /s {{remote_name}} /u {{username}} /p {{password}}
```
#### Display services using each process:
```shell
tasklist /svc
```
{% endraw %}{% raw %}
<h2 id="title">
  <a href="/en/windows/title.html">title</a> <a href="#title"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set the title of the command prompt window.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/title>.

#### Set the title of the current command prompt window:
```shell
title {{new_title}}
```
{% endraw %}{% raw %}
<h2 id="tree">
  <a href="/en/windows/tree.html">tree</a> <a href="#tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display a graphical tree of the directory structure for a path.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/tree>.

#### Display the tree for the current directory:
```shell
tree
```
#### Display the tree for a specific directory:
```shell
tree {{path/to/directory}}
```
#### Display the tree for a directory including files:
```shell
tree {{path/to/directory}} /f
```
#### Display the tree using ASCII characters instead of extended characters:
```shell
tree {{path/to/directory}} /a
```
{% endraw %}{% raw %}
<h2 id="tskill">
  <a href="/en/windows/tskill.html">tskill</a> <a href="#tskill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ends a process running in a session on a Remote Desktop Session Host.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/tskill>.

#### Terminate a process by its process identifier:
```shell
tskill {{process_id}}
```
#### Terminate a process by its name:
```shell
tskill {{process_name}}
```
{% endraw %}{% raw %}
<h2 id="type">
  <a href="/en/windows/type.html">type</a> <a href="#type"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the contents of a file.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/type>.

#### Display the contents of a specific file:
```shell
type {{path/to/file}}
```
{% endraw %}{% raw %}
<h2 id="tzutil">
  <a href="/en/windows/tzutil.html">tzutil</a> <a href="#tzutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool for displaying or configuring the system time zone.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/tzutil>.

#### Get the current time zone:
```shell
tzutil /g
```
#### Display a list of available time zones:
```shell
tzutil /l
```
#### Set the system time zone to the specific value:
```shell
tzutil /s {{timezone_id}}
```
{% endraw %}{% raw %}
<h2 id="ver">
  <a href="/en/windows/ver.html">ver</a> <a href="#ver"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the current Windows or MS-DOS version number.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/ver>.

#### Display the current version number:
```shell
ver
```
{% endraw %}{% raw %}
<h2 id="virtualboxvm">
  <a href="/en/windows/virtualboxvm.html">virtualboxvm</a> <a href="#virtualboxvm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The VirtualBox virtual machine management CLI.
> More information: <https://www.virtualbox.org>.

#### Start a virtual machine:
```shell
virtualboxvm --startvm {{name|uuid}}
```
#### Start a virtual machine in fullscreen mode:
```shell
virtualboxvm --startvm {{name|uuid}} --fullscreen
```
#### Mount the specified DVD image file:
```shell
virtualboxvm --startvm {{name|uuid}} --dvd {{path/to/image_file}}
```
#### Display a command-line window with debug information:
```shell
virtualboxvm --startvm {{name|uuid}} --debug-command-line
```
#### Start a virtual machine in a paused state:
```shell
virtualboxvm --startvm {{name|uuid}} --start-paused
```
{% endraw %}{% raw %}
<h2 id="vol">
  <a href="/en/windows/vol.html">vol</a> <a href="#vol"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about volumes.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/vol>.

#### Display the label and serial number for the current drive:
```shell
vol
```
#### Display the label and serial number for a specific volume:
```shell
vol {{D:}}
```
{% endraw %}{% raw %}
<h2 id="where">
  <a href="/en/windows/where.html">where</a> <a href="#where"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the location of files that match the search pattern.
> Defaults to current work directory and paths in the PATH environment variable.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/where>.

#### Display the location of file pattern:
```shell
where {{file_pattern}}
```
#### Display the location of file pattern including file size and date:
```shell
where /T {{file_pattern}}
```
#### Recursively search for file pattern at specified path:
```shell
where /R {{path/to/directory}} {{file_pattern}}
```
#### Display only the error code for the location of file pattern:
```shell
where /Q {{file_pattern}}
```
{% endraw %}{% raw %}
<h2 id="whoami">
  <a href="/en/windows/whoami.html">whoami</a> <a href="#whoami"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display details about the current user.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/whoami>.

#### Display the username of the current user:
```shell
whoami
```
#### Display the groups that the current user is a member of:
```shell
whoami /groups
```
#### Display the privileges of the current user:
```shell
whoami /priv
```
#### Display the user principal name (UPN) of the current user:
```shell
whoami /upn
```
#### Display the logon id of the current user:
```shell
whoami /logonid
```
{% endraw %}{% raw %}
<h2 id="winget">
  <a href="/en/windows/winget.html">winget</a> <a href="#winget"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Windows Package Manager CLI.
> More information: <https://docs.microsoft.com/windows/package-manager/winget>.

#### Install a package:
```shell
winget install {{package}}
```
#### Display information about a package:
```shell
winget show {{package}}
```
#### Search for a package:
```shell
winget search {{package}}
```
{% endraw %}{% raw %}
<h2 id="wmic">
  <a href="/en/windows/wmic.html">wmic</a> <a href="#wmic"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interactive shell for detailed information about running processes.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/wmic>.

#### Fundamental grammar:
```shell
wmic {{alias}} {{where_clause}} {{verb_clause}}
```
#### Show brief details about the currently running processes:
```shell
wmic process list brief
```
#### Show full details about the currently running processes:
```shell
wmic process list full
```
#### Access specific fields such as process name, process ID and parent process ID:
```shell
wmic process get {{name,processid,parentprocessid}}
```
#### Display information about a specific process:
```shell
wmic process where {{name="example.exe"}} list full
```
#### Display specific fields for a specific process:
```shell
wmic process where processid={{pid}} get {{name,commandline}}
```
#### Kill a process:
```shell
wmic process {{pid}} delete
```
{% endraw %}{% raw %}
<h2 id="wsl">
  <a href="/en/windows/wsl.html">wsl</a> <a href="#wsl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage the Windows Subsystem for Linux from the command-line.
> More information: <https://docs.microsoft.com/windows/wsl/reference>.

#### Start a Linux shell (in the default distribution):
```shell
wsl {{shell_command}}
```
#### Run a Linux command without using a shell:
```shell
wsl --exec {{command}} {{command_arguments}}
```
#### Specify a particular distribution:
```shell
wsl --distribution {{distribution}} {{shell_command}}
```
#### List available distributions:
```shell
wsl --list
```
#### Export a distribution to a `.tar` file:
```shell
wsl --export {{distribution}} {{path/to/distro_fs.tar}}
```
#### Import a distribution from a `.tar` file:
```shell
wsl --import {{distribution}} {{path/to/install_location}} {{path/to/distro_fs.tar}}
```
#### Change the version of the specified distribution:
```shell
wsl --set-version {{distribution}} {{version}}
```
#### Shut down Windows Subsystem for Linux:
```shell
wsl --shutdown
```
{% endraw %}{% raw %}
<h2 id="xcopy">
  <a href="/en/windows/xcopy.html">xcopy</a> <a href="#xcopy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copy files and directory trees.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/xcopy>.

#### Copy the file(s) to the specified destination:
```shell
xcopy {{path/to/file_or_directory}} {{path/to/destination}}
```
#### List files that will be copied before copying:
```shell
xcopy {{path/to/file_or_directory}} {{path/to/destination}} /p
```
#### Copy the directory structure only, excluding files:
```shell
xcopy {{path/to/file_or_directory}} {{path/to/destination}} /t
```
#### Include empty directories when copying:
```shell
xcopy {{path/to/file_or_directory}} {{path/to/destination}} /e
```
#### Keep the source ACL in the destination:
```shell
xcopy {{path/to/file_or_directory}} {{path/to/destination}} /o
```
#### Allow resuming when network connection is lost:
```shell
xcopy {{path/to/file_or_directory}} {{path/to/destination}} /z
```
#### Disable the prompt when the file exists in the destination:
```shell
xcopy {{path/to/file_or_directory}} {{path/to/destination}} /y
```
#### Display detailed usage information:
```shell
xcopy /?
```
{% endraw %}