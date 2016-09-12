---
layout: post
title: Week Three - Bugs, Bugs, Bugs!
---

What did you do this past week?
------
On the technical side, I spent a good portion of my life reading Piazza, working on a mini-shell project for 439 (bless the TAs), and completing Collatz for OOP.

I ended up participating in a skit in 439 in order to simulate many important scheduling algorithms used within operating systems.

I hated it.

Basically, the teacher asked for 7 volunteers who didn't mind looking like fools (maybe I should've paid attention to that last part), and I ended up standing up in the front of class dancing to 'Wheels on the Bus'... not just once, but multiple times. Granted, it was a very good visual in representing First In First Out (FIFO), Round Robin, Shortest Job First (SJF), and Multilevel Feedback Queues with scheduling, process execution, and I/O interrupts, but please... don't ever let me dance to music that goes 'all through the town' ever again.  

On the non-technical side, I attended a prayer gathering for my church (which was great because it was on the day that Collatz was due), played Blazer Tag and ate Magnolia's cafe with my life group, and had a successful night at Slosh social dance (Shoutout to Michelle and Ethan for an awesome dance lesson).


What’s in your way?
------
I found that even though I started working on all my projects early (439 and OOP), I still encountered crunchtime in finishing Collatz (the OOP project).

Collatz was hard, not only in maintaining a routine in testing files on Docker, committing them on Github, and doing continuous integration on Travis CI, but there were multiple things that I did not take account for because of the sheer amount of software that we had to work with.

For Github, there were multiple times where I accidently worked on the master branch instead of my dev branch, thus committing and pushing onto the main source files rather than the separate dev branch space. Additionally, while learning to use different commands such as 'git reset', 'git stash' and 'git commit --amend', I found that many times I would end up corrupting the files in my local space with merge conflicts in files that are auto-generated. Resolving those issues were painstakingly annoying, and I learned that careful planning and design were necessary to carry out any execution, or else 90% of the time will be spent fixing problems that I created.

Furthermore, encountering errors with 'dot' and background files for specific tools like Travis CI and Docker just 'triggered' me to the times during the beginning of spent my internship. About 5% of my time was spent coding, while the rest of the time was spent searching and reading through 10-15 page long wikis in order to figure out how to set up a desktop that I never ended up using. Though I did end up using Travis CI and Docker a lot, it reminded me that inevitably a good amount of software development time is spent learning how to use tools to develop software (APIs, Version Control, Continuous Integration, etc...), and I just had to accept that fact as a software developer.


OOP Class Impressions
------
As much as I delight the learning style Downing executes, I found that several friends of mine did not enjoy it as much. Though I had thought that everyone would learn the best under Downing's style, in reality, not everyone learns in the same way. In fact, it seemed like several of them enjoyed the lecture-heavy, ask-questions-anytime style most professors do rather than the teach-through, get-called-on and get-challenged-by-any-questions-asked style that Downing takes.

Furthermore, there seems to be some tension amongst students and the professor/TAs the past several weeks, which I was not sure if it was because of the recent Travis CI issue, or the situation with the public-repo tests where many tests contained faulty tests or bad format (I'll admit, I was one of them who had both faulty tests and carriage returns ._.).

I hope that rather than defaulting to pointing fingers at one another by saying who's wrong and such, we can understand several things.

(1) The TAs have 180 student's projects to grade, so organizing how pull requests get submitted while answering any Piazza questions can be overwhelming, especially during crunch time at the end of the project. And though you can say it's their job and they made several mistakes, the TAs are trying their best, and being students also, they have their own work that they need to accomplish, while grading all our projects (which are obviously a priority for us). Thanks Onur Domanic, Reza Mahjourian, Cindy Wu, and Peter Scamman!

(2) We are like a mini-student community in class, and in being so, we can do many things to help one another get through the same problems that we encounter. Encouragingly enough, this happened a lot, especially with Travis CI, Docker issues, invalid test cases, and many other problems resolved by students on Piazza. A big shoutout to Simon (Xuming) Zeng (for too many things to count for), Brian Cui (for catching test cases), Ryan Le (main Travis CI communicator), Megan Chen (for step-by-step project setup), George Farcasiu (for the acceptance test script) and many others that I can't cover (because there's too many of you), who've helped out on Piazza and behind the scenes. Thanks guys! *thumbs up sign*


What will you do next week?
------
I plan to schedule out times to meet with my partner in working on Project 2 for Collatz. Hopefully after experiencing the first project, set up should be easier to go through and a greater amount of time can be used to design, code, and optimize the project.

On top of that, I aim to finish my first 439 project, creating my first mini-shell and answering all design questions.

Additionally, I will be preparing for the career fair next Tuesday, creating the perfect elevator pitch, bringing my resume up to date, and studying 'Cracking the Coding Interview' in order to be at my best shape during interviews.

Finally, I hope I can manage my time well enough so that not only I can do all those technical, school work stuff, but also I can spend time with my church family as well as practice dance moves for the one step lesson this Saturday for Slosh.


Tip of the Week
------
As you may know, I am a productivity fanatic, and I find that there can be a lot of time saved if we didn't have to study. Studying is hard (not gonna lie) and I know I would much rather spend hours of my time on the weekend [speed-watching](https://chrome.google.com/webstore/detail/video-speed-controller/nffaoalbilbmmfgbnbgppjihopabppdk) YouTube videos of [Ted Talks](https://www.youtube.com/watch?v=eIho2S0ZahI), [Cooking videos](https://youtu.be/eQgIwwKmjdo), or [Better ways to resolve traffic](https://www.youtube.com/watch?v=iHzzSao6ypE) rather than studying. But what if we could improve our studying?

I was introduced to a [Study Hacks Blog](http://calnewport.com/blog/archive/) last year, and I wish I knew about it before college. Not only were there tips on studying, paper writing, note-taking, and test taking, but there were also tips about college admissions, interviews, and fighting procrastination. All the solutions for problems that I wanted solved were all given to me right [here](http://calnewport.com/blog/category/tips-time-management-scheduling-productivity/). Also, the author is a Computer Science professor, and he's written several interesting books that I recommend [checking out](http://calnewport.com/books/). ('So Good They Can't Ignore You' is very mind blowing for people who try to follow their passion).

