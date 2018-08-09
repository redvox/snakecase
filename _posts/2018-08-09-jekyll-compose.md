---
layout: post
title: jekyll-compose
date: 2018-08-09 13:08 +0200
---

To streamline the writing process for this blog i added a new dependencie calles 'jekyll-compose'

[jekyll/jekyll-compose](https://github.com/jekyll/jekyll-compose)

## Installation

Add this line to your application's Gemfile:

    gem 'jekyll-compose', group: [:jekyll_plugins]

And then execute:

    $ bundle

## Usage

After you have installed (see above), run `bundle exec jekyll help` and you should see:

Listed in help you will see new commands available to you:

```sh
  draft      # Creates a new draft post with the given NAME
  post       # Creates a new post with the given NAME
  publish    # Moves a draft into the _posts directory and sets the date
  unpublish  # Moves a post back into the _drafts directory
  page       # Creates a new page with the given NAME
``` 