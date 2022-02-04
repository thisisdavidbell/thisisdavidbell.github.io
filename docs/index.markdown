---
layout: page
title: Welcome
permalink: /
---

A github pages site, managed using Jekyll.

#### Useful doc:
- pages: [https://pages.github.com/](https://pages.github.com/)
- links to using Jekyll: [https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll)

---
Including latest post on the front page...
Using method from: [github gist](https://gist.github.com/nimbupani/1421828/733af8c41a7021a554df513a5cdcab5ca9facdf4)

<div class="blog-index">  
  {% assign post = site.posts.first %}
  {% assign content = post.content %}
  {% include post_detail.html %}
</div>

--- 

## Latest Blog Posts:

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

---

This is the base Jekyll theme. You can find out more info about customizing your Jekyll theme, as well as basic Jekyll usage documentation at [jekyllrb.com](https://jekyllrb.com/)

[jekyll-organization]: https://github.com/jekyll
