---
layout: default
title: "notmuch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="notmuch">
  <a href="/en/common/notmuch.html">notmuch</a> <a href="#notmuch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line based program for indexing, searching, reading, and tagging large collections of email messages.
> More information: <https://notmuchmail.org/manpages/>.

#### Configure for first use:
```shell
notmuch setup
```
#### Add a tag for all messages matching a search term:
```shell
notmuch tag +{{custom_tag}} "{{search_term}}"
```
#### Remove a tag for all messages matching a search term:
```shell
notmuch tag -{{custom_tag}} "{{search_term}}"
```
#### Count messages matching the given search term:
```shell
notmuch count --output={{messages|threads}} "{{search_term}}"
```
#### Search for messages matching the given search term:
```shell
notmuch search --format={{json|text}} --output={{summary|threads|messages|files|tags}} "{{search_term}}"
```
#### Limit the number of search results to X:
```shell
notmuch search --format={{json|text}} --output={{summary|threads|messages|files|tags}} --limit={{X}} "{{search_term}}"
```
#### Create a reply template for a set of messages:
```shell
notmuch reply --format={{default|headers-only}} --reply-to={{sender|all}} "{{search_term}}"
```
{% endraw %}