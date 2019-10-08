---
title:  "Notes on the Design of This Site"
layout: post
description: Notes on how I designed this website.
category: Web
author: Rick Wysocki
comments: true
excerpt_separator: <!--more-->

---

## Switching Up

I'm a hobbyist developer / programmer. A byproduct of this is that I don't typically have a "real" web project to work on, so I end up designing and redesigning my own website to try out new techniques, frameworks, and libraries.

I'm ending this annoying practice. <!--more-->It doesn't promote actual writing (the apparent purpose of a blog) and just ends up a confusing mess of content strewn across multiple sites and folders.

Instead, I've decided to commit to a simple but functional site design: more or less what you're seeing now. I may make minor changes as I notice problems, but ultimately I'm attempting to shift my focus to writing. Hopefully, this will force me to finally start some more interesting digital projects.

## Design Notes

I'm going to use this post to collect information regarding my site design, in case others' want to reference it for their own projects. Due to work contraints, this will probably roll out over a few phases, starting here with a basic list of the tools and technologies I used in this site design. It's a living document, and I'll timestamp revisions as I add them. If you want further explanation of something, feel free to mention it in the comment box below.

### Tools and Technologies

I used the follow tools and technologies in the design of this site.

- [Jekyll](https://jekyllrb.com/): Jekyll is a Ruby-based static blog generator. I love it. Everything is neat and tidy, and I get to write in Markdown. Jekyll gets deployed to Github Pages (see below).
- [Gutenberg Typography](https://github.com/matejlatin/Gutenberg/wiki): I'm lazy and hate setting up typography for sites, so I used Gutenberg. Because the Grunt-based compiling wasn't reliably working for me (definitely user-error: I didn't know what I was doing), I just scraped all their good CSS out into a new, static CSS file after a successful compile. It looks great though--many thanks to the Gutenberg folks.
- [SCSS](https://sass-lang.com/): After I scraped out all of that compiled CSS, I wanted to make it more manageable for site-wide updates. So I reformatted the page as a dynamic SCSS stylesheet.
- [Jekyll Scholar](https://github.com/inukshuk/jekyll-scholar): It's doing all the citation. Works great besides a few very minor quirks.
- [Github](https://github.com/) / [Github Pages](https://pages.github.com/): The repository that I push my site to. Not that much to it, except that Jekyll-Scholar won't compile on Github Pages. So I'm building my site with...
- [Netlify](https://www.netlify.com/): All my site building is handled with Netlify, which pulls from my Github repository. This makes Jekyll Scholar functional, as well as any other Jekyll plugins I add
