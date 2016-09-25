---
layout: post
title: Week Five - Hack my Life Away
---

What did you do this past week?
------
I spent my first 4 AM sesh with my pair programming partner in the computer lab trying to figure out the best way to parse a string in C++ to store into a cache (of course we did other things, but that was one of the tasks we took on). I realized by taking a string, passing it into an istringstream, converting it into a istream_iterator, and storing it as a vector<string>, I can get data in an array through random access. It would've been way more efficient to create a macro to do this, but here's how the code looks uncovered.

    istringstream buf(line);
    istream_iterator<string> beg(buf), end;
    vector<string> data(beg, end);
    cache[stoi(data[0])] = stod(data[1]);

Also, we removed running our diff section in .travis.yml due to the fact that Travis CI would not allow us to access the files within the Travis environment. It's true that we could've set up an environment that would've allowed access to the files, but we figured that our diff file worked both 

In addition to school life, I just finished HackGT, a hackathon at Georgia Tech! Though I was the only UT student there (which makes hackathons pretty lonely not knowing anyone), I was luckily able to find a team to work with. The guys I got to work with were [Manav](https://github.com/manav95/), [Fernando](https://github.com/madpeanuts), and [Ambika](https://github.com/ambikagupta), all Georgia Tech students/ alumni who lived around the area.

We ended up making this cool app called [Hungry Cats](http://devpost.com/software/hungry-cats) and you can  check out the code [here](https://github.com/manav95/HungryCats) on github. (I also have a [Powerpoint presentation](https://drive.google.com/open?id=0B-S5sh0cBWk1Q04tNmdwNld0dGs) that I hashed together 30 mins prior to the hackathon demoing time) Unfortunately we did not win any prizes, but I got to re-familiarize myself with Android development and experience a hackathon in a team for the first time.

I worked in front-end on Android Studio (the bane of my existence) and helped design and edit sprites/images that our objects would represent. I also pair programmed with Manav over some very difficult, undocumented open-source code, an Android-curated java engine called [AndEngine](https://github.com/nicolasgramlich/AndEngine). Here's my two cents on it. Though AndEngine does it's job in providing a Java Physics Engine that is relatively smooth flowing and there has to be some appreciation in all work put into an open-source project, it was probably one of the worst experiences developing with it. AndEngine has absolutely no documentation, making it hard to traverse through the code for methods required in implementation (I now realize I have taken documentation for granted). In addition to the poor documentation, many errors were hard to resolve and Google/StackOverflow (bless these tools) gave results all over the place on how to resolve these annoying issues.

Fortunately, after pulling an all-nighter pair-programming, drinking my 3rd actual cup of coffe in my life, and many breaks to food events (shout out to [Insomnia Cookies](https://insomniacookies.com/) and [Sublime Donuts](http://www.sublimedoughnuts.com/) ), we were able to create a very buggy, yet functional app that has animation, collision detection, and a very aesthetic feel to it.

Naturally in a non-programming perspective, the game was a disaster, and didn't fulfill any needs of the user, providing intolerable gameplay, ghetto-ish animations, and a horrible user experience, (similar to Pokemon Go, except that app became #1 Nationally and people still play it right now...). But to our team, who has a creditable amount of programming experience, the game was an achievement. All our time/energy spent and sleep sacrificed during the hackathon helped nurture an idea into a physical product. Though we were unable to win any prizes (which would've have been the sweetest icing on top), being able to witness 36 hours of brainstorming, designing, and programming bring forth a working game that I can point back to and be proud of made all of it worth it in the end. (I'm pretty sure I ate 10 lbs of fruit snacks (and food) though, so I might have some post-hackathon problems to resolve...)

What’s in your way?
------
10 lbs of fruit snacks/food to burn. Also, because I ended up doing a hackathon over the weekend instead of working on my 439 project, I will have to get my game on for that. Fortunately, I have thought over some of the logic for the 2nd and 3rd part, so hopefully implementing it won't be too hard (though that's speaking positively for one of the hardest classes of a CS career).

OOP Class Impressions
------
Monday's class was good, because it helped be less complacent and more attentive to detail with facts. I didn't take much notice to the hierarchy of iterator demand and provided capabilities, until halfway in class I didn't register anything Downing was telling about. I ended up asking questions in order to get clarification on how these iterators worked for both containers and algorithms, thereby becoming more conscious to the fact of three things: 

1. I don't know everything.
2. I take many things for granted, and
3. Learning has a cost.

No matter what the cost (pride, openness, etc...) it is more fulfilling to learn in the face of judgement, than suffer in peace and confusion.

Anyways, on Wednesday, I found the JPL talk to be very informative and enjoyable. I really love the aspect of being able to hear from full-time employees what they do in their lives. Not only because I get to hear how they work pre-code, but also how they interact with others post-code. Storyboarding was a very interesting way of finding ideas to work on, and I tried to implement 'storyboarding' during the hackathon, but it didn't fare well, and we ended up going with the traditional "speak-or-no-chances-stay-silent-forever" method of brainstorming.

Unfortunately, I missed out on Friday's lecture because of the hackathon, so I can't say much on it.

What will you do next week?
------
I plan to finish my Threads project, a dream that I can only hope become a reality. I also need to catch up on sleep, all the readings and school work that I would've gotten done this weekend. And finally I need to start studying for 439 and OOP.

Additionally, I plan to consider whether I should go to TAMUHack or not the following weekend, since I don't particularly want to get another sleep-deprived weekend in my records, but I do want to learn. *sigh, as I said, learning has a cost.

Tip of the Week
------
If you ever plan to do any game development on Android, IOS, Web, VR, etc... I highly recommend using [Unity](https://unity3d.com/). You'll have to learn C# and there's a learning curve with new software, but Unity already has a lot of provided features that you don't need to implement from scratch like other software, and it's a great tool to use if you want to go into the game industry. Sure, if you want to struggle with the undocumented AndEngine or learn another Open-source Java/C++/etc... game engine, go right ahead. You'll learn a lot, but be warned, you may spend hours doing something that only takes a few clicks and lines on Unity!
