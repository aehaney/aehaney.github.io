---
layout: post
title:  "I love group work and assignment 4"
date:   2016-11-2 19:45:31 +0530
categories: ["blogging", "about"]
author: Amanda Haney
---

Assignment 4: Probably my favorite assignment so far.  I think the reason behind this is the fact that, for the most part, it was a group project.  I love the collaboration and the teamwork that comes with a group project, especially when you have a great group (I did). 
<br><br>
We started off by having most of the work take place in Brynna's workspace.  After cleaning up the repository, we created a list of five questions.  At first they were the same questions from the practice run earlier, but we changed them to five other random questions that (we thought) were sillier.
<br><br>
After that, we moved on to the next step of writing a random string of characters to a variable as a unique identifier.  This area was definitely one of the challenging areas.  After a long period of searching through the readings and navigating our good friend Google, we used the following:
<br>
```
random()
{
        cat /proc/sys/kernel/random/uuid
}
    echo "$(random)"
```
<br>
Doing this gave a unique identifier to the questions that were answered when one runs the script.  The next step was to add the date time stamp.  This was much easier, as one of our group members had previous experience and was able to talk us through how she found it and did it.  In the script we wrote
```
# Saving the date the user answered the questions
today() {
        date +%m-%d-$Y
}
```
<br>
This showed the month, date, and year on the date-time stamp.
<br>
The final step was probably a little bit more challenging.  We were consistanly so close to getting it done, but we were always just a little bit off.  In order to make sure the answers the user typed ended up in a separate CSV file, we first tried something that ended up putting the entirety of the script in a separate CSV file.  We finally realized that if we put
```
echo $(random),$(today),$name,$color,$fear,$major,$food >> scriptanswers.csv
```
it would move the answers of the user into a separate file called "scriptanswers.csv".  This was a pretty easy fix, but was definitely one that took awhile to figure out. I would say, though, that it was our major "AHA!" moment because it's the area we spent the most time researching and we were so close to figuring it out nearly the entire time.
<br>
<br>
I really can't emphasize how much I enjoyed working in a group.  I've definitely enjoyed the other projects, but I liked how this offered a new level of teamwork and collaboration.  We all were able to use each other's strengths to move forward when one of us felt stuck.  

Because we didn't fork the repository and only cloned it into our workspace, I'm linking to what's actually Brynna's repository.  This is cloned into my Cloud9 workspace, but, as I said, not forked into my own repository.  
https://github.com/brynnaw/BlueBlueGreen-Assignment-4


Also, here's a picture of President Obama since I missed part of class.
![Alt Text](https://scontent.xx.fbcdn.net/v/t1.0-9/14947500_10211490891136234_1384724898768224553_n.jpg?oh=3bccfcc4299cecec5ae6919b58c95571&oe=588C7DA9)