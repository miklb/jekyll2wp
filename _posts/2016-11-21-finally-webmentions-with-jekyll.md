---
ID: 1112
post_title: Finally Webmentions with Jekyll
author: miklb
post_date: 2016-11-21 05:41:49
post_excerpt: ""
layout: post
permalink: >
  http://michaelbishop.me/2016/11/21/finally-webmentions-with-jekyll/
published: true
tags:
  - 'a:2:{i:0;s:10:"webmention";i:1;s:6:"Jekyll";}'
summary:
  - "I think I've finally nailed getting webmention working with Jekyll"
---
If you can't tell by previous posts, I've been working on getting
[Webmentions](https://indiewebcamp.com/Webmention) to work with my new Jekyll site. I *think* I've finally nailed. If you take a look at my initial post [on moving to Jekyll](http://miklb.com/making-the-move-to-jekyll), there's a link for a tutorial on using Travis CI to build a branch and move the flat files into the mater branch to be served on GitHub. With the help of a Aaron Gustafson's [Webmention.io plugin](https://github.com/aarongustafson/jekyll-webmention_io) I finally have it working. The trick was that the rakefile was firing in the build process too fast, so webmention.io couldn't find the post on my domain, thus not sending the mention. My probably not so elegant solution was to put a `sleep 2m` in my shell script to slow things down and let GitHub catchup before firing the rakefile and sending the mentions. This post will be my final test. If all goes well, I will try and write up a more detailed explanation of what I've done since there's still a lot missing for doing this with a Jekyll site.

<a href="https://brid.gy/publish/twitter"></a>