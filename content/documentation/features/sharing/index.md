---
title: "Sharing"
date: 2018-10-12T21:33:16+10:00
draft: false
---

This theme includes sharing buttons from https://sharingbuttons.io/ by default.

To enable sharing, add the following to your site configuration:

```toml
[params.sharing]
  enabled = ["twitter", "pinterest", "facebook", "unk"] 
  size = "large" # OPTIONAL [small, medium, large (default)]
  style = "solid" # OPTIONAL [solid (default), circle, solidcircle, normal]
  label = "Share on " # OPTIONAL "Share on " default
```

The above renders the following:

![Sharing Buttons Screenshot](/images/screenshot-sharing.png)

Roll out your own sharing buttons by overwriting `layout/partials/utils/sharing.html` and `assets/scss/_sharing.scss`.

The full list of available buttons are:   

  - facebook
  - twitter
  - googleplus
  - tumblr
  - email
  - pinterest
  - linkedin
  - reddit
  - xing
  - whatsapp
  - hackernews
  - vk
  - telegram
