---
title: Writing guide
layout: page
---

# Start Jekyll with 
```
jekyll serve
```

# Algolia

To be able to push new search results you need to compile jekyll with new data

```
ALGOLIA_API_KEY='ADMIN-KEY' bundle exec jekyll algolia
```

# Helper elements for include

## Youtube Lazy Load

## 2 Columns for imagesand text


# Folders

- getting-started
- basics
- guides
- advanced
- tutorials
- integrations
- faq

# Helper classes 

```
{: .col-2}
![](/wp-content/uploads/2022/05/Screenshot-2022-05-25-at-21.46.48-800x1217.png){: .half-img}
![](/wp-content/uploads/2022/05/Screenshot-2022-05-26-at-13.37.07-800x1796.png){: .half-img}
```

will wrap images in p with class="col-2"

## Available helper classes

.col-2
.col-3
.col-4

## Reusable parts

OEmbed (Youtube)

```
{% include youtube.html id="xxxxxxx" %}
```

replace xxxxxxx with youtubeID and not the entire URL
