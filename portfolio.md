---
title: Portolio
layout: default
description: My teaching portfolio.
order: 3
published: false
---

## Publications

{% include publications.md %}

## Editorial Work

### Kairos
I am an editor at Kairos: A Journal of Rhetoric, Technology, and Pedagogy.

![Kairos logo](assets/images/kairos-logo.png "Kairos Logo")

### Making Future Matters
In 2017-18, I co-edited a born digital edited collection with Mary P. Sheridan. It was published by Computers and Composition Digital Press / Utah State University Press.

![Making Future Matters logo](assets/images/mfm-logo.jpg "Making Future Matters logo")


## Teaching

{% for course in site.courses %}

  <article class="post-card">
  <h4 class="post-list"><a href="{{ course.url }}">{{ course.title}}</a></h4>
  <span class="postDate">{{ post.date | date: "%b %-d, %Y" }}</span>
  <p>{{ course.excerpt }}</p>
  <a class="read-more" href="{{ post.url }}">Read More</a>
</article>

{% endfor %}
