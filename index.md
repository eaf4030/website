---
layout: default
---

# Hi, I'm Your Name.

I'm a researcher working on **[your field]**. My work looks at
[one sentence about the questions you care about].

Before this, I [short background — degree, institution, or current role].

On this site you'll find my [research](research/) and a [blog](blog/)
where I write about ideas I'm thinking through.

## Recent posts

<ul class="post-list">
{% for post in site.posts limit:3 %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span class="date">{{ post.date | date: "%b %Y" }}</span>
  </li>
{% endfor %}
</ul>
