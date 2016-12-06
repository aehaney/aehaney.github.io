---
layout: post
title:  "What the SQL?"
date:   2016-11-16 19:45:31 +0530
categories: ["blogging", "about"]
author: Amanda Haney
---

Oh.<br><br>
My.<br><br>
Goodness.<br><br>

Is there such a thing as death by coding?  Because if there is, I think I came close.  All jokes aside, this assignment was by far the most challenging one we have yet to undergo. <br>
<br>
From the beginning we were experiencing challenges.  But the great thing about this project was that it forced us to heavily rely on collaboration.  The key part of what we did was go into sql to create a database and then a table to go in our database.  We did so with the following commands:

```
CREATE TABLE scripttable (Name VARCHAR(255),
                          Color VARCHAR(255),
                          Fear VARCHAR(255),
                          Major VARCHAR(255),
                          Food VARCHAR(255),
                          Date VARCHAR(255),
                          UID VARCHAR(255));
```

After creating this table, we put the following in our script to help it connect to the database.  It would use the data from the scriptanswers.csv file to put the data in to the database.  When we ran mysql, we would see our table complete with the data.  

```
echo $name,$color,$fear,$major,$food,$(today),$(UID) >> scriptanswers.csv

# IFS=,
# while read UID today name color fear major food
#     do
#         echo "INSERT INTO scripttable (Name,Color,Fear,Major,Food,Today,UID) VALUES ('$UID', '$today', '$name', '$color', '$fear', '$major', '$food');"
        
# done < scriptanswers.csv | mysql -u aehaney -p scriptdatabase;

mysql -u $username -p -H -e "LOAD DATA INFILE '/home/ubuntu/workspace/bluebluegreen/BlueBlueGreen-Assignment-4/scriptanswers.csv' IGNORE INTO TABLE scripttable FIELDS TERMINATED BY ',';" scriptdatabase

mysqldump -u $username -p scriptdatabase > scriptdatabase.sql

# mysql -u aehaney -p -H -e "SELECT COUNT(*) FROM scripttable;" scriptdatabase
```

As you can see, some of what we put in there is commented out.  This is because these were attempts to try new things that were either not succsesful or we didn't want to completely get rid of in case we thought to come back to them.  

One of challenges in this assignment was seeking out the necessary tools to have the correct code.  We ended up spending over an hour trying to figure out how to stop having duplicates come up in our database table.  It ended up being an extremely easy fix by just adding "IGNORE" in the code.  The other major challenge is that when my groupmates tried to pull the information, we were met with an ERROR.  This is because it was using my username in the code.  We fixed this by replacing where my username was with `$username`. 

This project was crazy.  It required so much teamwork and so much perseverance.  But I was so lucky to have an awesome group that worked together to overcome these challenges.  