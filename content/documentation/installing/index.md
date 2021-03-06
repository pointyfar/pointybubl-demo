---
title: "Installing the Theme"
date: 2018-09-24T22:09:47+10:00
draft: false
weight: 1
---

Follow the instructions in the Hugo documentation: 
https://gohugo.io/themes/installing-and-using-themes/ 

If you are deploying your Hugo site on Netlify, please note that you need to add the theme as a submodule: 
https://gohugo.io/hosting-and-deployment/hosting-on-netlify/#use-hugo-themes-with-netlify

---

Add `pointybubl` as submodule    
  ```
  $ git submodule add https://github.com/pointyfar/pointybubl.git themes/pointybubl/
  ```    
  
  
Configure your Hugo site to use `pointybubl` as its theme and then run `hugo server`    
  ```toml
  # config.toml
  theme = "pointybubl"
  ```

Navigate to your hugo project and run 

```bash
hugo server
```
Open your browser and navigate to `localhost:1313`.

Up Next: [Configuring]({{% relref "/documentation/configure/introduction/index.md" %}})

