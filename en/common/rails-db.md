---
layout: default
title: "rails db"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rails-db">
  <a href="/en/common/rails-db.html">rails db</a> <a href="#rails-db"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Various database-related subcommands for Ruby on Rails.

#### Create databases, load the schema, and initialize with seed data:
```shell
rails db:setup
```
#### Access the database console:
```shell
rails db
```
#### Create the databases defined in the current environment:
```shell
rails db:create
```
#### Destroy the databases defined in the current environment:
```shell
rails db:drop
```
#### Run pending migrations:
```shell
rails db:migrate
```
#### View the status of each migration file:
```shell
rails db:migrate:status
```
#### Rollback the last migration:
```shell
rails db:rollback
```
#### Fill the current database with data defined in `db/seeds.rb`:
```shell
rails db:seed
```
{% endraw %}