---
layout: page
title: Contact
permalink: /contact/
feature-img: "img/sample_feature_img_2.png"
---

Type Theme is a free and open-source theme for [Jekyll](http://jekyllrb.com/), licensed under the MIT License.

Head over to the [theme's documentation](https://rohanchandra.github.io/project/type/) for much more information about Type Theme or to install this theme on your own Jekyll site.

This file is an example of a page in Jekyll, that automatically shows up in the header navigation, you can delete or modify this file freely.


  <div class="posts">
    {% for post in paginator.posts %}
    <div class="post-teaser">
      <header>
        <h1>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">
            {{ post.title }}
          </a>
        </h1>
        <p class="meta">
          {{ post.date | date: "%B %-d, %Y" }}
        </p>
      </header>
      <div class="excerpt">
        {{ post.excerpt }}
        <a class="button" href="{{ post.url | prepend: site.baseurl }}">
          {{ site.theme.str_continue_reading }}
        </a>
      </div>
    </div>
    {% endfor %}
  </div>