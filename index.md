---
layout: default
---

<div class="mainheading">
  <h1 class="sitetitle"></h1>
  <p class="lead">
    "Sometimes you gotta run before you can walk" - Tony Stark
  </p>
</div>

<section class="recent-posts">
  <div class="section-title">
    <h2><span>All Posts</span></h2>
  </div>
  <div class="card-columns listrecent">
    {% for post in site.posts %}
      <div class="card">
        <a href="{{ post.url }}">
          <img class="img-fluid" src="/assets/img/demopic/8.jpg" alt="">
        </a>
        <div class="card-block">
          <h2 class="card-title"><a href="{{ post.url }}">{{ post.title }}</a></h2>
          <h4 class="card-text">{{ post.excerpt }}</h4>
          <div class="metafooter">
            <div class="wrapfooter">
              <span class="meta-footer-thumb">
              <a href="{{ post.url }}">
                <img class="author-thumb" src="https://s.gravatar.com/avatar/79c3827e7bad5914462a25d732300459?s=250&amp;d=mm&amp;r=x" alt="Ryan">
              </a>
              </span>
              <span class="author-meta">
              <span class="post-name"><a href="/author.html">Ryan</a></span><br/>
              <span class="post-date">22 July 2017</span><span class="dot"></span><span class="post-read">6 min read</span>
              </span>
              <span class="post-read-more">
                <a href="{{ post.url }}" title="Read Story">
                  <svg class="svgIcon-use" width="25" height="25" viewbox="0 0 25 25">
                    <path d="M19 6c0-1.1-.9-2-2-2H8c-1.1 0-2 .9-2 2v14.66h.012c.01.103.045.204.12.285a.5.5 0 0 0 .706.03L12.5 16.85l5.662 4.126a.508.508 0 0 0 .708-.03.5.5 0 0 0 .118-.285H19V6zm-6.838 9.97L7 19.636V6c0-.55.45-1 1-1h9c.55 0 1 .45 1 1v13.637l-5.162-3.668a.49.49 0 0 0-.676 0z" fill-rule="evenodd"></path>
                  </svg>
                </a>
              </span>
            </div>
          </div>
        </div>
      </div>
    {% endfor %}
  </div>
</section>
