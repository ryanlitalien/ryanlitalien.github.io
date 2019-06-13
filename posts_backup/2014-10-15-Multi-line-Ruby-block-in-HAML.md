---
layout: post
title: Multi-line Ruby block in HAML
published_at: 2014-10-15
tags:
  - Technology
  - Ruby
  - HAML
---

I always seem to forget the syntax for multi-line syntax in haml.  You can also use `:css`, `:javascript`

```
:ruby
  first_name = "Ryan"
  last_name = "L'Italien"
%h1
  = "#{last_name}, #{first_name}"
```

Source: [http://makandracards.com/makandra/2797-multi-line-ruby-block-in-haml](http://makandracards.com/makandra/2797-multi-line-ruby-block-in-haml)
