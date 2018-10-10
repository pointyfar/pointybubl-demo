---
title: "Configure Sidebar"
date: 2018-09-24T22:11:12+10:00
draft: false
---

Several sidebar 'boxes' are available to customise and use. 

## author

Populates the box with author details if a featured author is configured. 

```toml
[[params.sidebar.box]]
  type = "author"
```

## tagcloud
Generates a 'tag' cloud using the taxonomy specified. An optional label may be configured. If a `threshold` is defined, only 'tags' whose related content count are greater than or equal to that value will be displayed.

```toml
[[params.sidebar.box]]
  type = "tagcloud"
  label = "A Cloud of Tags"
  taxonomy = "authors"
  threshold = 1
```

## social

```toml
[[params.sidebar.box]]
  type = "social"
  data = "social"
```

You can add a social box on the sidebar by pointing `data` to a file in your `data` folder. This demo site has a sample `social.toml` data file which has the following contents:

```toml
label = "I am social!"

[[social]]
  url = "http://www.twitter.com"
  icon = "fab fa-twitter"
  color = "#55acee"

[[social]]
  url = "http://www.github.com"
  icon = "fab fa-github"
  color = "#333"

...
```

`color` is optional and the [configured `primary` color]({{< relref "../customising/scss/index.md" >}}) will be used by default.

![Social Box Screenshot](/images/screenshot-social-box.png)


## custom

Custom boxes can also be added. Simply specify the partial to be used to render the box.

```toml
[[params.sidebar.box]]
  type = "custom"
  partial = "sidebar/custom-box.html"
```