---
layout: post
title: Handlebars render safe HTML
published_at: 2015-03-20
tags:
  - Technology
  - Handlebars
---

I have an Ember application that I need to display some custom text.

If you want to render raw html to the page, use a triple curly brace:

```
{{{customText}}}
```

Normally it's only a double curly:

```
{{customText}}
```

Source: [http://handlebarsjs.com/](http://handlebarsjs.com/)
