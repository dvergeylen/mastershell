---
layout: default
title: "gh api"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gh-api">
  <a href="/en/common/gh-api.html">gh api</a> <a href="#gh-api"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Makes authenticated HTTP requests to the GitHub API and prints the response.
> More information: <https://cli.github.com/manual/gh_api>.

#### Display the subcommand help:
```shell
gh api --help
```
#### Display the releases for the current repository in JSON format:
```shell
gh api repos/:owner/:repo/releases
```
#### Create a reaction for a specific issue:
```shell
gh api --header {{Accept:application/vnd.github.squirrel-girl-preview+json}} --raw-field '{{content=+1}}' {{repos/:owner/:repo/issues/123/reactions}}
```
#### Display the result of a GraphQL query in JSON format:
```shell
gh api graphql --field {{name=':repo'}} --raw-field '{{query}}'
```
#### Send a request using a custom HTTP method:
```shell
gh api --method {{POST}} {{endpoint}}
```
#### Include the HTTP response headers in the output:
```shell
gh api --include {{endpoint}}
```
#### Do not print the response body:
```shell
gh api --silent {{endpoint}}
```
#### Send a request to a specific GitHub Enterprise Server:
```shell
gh api --hostname {{github.example.com}} {{endpoint}}
```
{% endraw %}