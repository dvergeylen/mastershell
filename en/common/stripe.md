---
layout: default
title: "stripe"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="stripe">
  <a href="/en/common/stripe.html">stripe</a> <a href="#stripe"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interact with a Stripe account.
> More information: <https://github.com/stripe/stripe-cli>.

#### Follow the logs of activity on the account:
```shell
stripe logs tail
```
#### Listen for events, filtering on events with the name `charge.succeeded` and forwarding them to localhost:3000/events:
```shell
stripe listen --events="{{charge.succeeded}}" --forward-to="{{localhost:3000/events}}"
```
#### Send a test webhook event:
```shell
stripe trigger {{charge.succeeded}}
```
#### Create a customer:
```shell
stripe customers create --email="{{test@example.com}}" --name="{{Jenny Rosen}}"
```
#### Print to JSON:
```shell
stripe listen --print-json
```
{% endraw %}