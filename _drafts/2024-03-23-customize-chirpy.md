---
layout: post
title: Customize the Chirpy Starter Jekyll Theme
date: 2024-03-23 15:55 +1300
categories: [documentation]
tags: [jekyll, how-to]
---


### Step 3: Changing the Side Menu 
The side menu defaults to Home, Categories, Tags, Archives and About pages. Lets update it and add Docs and Posts. 


In the `_data` directory, create a new directory called `_locales` 
```bash
mkdir -p _data/_locales
``` 

Go to [Chirpy Locales](https://github.com/cotes2020/jekyll-theme-chirpy/tree/master/_data/locales) and copy `en.yaml` (or your preferred locale) into the new `_locales` directory 

Look for the tabs section in `en.yaml`  and change it to the following: 
```yaml
# The tabs of sidebar
tabs:
  # format: <filename_without_extension>: <value>
  home: Home
  categories: Docs
  tags: Tags
  archives: All Posts
  about: About
```

We're changing the values for `categories` to `Docs` and `archives` to `All Posts`

Up to you what you want to rename these to
