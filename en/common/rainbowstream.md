---
layout: default
title: "rainbowstream"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rainbowstream">
  <a href="/en/common/rainbowstream.html">rainbowstream</a> <a href="#rainbowstream"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Terminal-based Twitter client supporting realtime tweetstream, trends, sending, search, favorites and user management.
> Online help with `h`, up and down arrows for history, tab to auto-complete and 2-tab for suggestion.
> More information: <https://github.com/orakaro/rainbowstream>.

#### Open rainbowstream:
```shell
rainbowstream
```
#### Show your timeline (optional number of tweets to display, default is 5):
```shell
home [{{num_of_last_tweets}}]
```
#### Show profile of a given user:
```shell
whois @{{user}}
```
#### Tweet the message as-is:
```shell
t {{message}}
```
#### Retweet the tweet with given id (id is beside the time):
```shell
rt {{tweet_id}}
```
#### Favorite the tweet with given id:
```shell
fav {{tweet_id}}
```
#### Perform a search for a given word (with or without hashtag):
```shell
s {{word}}
```
{% endraw %}