---
layout: default
title: "zenity"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zenity">
  <a href="/en/linux/zenity.html">zenity</a> <a href="#zenity"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display dialogs from the command-line/shell scripts.
> Return user-inserted values or 1 if error.

#### Display the default question dialog:
```shell
zenity --question
```
#### Display an info dialog displaying the text "Hello!":
```shell
zenity --info --text="{{Hello!}}"
```
#### Display a name/password form and output the data separated by ";":
```shell
zenity --forms --add-entry="{{Name}}" --add-password="{{Password}}" --separator="{{;}}"
```
#### Display a file selection form in which the user can only select directories:
```shell
zenity --file-selection --directory
```
#### Display a progress bar which updates its message every second and show a progress percent:
```shell
{{(echo "#1"; sleep 1; echo "50"; echo "#2"; sleep 1; echo "100")}} | zenity --progress
```
{% endraw %}