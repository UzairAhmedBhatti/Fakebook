# Fakebook
Console-based Social Network Application

Project Description
We need to develop a console based social network application. Each User in the application has a unique ID and name. He may have other users in his friend list, having 10 friends at max. He has a list of pages which he has liked (10 pages at max). Each Page has a unique ID, title, list of posts it has shared and total number of people who have liked it. Each Post has a unique ID, description, no of likes, list of people who have liked it and shared date for example; a post is shared at 25th October 2017. A user or a page can share 10 posts at max. A post can have 10 comments at max. A comment is posted by a specific user/page. User can delete a comment on his posts. All the Users, Pages and Posts in the application are objects having IDs.
 
Required Functionality:
1-	Set Current User
a.	Ask user about his ID and set him as current user of application. Now everything that we see in the system will be view of this user.
2-	View Home of Current User
a.	Display posts of all friends shared in last 24 hours. For example,
Rabia Adnan shared “<Post ID - Post Description>”
-	Ayesha Butt wrote: “Comment 1”
-	Ahmed Bilal wrote: “Comment 2” and so on

Asif Mustafa shared “<Post ID - Post Description>”
-	Talha Javed wrote: “Comment 1”
-	Faisal Zaka wrote: “Comment 2”
-	Mannan Ahmed wrote: “Comment 3” and so on

b.	Display posts of all his liked pages (or communities) shared in last 24 hours. For example 
FAST-NU shared “<Post ID – Post Description>”
-	Ayesha Butt wrote: “Comment 1”
-	Ahmed Bilal wrote: “Comment 2” and so on

ICC – International Cricket Council shared “<Post ID – Post Description>”
-	Talha Javed wrote: “Comment 1”
-	Faisal Zaka wrote: “Comment 2”
-	Mannan Ahmed wrote: “Comment 3” and so on
3-	Like a post
a.	Ask user about ID of post and like it. A post can be liked by 10 users at max.
4-	View the list of People who liked a post
a.	Take Post ID from user and display list of people who have liked it
5-	Comment on a Post
a.	Take post ID and comment from the user and add this comment in the post
6-	View a Post
a.	Take post ID and Display the post with its Comments
7-	Share a Post
a.	Take post ID from user and share it
8-	View User’s Timeline
a.	Display User Name
b.	Display user’s posts in his timeline
9-	View Friend List
a.	Take ID of a user and display his friends list
10-	View Page
a.	Take Page ID and display all its posts
11-	Search
a.	Take a keyword from user and display all the People, Pages and Posts having this keyword in their name, title or description respectively.
Important Instructions
•	You are not allowed to use global variables and functions
•	Use best practices studied so far
•	Memory deallocation carrys significant weightage
Sample Run: You are required to bring following output (on your console window) at time of your evaluation.
Phase I includes output highlighted in Blue. U7 is just a sample, your program should properly run on any user.
Command:                Set current user “u7”
Abdullah Nadeem successfully set as Current User

Command:                Set current System Date 15 11 2017
System Date:            15/11/2017

Command:                View Friend List
-------------------------------------------------------------------------------------------------------------
Abdullah Nadeem – Friend List

u3 - Waheed Khan
u11 – Ahsan Ali
u12 – Kamal Subhani
---------------------------------------------------------------------------------------------------------------

Comand:                  View Liked Pages
---------------------------------------------------------------------------------------------------------------
Abdullah Nadeem – Liked Pages


P1 – Food Fusion
P2 – Al Jazeera English
P5 – Rumi Quotes
P9 – BBC News
---------------------------------------------------------------------------------------------------------------

Command:                View Home
---------------------------------------------------------------------------------------------------------------
Abdullah Nadeem – Home Page 

//This is displaying posts of 15th and 14th November
--- s shared “Waheed Khan is excited about CP Project“
                                        Amna Akram wrote: “Best of Luck”
                                        Abdullah Nadeem wrote: “Interesting”

--- Ahsan Ali shared “Waiting for Weekend”
                                        Saad Ali wrote: “Any plans for Get Together?”
                                        Abdullah Nadeem wrote: “Yes BBQ”
                                        Nimra Batool wrote: “Lunch Buffet please”

--- Kamal Subhani shared “Waiting for Result”

--- Food Fusion shared “Food Fusion is making Kashmiri Chai (Pink Tea).”
                                        Food Fusion wrote: “Followrs please try this recipe and give your feedback”
                                        Amna Akram wrote: “Yummy”
                                        Ahsan Ali wrote: “One pink tea for me”

--- Al Jazeera English shared “Oil drilling in Alaska's indigenous communities is on the table again.”

--- Rumi Quotes shared “Be free of possessing things - Rumi”
                                        Kamal Subhani wrote: “Rumi is great”
---------------------------------------------------------------------------------------------------------------
Command:                  View TimeLine
---------------------------------------------------------------------------------------------------------------
Abdullah Nadeem –Time Line

--- “Happy Birthday to my dear Mom” … (14/11/2017)
                                        Waheed Khan wrote: “Happy Birthday Aunty”

--- “Happy Birthday to my dear Father” … (14/10/2017)
                                        Ahsan Ali wrote: “Happy Birthday Uncle”

---------------------------------------------------------------------------------------------------------------
Command:                   ViewLikedList(post5)

Post Liked By:
U2 – Amna Akram
P1 – Food Fusion
U3 - Waheed Khan
U4 - Burhan Tahir
---------------------------------------------------------------------------------------------------------------
Command:                   LikePost(post5)
Command:                   ViewLikedList(post5)

Post Liked By:
U2 – Amna Akram
P1 – Food Fusion
U3 - Waheed Khan
U4 - Burhan Tahir
u7 – Abdullah Nadeem
---------------------------------------------------------------------------------------------------------------
Command:                   PostComment(post4, Good Luck for your Result)
Command:                   ViewPost(post4)

Kamal Subhani shared “Waiting for Result”
                                        Abdullah Nadeem wrote: “Good Luck for your Result”
---------------------------------------------------------------------------------------------------------------
Command:                   PostComment(post8, Thanks for the wishes)
Command:                   ViewPost(post8)

--- “Happy Birthday to my dear Mom”
                                        Waheed Khan wrote: “Happy Birthday Aunty”
                                        Abdullah Nadeem wrote: “Thanks for the wishes”

---------------------------------------------------------------------------------------------------------------

Command:                   SharePost(post5)
Command:                  View TimeLine


Abdullah Nadeem –Time Line

--- “Happy Birthday to my dear Mom” … (14/11/2017)
                                        Waheed Khan wrote: “Happy Birthday Aunty”

--- “Happy Birthday to my dear Father” … (14/10/2017)
                                        Ahsan Ali wrote: “Happy Birthday Uncle”

--- “Food Fusion is making Kashmiri Chai (Pink Tea).” … (15/11/2017)
---------------------------------------------------------------------------------------------------------------
Command:                   ViewPage(p1)

Food Fusion
--- “Food Fusion is making Kashmiri Chai (Pink Tea).” … (14/11/2017)
                                        Food Fusion wrote: “Followrs please try this recipe and give your feedback”
                                        Amna Akram wrote: “Yummy”
                                        Ahsan Ali wrote: “One pink tea for me”

--- “Food Fusion is making Halwa Puri.” … (10/11/2017)
---------------------------------------------------------------------------------------------------------------
Command:                   Search(“Birthday”)

Posts:
--- post8 - Abdullah Nadeem shared “Happy Birthday to my dear Mom”
--- post11 - Haris Muneer shared “Happy Birthday Ali Bhai”
--- p11 - Birthday Cakes

---------------------------------------------------------------------------------------------------------------
Command:                   Search(“Ali”)

Users:
--- u2 - Muhammad Ali
--- u6 - Saad Ali
--- u11 - Ahsan Ali
Posts:
--- post11 - Haris Muneer shared “Happy Birthday Ali Bhai”
Pages:
--- p12 - M Ali Jinnah



Instructions:
1-	All the arrays should be dynamically allocated.
2-	Wherever you need an array of objects, keep it as double pointer. For example if a page has no posts or if a user has no friends and no liked pages then these double pointers should be null.



