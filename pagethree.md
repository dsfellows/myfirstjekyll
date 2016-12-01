---
layout: page
title: Page Three
permalink: /pagethree/
random-fact: "Laurie loves elephants."
picture-of-laurie: "/assets/images/laurie-talky.jpg"
---

## Sample Content
Here is a picture.
![legend](/assets/images/land-use-key.png){: .img-responsive .text-right .img-square}


###  Here is a random fact

<strong>  {{ page.random-fact }} </strong>

### Here is a random fact from the data.

<strong> {{ site.data.data.Person3.random-fact }} </strong>


### Here is a list of posts.

Notice how, on the website, it's got the text of a blog post, but on the makdown page, it's just some code.
The curly brakets and percent signs indicate commands that jekyll will follow as it builds the site. site.posts means things in the posts directory, etc. There's more described [on the jekyll variables page](https://jekyllrb.com/docs/variables/).

<ul class="post-list">
  {% for post in site.posts %}
    <li>{{ post.date | date: "%b %-d, %Y" }}
      <h3>
        <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h3>
    </li>
  {% endfor %}
</ul>

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>
