---
layout: post
title:  "The Best Place to Start is the Beginning!"
date:   2016-09-24 19:45:31 +0530
categories: ["blogging", "science", "about"]
author: Amanda Haney
---

Well, it's official.  This website is up and going and so that is something worth being proud of (right?).

These past few weeks have been a huge learning curve.  I came into this class with virtually no experience with command lines, HTML, Markdown, or anything like these.  I was extremely nervous when I started going over the syllabus.  I thought to myself, "I have to build my own website??" It sounded horrifying!  But before I even realized it, I was being equipped with the tools necessary to do just this!

We started off learning the command line.  We practiced basic things like `pwd`, `cd`, and `ls`. These were basic things that taught us how to navigate.

More recently we've moved on to learning how to use Git as our version control system all working in a Github repository.  These things sounded extremely (and I mean EXTREMELY) intimading and difficult.  That overwhelmed feeling I had at the beginning of the semester?  Well, let's just say it came back.  

Honestly, though, I'm confident that whatever happens, I'm going to be okay.  I'm recognizing that this is all a trial and error process.  The best thing about the requirements of this class are that you learn through hands-on learning.

I think what I'll start off sharing for my website is how I created it!  

First, I selected by layout (I chose to use the Gravity theme) and cloned it into a new Cloud 9 workspace.  I then pushed it into my own repository. Part of this process also involved running `jekyll serve --host $IP --port $PORT`.  From there, while in my Cloud 9 workspace, I opened `_config.yml` and changed the base url to the appropriate url with my github username.  After all of that, I followed a few steps to crate this post!

```
cd Gravity
cd _posts
```

Then I created a new post which I named 2016-09-24-first-blog-post.markdown.  I opened up the blog post, filled out the content that you're seeing here and saved it.  After that, I typed the following in my terminal:

```
git status
git add .
git commit -m "Inserted relevant content with reflection on class so far"
git push
```

I filled out the appropriate information and the information was available on the website like you are seeing now.

It always feels good to have little successes like this.  It's those moments where I'm convinced these things are way too over my head for me to be successful, yet I find myself being successful, that mean the most.

It will definitely take more practice, but I'm feeling confident about the path that I'm on.
