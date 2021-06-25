---
layout: default
title: "feedreader"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="feedreader">
  <a href="/en/linux/feedreader.html">feedreader</a> <a href="#feedreader"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A GUI desktop RSS client.
> More information: <https://jangernert.github.io/FeedReader/>.

#### Print the count of unread articles:
```shell
feedreader --unreadCount
```
#### Add a URL for a feed to follow:
```shell
feedreader --addFeed={{feed_url}}
```
#### Grab a specific article using its URL:
```shell
feedreader --grabArticle={{article_url}}
```
#### Download all images from a specific article:
```shell
feedreader --url={{feed_url}} --grabImages={{article_path}}
```
#### Play media from a URL:
```shell
feedreader --playMedia={{article_url}}
```
{% endraw %}