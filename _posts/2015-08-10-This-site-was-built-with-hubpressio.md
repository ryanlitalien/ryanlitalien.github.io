---
layout: post
title: This site was built with hubpress.io
tags:
  - Technology
image: /assets/img/demopic/10.jpg
---

I needed a "quick", free and server-less blog with domain forwarding. I liked the [Jekyll](http://jekyllrb.com/) static site generator, though there were too many caveats. The open source project hubpress.io/ seemed solid, fork a repo, change a config.json file and then good to go, right? Not so fast.

I ran into several problems, but mostly were my legacy problems. I had previously setup two blogs using [GitHub Pages](https://pages.github.com/). One of those projects had a `_config.yml` file that redirected to an old, unused and completely different domain. It also didn't help that I had several CNAME redirects setup in AWS Route 53. After deleting both old repos, removing A and CNAME records within AWS, we're good to go.

Here's the configuration I ended up with:

```
https://github.com/ryanlitalien/website/blob/609b3cee892e104aedea71aabde16cd85ea4b63b/hubpress/config.json
```

I might open a pull request with the guys at HubPress to format the `config.json` with pretty print.

Not bad for the first post :)

---

#### Update (June 12th, 2019)

> I scrapped hubpress.io since it now links to a "Buy Instagram Followers" page, aka domain squatted. Moving/moved to Jekyll via Github Pages.
