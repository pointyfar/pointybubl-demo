---
title: "Section Layouts"
date: 2018-09-24T22:12:53+10:00
draft: false
---

You can configure the list layout view for section pages in its `_index.md` frontmatter. You can also configure whether to paginate the list view by specifying `paginatelist: true` in the front matter.


## default
![Section List](/images/screenshot-list-default.png) 


## `layout: cardlist`

This layout takes the first image resource it finds for a post and uses that as a preview image. 

![Section List](/images/screenshot-list-card.png) 

## `layout: gallery`

Similar to the above, but with larger featured image.

![Image Preview](/images/screenshot-list-gallery.png) 

---

You can configure a default placeholder image to use for pages that don't have images. You can also alternatively configure an inline svg to render instead.

![Placeholder SVG](/images/screenshot-placeholder-svg.png) 

You can also disable the image preview entirely by setting `disabled = true` under `[params.placeholder]`

```
[params.placeholder]
  # default value is false, i.e. displayed
  disabled = false
  
  ## use img 
  img = "/img/placeholder-100.png"
  
  ######## OR 
  
  ## use svg
  size = "100px"
  text = "[no image available]"
  text_size = "9px"
```