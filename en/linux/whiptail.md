---
layout: default
title: "whiptail"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="whiptail">
  <a href="/en/linux/whiptail.html">whiptail</a> <a href="#whiptail"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display text-based dialog boxes from shell scripts.

#### Display a simple message:
```shell
whiptail --title "{{title}}" --msgbox "{{message}}" {{height_in_chars}} {{width_in_chars}}
```
#### Display a boolean choice, returning the result through the exit code:
```shell
whiptail --title "{{title}}" --yesno "{{message}}" {{height_in_chars}} {{width_in_chars}}
```
#### Customise the text on the yes / no buttons:
```shell
whiptail --title "{{title}}" --yes-button "{{text}}" --no-button "{{text}}" --yesno "{{message}}" {{height_in_chars}} {{width_in_chars}}
```
#### Display a text input box:
```shell
{{result_variable_name}}="$(whiptail --title "{{title}}" --inputbox "{{message}}" {{height_in_chars}} {{width_in_chars}} {{default_text}} 3>&1 1>&2 2>&3)"
```
#### Display a password input box:
```shell
{{result_variable_name}}="$(whiptail --title "{{title}}" --passwordbox "{{message}}" {{height_in_chars}} {{width_in_chars}} 3>&1 1>&2 2>&3)"
```
#### Display a multiple-choice menu:
```shell
{{result_variable_name}}=$(whiptail --title "{{title}}" --menu "{{message}}" {{height_in_chars}} {{width_in_chars}} {{menu_display_height}} "{{value_1}}" "{{display_text_1}}" "{{value_n}}" "{{display_text_n}}" ..... 3>&1 1>&2 2>&3)
```
{% endraw %}