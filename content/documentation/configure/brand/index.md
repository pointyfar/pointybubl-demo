---
title: "Configure Brand"
date: 2018-09-24T22:10:53+10:00
draft: false
---

The theme uses `params.title` to populate the top left of the nav bar. 

The hero banner on the index page also uses this value. 


```toml
[params]
  title = "Pointy's"
  subtitle = "Blog Template for Hugo"
```

The subtitle uses the `params.subtitle` value on the index page. Author information is used on content pages. Read about [configuring authors here]({{< relref "authors/index.md" >}}).

Alternatively, you can choose to use a logo or image instead of hero text.

```toml
[params.brandimage]
  image = "images/awesome-logo.png"

```
![Screenshot Hero Image](/images/screenshot-image-hero.png)
