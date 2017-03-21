---
layout: post
title: Who Needs A Break
---

What did you do this past week?
------
This past week, I ended up doing a lot of activities and not much homework.

For the first half of Spring Break, I spent it with my parents outside of Austin at Black Rock Park. We lived in a cottage that was set right next to a lake, and it was pretty frightening living there because the day we moved in, there was a ton of rain pouring and the waves from the lake looked like they would crawl up the shoreline and swallow our tiny cottage whole. Fortunately, that didn't happen (though the nights were really chilly). We spent our time using the cottage as a home base, and going out to Enchanted Rock and Fredricksburg and exploring many different sites within the rural country of Texas.

After that, on Tuesday and Wednesday, I got to go to SXSW's hackathon with a friend of mine, and we competed against over 20 teams. The theme of the hackathon was Music, Film, and VR/AR, and though initially we didn't have a full team, we ended up creating one last minute and working on a pretty nifty problem in the music industry. The problem is that every year, several million dollars are lost on royalty rights because of uncounted song plays at live music performances. This means that a huge amount of credit that artists deserve doesn't get allocated. Our hack solves that problem.

Hosted on a web app platform, we take input of twitter hashtags. Using these Twitter Hashtag feeds for live event, we call Twitter's API to scrape text, and analyze tweets to assert from it what songs are played and connect it to the artist associated to it. Using Mapquest API, we only assert twitter tweets from areas aggregated around the venue the event is based on, sub-setting the tweets that needs to be analyzed. With PubNub's real-time communication API, we send the data over to our computer server, which analyzes the tweets, and send the data back to our web app, updating it so that it displays all the songs, artists, and other relevant information that can be formatted into a readable form. Afterwards, behind the scenes, we take that data, store it into a JSON format, and send it off to SOCAN, one of the leading licensing companies for artists, who can use the data assert the royalty rights, and in doing so, get artists the credit that they deserve.

It was a really fun experience overall. Throughout the hackathon, I got to meet so many amazing people, such as company founders, fellow hackers, and worked really closely with some companies over their APIs. Additionally, there's no such thing as a SXSW event without any music, and we ended up having a live performance by a band called New Thousand. In the end, after 24+ hours of hackathon, countless battles of sleep deprivation, and an enormous amount of food and sugary drinks consumed, I'm proud to say that our hack ended up winning. If you're interested in reading more on the project, here's the [Devpost](https://devpost.com/software/credit-writer) and [Github](https://github.com/theCreedo/Credit-Writer) link.

After a long day of no sleep, and a night of rejuvenation, I ended off the Spring Break with a staycation in Austin with my Sophomore class from Harvest Church. We ended up doing a lot of things, such as cooking together, eating a lot of food (with leftovers), doing devos, roller skating like noobs, having movie nights, playing countless games of Hot Seat, having a "formal" dinner night at Maggianos for no reason (that's what we said to the waitress), paddle boarding the bright surface of Lake Travis, getting sunburned, making last-minute cancels on plans so we can just stay inside and chill, and all in all, spending the our break getting to know one another better and deeper than we ever could during the school year. I'm glad that I was able to finish my Spring Break with them.


What’s in your way?
------
I didn't do any work over Spring Break. Though I did finish a faculty profile article for UTCS as well as facilitated and communicated over my SWE website project, I traveled and spent a lot of time doing so many activities that I never really had much time to stop and sit, pull out my computer, and work on the assignments I had (especially since I didn't have internet or a computer half the time).


Spring Break Impressions?
------
Not including Spring Break Missions last year (which was a completely different experience), I found this Spring Break to be one of the most fun I've had in a while. This was one of the few times over break where I didn't just sit around and do nothing, so I'm really glad I was able to go out and do a lot of fun activities with my family and friends, and I'm definitely hoping to keep one of these under my memory belts (if there is such a thing as that).


What will you do next week?
------
Catching up on homework. The SWE website project is due on Thursday, and we still have a lot of tasks we have to complete as a team. I will be finishing up documentation on the API we will be implementing, as well as working on Flask so I can get some type of communication between the Database we will create and the front end of our website. Finally, I will write up a small chunk of the technical report involving the RESTful API design, and hopefully meet up with my teammates in order to assign and finish off all the tasks that were assigned for this given phase.

I will also be studying for Algo. This 2nd phase of the class has been focused a lot on the aspect of Flow Networks, and though I understand the concept and how to approach the problem, I still struggle with proving by correctness the graph I create as well as interpreting many of the logic flows that I have to go through in explanation of the problem.

Finally, I hope that even with all the fun and tiredness that I experienced from Spring Break, I will be able to reorient myself back to a mind that is productive and working at semi-full to optimal capacity so I can use my time to do all the programming, reading, blogging, learning, and studying I can.


Tip of the Week
------
One of the hardest things I find as a developer when working on a project, is setting up the environment when coding, whether it's deciding to work on Maven or Gradle, choosing what IDE to work with, or finding the required packages needed in order to complete a project. During these times, I find that I run into errors a lot, and it really annoys me, since I want to focus on the project I have to work on rather than the set up itself. One of the best things I've found that have helped me through these times is having perseverance, mentors, and Google. Here's the process I go through during these hard times.

Whenever faced with a bug, I don't allow myself to become down, but take it as an opportunity to learn, and persevere after it. I first take the text associated with the error, copy pasta it, and search about it on Google. Usually someone else in the world will have experienced the same error I've gone through. Afterwards, I will take time and look through the comments, questions, or StackOverflow posts related to the error, and try to replicate the solutions they say.

If that doesn't work, I try to look for experienced people (especially at an internship or hackathon) who can help me work through the problem if they've encountered it before also. Afterwards, if I can't seem to find the answer, I turn to my trusty old friend, StackOverflow, to give me a good boost of help (or demoralization) and hopefully within the next few hours or limited amount of days I have, wait for an answer and try to focus my time on another task that isn't blocked by the bug. Most of the time, something good happens through this process. If not, I usually spend the rest of my time wondering how in the world the bug is produced and either, A. continue to try to fix the bug, or B. move on over the next 99 bugs I have to work on for a project.

Hope the tip helps!
