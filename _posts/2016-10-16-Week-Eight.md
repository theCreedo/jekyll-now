---
layout: post 
title: Week Eight - Eat, Work, Blog, Sleep
---

What did you do this past week?
------
I got a job.

One of my friends, Sonam, told her friend Meghana, a UT CS blogger, that I wrote a blog. Apparently the department of CS was looking for another blogger, and she suggested that I apply for the position. Now I'm an official blogger for the UT CS department! I never knew, but this blog for Downing's class really helped me process and explain my thoughts of the week, improve my writing abilities (hopefully), and eventually led me to writing for the UT CS department. If you're interested, posts will be updated every Tuesday (first post this Tuesday!) covering topics from hackathons, recruiting season, to my own personal CS life. [Eric's UTCS Blog](http://www.cs.utexas.edu/blog).

On another note, my team for Operating Systems spent 3 days trying to figure out one of the stupidest technical bugs ever. Try to catch it.

	// C code - Declaring cmd_line arguments and file names 
	char* cmd_line, file;

	// some code...

	file = *(char** ) get_file(pseudo-arguments);
	open(file); // error

For our Operating system, we were declaring several char* variables, and later we tried to save a char* into 'file', and call open() to open the file. Unfortunately, we were getting a page fault, causing all our tests to fail.

At first, we tried to check the beginning and ending address of the char* file, because we could've been accessing kernel addresses (which would cause major errors), but we weren't able to even call strlen(file) because the beginning address of the file was already considered kernel address.

	char* end_file = file + strlen(file); // error in strcmp for strlen().
	vaddress(file); // checks if file address is valid
	vaddress(end_file); // checks if end_file address is valid

After that, we tried to allocate memory in order to solve the problem, because it's possible that the memory being accessed currently was not user address. This actually solved the problem, but the TAs said that we shouldn't be allocating any memory, because that was a sketchy move to do

	
	char* cmd_line;
	// Putting on separate line in order to allocate 4 bytes of memory for 32 bit system pointer.
	char* file = malloc(4);

In the end, it turns out that depending on how you declare char* variables in a single line, they won't equate to putting them on separate lines. Apparently we were declaring a char* variable and char variable rather than two char* variables. So rather than solving the problem by allocating memory, by declaring the variables on separate lines, we ended up getting two char* variables rather than an obscure char variable.

	// incorrect way
	char* cmd_line, file; // cmd_line will be a char*. file will be a char.
	// correct way
	char *cmd_line, *file; // both cmd_line and file will be char*.

So end lesson: don't try to make code more compact/optimized by putting them onto one line unless you know what you're doing.

At least for Object Oriented Programming, the Allocator project is going very smoothly for Gilbert and me. The project does not seem too hard, and after debugging certain set up problems and designing the 4 required methods/constructors, we have already arrived at our unit tests, spending only about 10-12 hours total. This was one of the smoothest projects I have ever experienced, and I am looking forward to finishing it either this Sunday or Monday when we meet up.

What’s in your way?
------
This week has been rough for me on many occasions.

Not understanding the C language syntax caused my OS team to become stuck on a bug for 3 days. Though we currently are passing tests, we need to start picking up our pace in order to finish the project by Friday, because I don't plan on using any slip days for the weekend.

Additionally, my sleep schedule has been whack these past few days, sleeping in the range of 3-5 AM because of problem sets, blog posts, and other individual studies.

Most of all, one of my friends from my church passed away this past week... so there was a lot of things going through my mind as the week ended. When people asked me how I was, I found it hard to respond with "I'm good" or "Just busy" when clearly things weren't fine. Through it all, I remember I spent a lot of time listening to Christian music and praying for the family members and friends who were affected by this tragic event. Though I did not know her personally, I still felt a mix of sadness, anger, confusion, frustration, and many other emotions. And knowing that the intensity of these emotions were nothing compared to what her family and friends were going through made me recognize that I didn't have a right to worry about the little things in my life... *sigh* Rest in peace Connie. You will be missed.

OOP Class Impressions
------
Downing may seem intimidating in class mainly because he asks people questions directly, and instantly rebukes you for anything you do wrong, but with the right mindset, his teaching style is not as terrifying as everyone makes of it. If you approach his teaching style with a desire to learn, then it makes sense how he teaches, and you can learn a lot from him. I really enjoy how at the end of class, I can go up and ask all project and lecture questions, getting a better understanding of how C++ works.

What will you do next week?
------
I plan to finish the Allocator and OS project tests in order to be done with projects for the week.

Furthermore, I plan to go to some HackTX info sessions and do some idea planning with my team in preparation for HackTX this coming weekend.

Finally, I plan to try and get some rest, because I don't think I can function working on my projects/individual work without more than 6 hours of sleep.

Tip of the Week
------
[Boomerang](https://chrome.google.com/webstore/detail/boomerang-for-gmail/mdanidgdpmkimeiiojknlnekblgmpdll?hl=en) - Allows you to schedule messages to be sent or returned at a later date.

Just like scheduling your text messages, you can schedule any emails you have with friends, families, or companies in order to have the facade that you don't stay up till 4 AM in the morning or always wake up at 8 AM in order to do emails.
