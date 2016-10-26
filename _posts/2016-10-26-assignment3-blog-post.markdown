---
layout: post
title:  "Getting through Assignment 3"
date:   2016-10-26 19:45:31 +0530
categories: ["blogging", "about"]
author: Amanda Haney
---

I just finished working through Assignment 3.  I'm not going to lie, at times, it seemed like a bit of a doozy.  Definitely was easier than creating my own website, but it still held its own challenges.  

One of the first things involved with assignment 3 was to create a workspace specifically for the assignment.  During class, we downloaded all of the necessary tools into the workspace to allow it to run the pandoc files.

After doing this, I got one of my old essays and turned it into a markdown file.  This was relatively easy because I just dragged the DOCX file over into the folder on cloud 9.  Then I used the following command to convert it to markdown:

```
pandoc -o philosophy-essay.md philosophy-essay.docx
```

This command allowed pandoc to know that I was taking the DOCX file and converting it to markdown.  

After that I renamed a doc.sh script that was already in place, renamed the script and edited the script that only had commands.  I edited the commands to show someone who may go and look at the script what was going to happen, and then told the script what to say and do. Using `# Say hi to user` I told anyone who might look at the script what was about to happen.  Then, saying `echo`, I told the script to say hello and ask the user's name.  After asking the person's name, I told the script using the term `read` and then $USERINPUT and a following command that says `echo "Nice to meet you $USERINPUT" to greet the user by name and then inform the user that the files would be coverted. Using the following commands, I told the script that it would convert the markdown file to a DOCX file, ODT, HTML, and PDF after greeting the user.

```
pandoc -o philosophy-essay.html philosophy-essay.md
pandoc -o philosophy-essay.docx philosophy-essay.md
pandoc -o philosophy-essay.odt philosophy-essay.md
pandoc -o philosophy-essay.pdf philosophy-essay.md
```

After doing this, I went into the original markdown file and made a few edits to it.  I used the code `&ldquo;` to use an opening smart quote and `&rdquo;` to make a closing smart quote.  I also used the `#` symbol before the words I wanted in a header to indicate I would make a header there. I also made a table using `-` and `|` around the font I wanted boxed into indicate that those would be the borders of the table.

After all of this, I ran the script and everything worked out well.  I was able to see that my text formatting was successful in all of the conversions.

The greatest challenge I faced was trying to incorporate an "if-then" script.  I couldn't find the correct structure to allow the script to recognize what to say and do if someone said Yes or No.  It wouldn't recognize the responses.  If more time was available, I have no doubt I could be successful.  I'm planning on working on my own time in the future to figure this out.

It's always nice at the end of these projects to see that, even though the work was challenging, I was successful.  Just like with the website, I was nervous and uncertain about if I could do what had to be done.  But the way the class is structured around collaboration has helped me to be successful.  I work to figure it out on my own, but if I can't, I can go to my classmates and see what they did to be successful.  

Here are the links to the files I converted:

DOCX: https://github.com/inls161/assignment-3-aehaney/blob/master/philosophy-essay.docx <br>
HTML: https://github.com/inls161/assignment-3-aehaney/blob/master/philosophy-essay.html <br>
Markdown: https://github.com/inls161/assignment-3-aehaney/blob/master/philosophy-essay.md <br>
ODT: https://github.com/inls161/assignment-3-aehaney/blob/master/philosophy-essay.odt <br>
PDF: https://github.com/inls161/assignment-3-aehaney/blob/master/philosophy-essay.pdf <br>
<br><br>
Here is the link to the script:<br>
https://github.com/inls161/assignment-3-aehaney/blob/master/aehaney-convert-docs.sh
<br><br>
Here is a link to my C9 Workspace:<br>
https://ide.c9.io/aehaney/assignment-2
