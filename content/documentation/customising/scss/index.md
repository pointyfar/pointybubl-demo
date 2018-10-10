---
title: "Scss"
date: 2018-09-24T22:14:16+10:00
draft: false
---

This theme uses the shiny new [Hugo Pipes](https://gohugo.io/hugo-pipes/)!

This theme uses [Bulma](https://bulma.io/) base styles. Follow their [instructions for customising Bulma](https://bulma.io/documentation/overview/customize/) using Sass.

You can override Bulma variables in `<YOUR-HUGO-SITE>/assets/scss/_bulma_overrides.scss`.

```scss 
$primary: hotpink;

```

You can also define additional custom styles in   `<YOUR-HUGO-SITE>/assets/scss/_custom.scss`, which will be imported after everything else.

```scss
.tag.cuisine-tag {
  background-color: aliceblue;
  color: black;
}

```

You can also configure a limited set of scss variables from your `config.toml` file:

```toml
[params.scss]
  primary = "hotpink"
```

The above will both result in

![Hotpink primary](/images/screenshot-configure-scss.png)

## NOTE:

The changes will only have an effect if you are using the [extended version of Hugo](https://gohugo.io/getting-started/installing), which allows for scss processing. 

If you are not using the extended version, you may still override individual styles by using a custom css file.

## SCSS variables

Below are the scss variables you can customise from your `config.toml`:

```
[params.scss]
  customFontBody = "Georgia,Utopia,Charter,serif"
  brandFont = "'Oswald', sans-serif"
  primary = "CadetBlue"
  primaryInvert = "#fff"
  footnote = "FOOTNOTE:"
  linkColor = "navy"
  
```