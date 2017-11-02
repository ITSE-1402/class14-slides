---
title: 'Class 14: Cloud Services and Your Code / Getting a Job As a Programmer'
separator: '\-\-\-\-\-'
verticalSeparator: '\+\+\+\+\+'
theme: 'moon'
revealOptions:
    transition: 'fade'
---

### ITSE-1402 Intermediate Python
<span style="font-family:Helvetica Neue; font-weight:bold; color:#e49436">Class 14: Cloud Services and Your Code / Getting a Job As a Programmer</span>
<br /><br />
##### [https://z3r0.tech/slides-14](https://z3r0.tech/slides-14)

-----

## Cloud Services and Your Code

+++++

Today we will be talking about AWS Elastic Beanstalk and Google Cloud Platform App Engine.

Note:
Both of these services have free tiers and both are relatively simple to use. 

+++++

### Google Cloud Platform - App Engine

+++++

##### What is App Engine?

- Hosting for your code
- Fully managed infrastructure
- Supports many languages and frameworks
- Works with docker images
- Scales effortlessly as your app grows
- Painless!

+++++

https://youtu.be/2PRciDpqpko

+++++

##### What languages does it support?

- Node.js
- Java
- Ruby
- C#
- Go
- Python
- PHP
- .net

+++++

##### Why use it?

- Focus on code and not infrastructure 
- Docker support!
- Monitoring and application insights with Stackdriver
- Instant versioning of your running application
- Ability to do staggered rollouts of new versions
- Easily use and integrate with many other GCP services
- Lots more!

+++++

https://youtu.be/sATG0OfdP4g

+++++

##### Getting Started

To get started with the google cloud API, download the SDK here:

[https://cloud.google.com/sdk/docs/](https://cloud.google.com/sdk/docs/)

+++++

### AWS - Elastic Beanstalk

+++++

#### What is it?

- Hosting for your code
- Fully managed infrastructure
- Supports many languages and frameworks
- Works with docker images
- Scales effortlessly as your app grows
- Painless!

+++++

https://youtu.be/SrwxAScdyT0

+++++

#### Why use it?

- Focus on code and not infrastructure 
- Docker support!
- Application Health Monitoring
- Ability to control every level of your stack
- Easily use and integrate with many other AWS services
- Lots more!

+++++

#### What languages does it support?

- Node.js
- Java
- Ruby
- C#
- Go
- Python
- PHP
- .net

+++++

#### Getting Started

To get started with the AWS EB CLI, install it here:

http://docs.aws.amazon.com/elasticbeanstalk/latest/dg/eb-cli3-install.html

-----

## Getting a Job As a Programmer - Tips, Tricks, and Practice

+++++

### Before the Interview

- Study the company
- Study the interviewer
- Make insider connections
- Gain experience (if you don’t have it already)
- Read through and study a book
- Practice, practice, practice

Note:
Study the company and learn as much as you can. Knowing about the company and showing passion for it’s mission can go a long way.
Study your interviewer and learn as much as you can. Knowing about them and mentioning a blog post or something of theirs creates a connection and that will go a long way (don’t be creepy though!)
If done right this can show that you are thorough and detail oriented as well as show a great interest in the company. If done incorrectly though, this can easily tank an interview. Be careful!
If you have a heads up, try to make connections on the inside. These connections can make a big difference if the referrer has pull and good things to say about you.
Gain experience if you don’t have it. Join or start an open source project. Start a blog. Build a small web app. Do or make something to show that you know your stuff. 
Cracking the coding interview is renownedly viewed as one of the best coding interview prep books
Practice, practice, practice...

+++++

You will be asked algorithm questions. 
Know the general concepts:

- Binary Search
- 2D Arrays
- Hash tables
- Dynamic Arrays
- Linked Lists
- Dynamic programming
- Big-O analysis
- Quicksort, merge sort


Note:
While you may not have (or even really need) formal CS experience, you will need to know the basics of algorithmic concepts. Some of these we briefly touched on such as hash tables and big-o analysis. Some of these we didn’t really, but the book has some info on. In general, be sure you have a pretty good understanding of these.

Strings
- Get comfortable manipulating a string as an array of characters, one character at a time (like C-style strings).

Numerical arrays
- Think about iterating backwards over the array elements as well as forwards. Backwards iteration is useful for, say, merging the contents of two arrays "in-place" (i.e., using O(1) outside storage).
- Would the problem be easier if your array were sorted? If so, you can always tell the interviewer that you'd first do an O(n lg n) sort. Heapsort is an asymptotically optimal "in-place" sort. Once your array is sorted, think about how you can use a variant of binary search to get O(lg n) performance rather than O(n) for an algorithm based on linear scanning.

Mappings and sets (hash tables)
- Always think of mapping keys to values to make your life easier. If you can scan through your dataset and create an auxiliary hash table to map keys to values, then you can do O(1) lookups in a latter part of your algorithm.
- For some array-based problems, you might find it useful to create a "reverse mapping" between array elements and their indices. e.g., "the number 42 appears at index 6 in the array" is represented as a mapping of "42 -> 6".
- You can use a hash table as a set to do O(1) membership lookups. If you are being tested on low-level skillz, use bitsets and the proper bit-level operations to operate on them.

Linked lists
- Linked list problems almost always involve singly-linked lists.
- If you are implementing an iterative algorithm to operate on a singly-linked list, chances are that you'll need to walk two pointers, which I like to call cur and prev, down the list until one is null.
- Some problems require you to keep a gap of N elements between your cur and prev pointers.
- Some problems requires your cur and prev pointers to advance at different speeds. e.g., moving prev up by one element while moving cur up by two elements.
- For most recursive algorithms, the base case is when the pointer is null.
- Sometimes you might need to keep a pointer to the final (tail) element of the list as well as to the head.

Binary trees
- Remember that not all binary trees are binary search trees, and know the difference between the two.
- Know about the idea of a balanced binary search tree (e.g., AVL tree or red-black tree), but don't worry about being able to implement one during an interview.

Graphs
- Whenever you need to represent binary relationships, think about using a graph. e.g., X is friends with Y, or X has a crush on Y, or Task X needs to be done before task Y.
- Now that you have a graph representation, what can you do with it? Chances are, you won't be asked to implement any sort of sophisticated graph algorithm since you simply don't have time in a 1-hour interview to do so.
- Definitely know how to implement a depth-first search using a stack data structure (or using recursion, which implicitly uses your function call stack)
- Definitely know how to implement breadth-first search using a queue data structure.
- Draw a few examples of graphs for your particular problem and see what common structure arises, then tailor your algorithms to that type of structure. For example, you might find that the graphs for your problem are all acyclic, or that they always have one unique source and sink node, or that they are bipartite (e.g., for 'matchmaking' problems), or that they are actually trees in disguise :)
- Know about the idea of topological sort.

Edge cases
- Always test your algorithm on edge-case examples. e.g., what if the user passes in an empty list or tree, or a list/tree with a single node?

+++++

Search for the company's interview questions online.

Note:
Generally companies that interview quite a few people will have a lot of the questions they asked documented on sites such as Glassdoor. Take advantage of this.

+++++

### The Phone Interview

Don’t assume it will be easy!
It can be anything from questions to coding
It will not be HR on the other end
This is where you can easily be weeded out

Note:
Don’t assume that it’s going to be a breeze. In fact, assume it will be hard. Anything can be included in the phone interview, even code!
Document is usually shared with you to code or a quiz
It typically won’t be HR, but rather a peer as it is technical
That’s the point of phone interviews. Even if you are very knowledgable, you can still do poorly in this portion

Looks for:
Knowledge of computer science fundamentals, such as data structures and algorithms.
Analytical skills.
Coding skills.
Cultural fit.

+++++

### The In-Person Interview

Who is there?
- Hiring Manager
- At least one member of your potential team
- Someone on a completely different team
- You!

Note:
At this point you hopefully are at least pretty well acquainted with the hiring manager. This isn’t who you should focus on though. The most important person in the room is the one not even on the team. They’re going to be your toughest critique because: 1) they aren’t even related to the team 2) they might not have the same bias (team might be short staffed) and 3) they typically have NO bias

+++++

### The Quizzing

- Avoid the trap questions and have good answers
- Know Computer Science basics
- Know concepts around programming
- Be honest ...
- But don’t be too honest 

Note:
Avoid the trap questions and always have good answers prepared. What is your greatest strength/weekness. Why are you looking for a new position? Tell of a time when you had a disagreement with a co-worker and how you handled it. 
Know computer science basics. You don’t need to know it all, but know show that you understand it. 
Know the concepts around programming. Specifically around what you are applying for. Databases, web servers, load balancers, etc are good to know for full stack. 
Be honest. If you don’t know the answer to the question, this is okay. Oftentimes they ask questions above what they expect you to know just to see how you respond. Talking through a potential answer after acknowledging lack of knowledge is the best way to handle this. 
Don’t be too honest. Telling the truth is good, but going the extra mile and providing unnecessary bad information will not help you. Don’t volunteer negative information that was not requested. 

+++++

### The Code

- Take time! Don’t stress!
- Ask questions to the interviewer
- Explain your approach(es) to your interviewer
- Draw your approach if you can

Note:
Ask questions to the interviewer. Clarify the ask.
Explain your approach(es) to your interviewer. Talk about tradeoffs between approaches. See if you can solicit feedback on which they are looking for or prefer (if any). 
Draw your approach if you can. It will help you understand the question better and it will better demonstrate the your understanding. If there are issues with your understanding, it allow the interviewer a chance to explain further. 

+++++

### The Code (cont)

- Code and explain as you go along
- Don’t be afraid to start over if you need to
- Ask questions along the way if you need to
- Once done coding, walk your interviewer through it
- Review code for issues and fix any found

Note:
Code and explain as you go along. If you have to pseudo code at first, explain that you are doing so and code it out after words. 
Don’t be afraid to start over if you need to. Keep talking though.
Ask questions along the way if you need to. Even ask for hints should you need them. Just don’t stress out.  
Once done coding, walk your interviewer through it
Review code for issues and fix any found. Interviewers expect to see bugs. Finding and fixing them makes a great impression. 

+++++

### After the interview

- Don’t think about how you did
- All interviews are graded on a curve
- If the news is bad, it’s not always your fault
- Walk away with your head high

Note:
Don’t think about how you did or worry about things you might have messed up. You’re typically wrong and it won’t help you one bit. 
All interviews are graded on a curve where the curve is set by the other candidates. You don’t know how good (or bad) the others did and thus have no idea how well you did. 
Once you hear back, if it’s negative it’s not always you. Sometimes others may have just been slightly better. Sometimes the interviewers might have thought you didn’t handle the problems quick enough and thus possible think you might not be competent enough. Sometimes team fit can be an issue. Maybe you came off as a bit arrogant or you might have been too up tight. Try to get as much feedback as you can (if possible) and use it to improve yourself!
Walk away with your head high. You just completed a tough test and regardless of how well you did you did well. 

+++++

### General Tips

- Confidence is key
- Be enthusiastic
- Read everything you can until you feel ready
- Practice a lot and then practice again
- Practice the same way you will be interviewed

Note:
Confidence is key, but don’t be overconfident. Many times candidates are turned away for soft skills issues vs technical skills
Be enthusiastic. Along the same lines as confidence, being enthusiastic will go a long way.
Practice a lot. Practice everything. Practice multiple times. Practice everything you can find.
https://www.amazon.com/Cracking-Coding-Interview-Programming-Questions/dp/0984782850/
Practice the same way you will be interviewing (whiteboard, gdocs, etc). You will not have any IDE assisting or compiler (regardless of how little sense this makes). If no whiteboard, use paper.

+++++

https://youtu.be/XKu_SEDAykw