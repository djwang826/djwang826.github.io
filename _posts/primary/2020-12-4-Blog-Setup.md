---
layout: post
title: Setup!
---

How I setup this blog/website, resources used, how I modified it, motivation, etc.

I setup this blog/website after spending a sleepless night thinking about how I never really had any kind of small project that I could say that
**I** made myself. So after accidently sleeping through a meeting, I woke up and asked my friend Gabe how he setup his simple website. He then directed me to his [personal blog post](https://dabe.tech/Making-This-Blog/) where he had detailed what he did step by step. I followed his resources and within five minutes I had my own site running.

Now that I had my own site, I decided to spice it up by adding an archive tab where I could keep a record of any knowledge I had sitting around in my brain. This part took considerably more effort, totaling another hour of fiddling around with the code before I found [another blog](https://stochastic.life/2016/01/06/multiple-blogs-on-single-jekyll-instance/) that showed how to create multiple blogs.

In summary, this method simply separates the different types of posts I have through a new parameter I called *archive* in the **YAML front-matter** block. If the parameter exists in the block, the post will only show in the archive tab. If the parameter does not exist, the post will appear in the primary blog listing, such as this post.

Now with everything setup, I could finally start just writing - which is exactly what I did with this post.

Resources:

1. [Build a Blog with Jekyll and GitHub Pages](https://www.smashingmagazine.com/2014/08/build-blog-jekyll-github-pages/)
2. [How to run multiple blogs on GitHub Pages using Jekyll](https://stochastic.life/2016/01/06/multiple-blogs-on-single-jekyll-instance/)
3. [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)