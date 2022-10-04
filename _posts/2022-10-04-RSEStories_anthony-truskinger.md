---
layout: post
title:  "RSE Stories: An Interview with Anthony Truskinger"
from:   2022-10-04 1:00:00
tags: ["RSE", "RSEStories", "ARDC", "2022"]
published: true                     
---

Posted by Paula Martinez on 4 October 2022

This post was originally published as a news item on the [Australian Research Data Commons website (26 September, 2022)]([https://ardc.edu.au/article/shaping-research-software-an-interview-with-anthony-truskinger/).

Shaping Research Software: An Interview With Anthony Truskinger
===============================================================

Research software engineer Dr Anthony Truskinger discusses how he works to help ecologists study the environment's multitude of sounds.

As part of our [Research Software Agenda for Australia](https://ardc.edu.au/project/research-software-agenda-for-australia/), the ARDC is working with the research community to shape better research software in order to recognise it as a first-class output of research. 

This interview is the fifth one in a series about research software engineers. Each month we will talk to a leading research software engineer about their experiences and best-practice tips in creating, sustaining and improving software for research. 

Continuing the series, we talked to Dr Anthony Truskinger from [Open Ecoacoustics](https://openecoacoustics.org/) and the [Queensland University of Technology](https://www.qut.edu.au/about/our-people/academic-profiles/a.truskinger).

What do you do as a research software engineer?
-----------------------------------------------

A little of everything.

I have been a Research Software Engineer since 2009 (a label I’ve applied post hoc). Over time, my roles and responsibilities have changed a lot so it can be hard to pin down any one answer.

I was originally hired to translate research code (MATLAB) into production code. This meant translating the code into the language the rest of our platform used, and making changes such that the analysis worked on a wide variety of data sources. 

I completed my PhD in the years between, in the same research group. Pure research was not enjoyable for me, but I liked working in ecoacoustics. I decided to stay on in a technical role.

These days, I am a systems admin, a backend developer, a front end developer, a mentor to others in my group, and I occasionally still contribute to research publications. 

One of the biggest reasons I was excited by the RSE concept is because I didn’t really fit into the normal University classifications. I wasn’t an academic. I wasn’t an eResearch specialist from a central university resource who moved from project to project. I was permanently embedded into a research group as a technical person who also sometimes produced academic publications!

How does your work as a research software engineer advance research?
--------------------------------------------------------------------

Our platform is an eResearch initiative; it exists to improve other researcher’s ability to conduct science. Our argument is that your average ecologist shouldn’t need to know about the intricacies of storing petabytes of audio data to do their job.  This was a novel concept in 2009! In the years since, I am glad to see that digital literacy of researchers has greatly improved. Resources like Software Carpentry and growth of the RSE movement have changed the landscape so much that it means we can provide more powerful solutions to researchers who can code.

![A spectrogram](https://ardc.edu.au/wp-content/uploads/2022/09/ecoacoustics-data-image-1024x224.png)

_A false colour spectrogram of a day of environmental audio data. Different indices are assigned to colour channels to create a composite image that exposes more detail than usual_.

Tell us about a project you have enjoyed working on.
----------------------------------------------------

I’ve worked in the same research group the whole time, on one big project! It has been incredibly exciting growing a platform up to handle so much data. We originally started out with a Silverlight (like Flash) web page that could stream 2-minute blocks of audio. We had about 100GB of audio data. Since then we now have a standards-based HTML 5 site that can stream audio indefinitely from our collection of 180TB (80+ years) of audio data. We used to only host data for our own projects, now we host it for any ecologist that wants a place to store their data. Most recently we built and created a batch upload interface so anyone can upload terabytes of audio data at a time.

Have you collaborated on extending existing software rather than recreating it? 
--------------------------------------------------------------------------------

Over the years we’ve contributed to a few open-source projects but those are usually technical contributions to JavaScript/Ruby libraries used in the creation of our website.

How we fix that depends. The first step is to see if an issue exists for the problem. If it doesn’t, we file one against the project’s issue tracker, so the maintainer knows there is a problem and can advise how to proceed. Sometimes we just straight up issue a pull request against a project — but do this with care; the maintainers will often have good advice for how to contribute to their project, communication is key.

What is the best feedback from users you have received to improve your software?
--------------------------------------------------------------------------------

The best feedback we’ve gotten has been indirect. Once your project gets past a certain size, and all of your users have been exposed (and biased) to your software, it becomes quite hard to generate useful feedback. 

What’s been more effective for us is running usability interviews with our users. We ask users who seem to be having trouble to do their normal workflow with us watching. When they get stuck, we ask them what they wanted to happen and then we go off and make sure it does. We report back with our enhancements/bug fixes a few weeks later and repeat the process again, until, for those users and their use cases, everything runs smoothly. This process has been enormously helpful in focusing our efforts into helping real users.

What best practices for quality software do you implement in your work? 
------------------------------------------------------------------------

*   Use version control. Your code will never be static, keep a history, write good commit messages. You will be the stranger who will be helped by this 6 months from now.
*   Separate your data from your code. There are a lot of ways to deal with data but the most important thing to understand is that version control does not store data well. Try [git lfs](https://git-lfs.github.com/) if you want that tightly integrated feeling.
*   Write tests. Your code is broken unless it is tested. You don’t have to go all in, you can add tests for small parts of your code base as you go. Anything is better than nothing.
*   Be a polyglot. The more you know the better you will be. There are commonalities in languages, operating systems, and platforms. Learning those commonalities will make your skills transferable and will allow you to pick up new tools with ease.
*   Be an advocate. I think most of the above advice is redundant to many readers. The real difference is you advocating these practices within your communities or research groups. 

Which research software communities do you recommend? 
------------------------------------------------------

The [RSE Association of Australia and New Zealand (RSE-AUNZ)](https://rse-aunz.github.io/) is a growing community but I often find it is too general to be useful to me. I recommend finding or creating communities with your own research fields and extending them with discussions about research software engineering.

For Ecoacoustics communities in Australia, check out the [Australasian Chapter of Ecoacoustics group on Facebook](https://www.facebook.com/groups/ausecoacoustics). For bioacoustics (for which many of our problems are similar) the new [Bioacoustics Stack Exchange](https://bioacoustics.stackexchange.com/) is a great resource.

Keep in Touch
-------------

You can connect with Anthony via [Twitter](https://twitter.com/atruskie), [LinkedIn](https://www.linkedin.com/in/anthonytruskinger), and [Github](https://github.com/atruskie).

Open Ecoacoustics is an ARDC-co-investment project. Read about [the project](https://ardc.edu.au/project/open-ecoacoustics/).

If you’d like to be part of the growing community of research software engineers in Australia, become a member of the [RSE Association of Australia and New Zealand (RSE-AUNZ)](https://rse-aunz.github.io/) (it’s free!).

Stay tuned for our next interview in the Shaping Research Software series, coming out in November.

**Learn more about the ARDC’s [Research Software Agenda for Australia](https://ardc.edu.au/project/research-software-agenda-for-australia/).**

_The ARDC is funded through the National Collaborative Research Infrastructure Strategy (NCRIS) to support national digital research infrastructure for Australian researchers._

### Author

Dr Paula Andrea Martinez, ARDC

### Reviewed by

Jo Savill, ARDC

Follow RSE-AUNZ
---------------

*   [Twitter](https://twitter.com/RSE-AUNZ)
*   [Linkedin](https://www.linkedin.com/groups/13836034/)
