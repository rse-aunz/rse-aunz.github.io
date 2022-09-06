---
layout: post
title:  "RSE Stories: An Interview with Johanna Bayer"
from:   2022-09-01 10:00:00
tags: ["RSE", "RSEStories", "ARDC", "2022"]
published: true                     
---

Posted by Paula Martinez on 6 September 2022

This post was originally published as a news item on the [Australian Research Data Commons website (31 August, 2022)](https://ardc.edu.au/news/shaping-research-software-an-interview-with-johanna-bayer/).

![Johanna Bayer - Research Software Engineer]("/assets/2022-08-24_JBayer.jpg")

Johanna Bayer, PhD Candidate at the University of Melbourne and a research software engineer.

As part of our [Research Software Agenda for Australia](https://ardc.edu.au/collaborations/strategic-activities/a-research-software-agenda-for-australia/), the ARDC is working with the research community to shape better research software in order to recognise it as a first-class output of research.

This interview is the fourth one in a series about research software engineers. Each month we will talk to a leading research software engineer about their experiences and best-practice tips in creating, sustaining and improving software for research.

Continuing the series, we talked to [Johanna Bayer](https://findanexpert.unimelb.edu.au/profile/830223-johanna-bayer) from the University of Melbourne.

What do you do as a research software engineer?
-----------------------------------------------

I am a final year PhD candidate at the University of Melbourne. My PhD focuses broadly on projects that improve the reproducibility of research on large neuroimaging datasets.

My first project uses machine learning methods to find biomarkers for mental health conditions, such as depression. I’ve created a method to use normative modelling, which allows us to identify individuals that deviate from the normative trajectory of brain growth. New normative modelling algorithms represent a novel way to parse and describe variant components and allow for individualised predictions.

Another project of my PhD focuses on site or batch effects that emerge when large neuroimaging data sets are created from pooling data sets across studies. I have written a review on methods to correct for those site effects, explaining the underlying mathematical foundation, and have published the relevant [software on normative modelling](https://github.com/likeajumprope/Bayesian_normative_models).

In my day to day work, my preferred programming languages are Python, Matlab and R, probably in that order. Python, also links in with everything that I do for fun, like web scraping, and [Kaggle](https://www.kaggle.com/) stuff. I have also used stan, but that’s more for modelling. For my computer science degree I used Java, C++, Pascal, and then Javascript, HTML and CSS.

Tell us about a project you enjoyed working on
----------------------------------------------

One of my favourite projects was being a Subject Matter Expert on Open Software for the [NASA Transform to Open Science (TOPS) program](https://science.nasa.gov/open-science/transform-to-open-science).

NASA declared the year of 2023 as the year of Open Science and launched a sprint to create a curriculum for a course that will be hosted on the platform [edX](https://www.edx.org/). I joined a group of open science experts from around the globe to create the chapter about Open Software in a sprint of 5 days! The course has 6 chapters on subjects like Licensing/Ownership, Code Management/Quality, Version Control, and Contributing. It was a super fun experience overall, and I particularly liked the project because it showed what can be done in a short amount of time when everyone is committed.

How does your work as an RSE advance research?
----------------------------------------------

I hope that my work as RSE makes a small contribution to overcome the reproducibility crisis in clinical neuroimaging. The reasons for unreproducible results are manifold, but certainly lie in small sample sizes and untransparent methods. My research focuses on individualised predictions, and the effective use of large, pooled datasets, which are publicly available.

In addition, I am trying to disseminate knowledge on how to do open research: I have been selected as [ReproNim INCF Fellow](https://www.repronim.org/fellowship.html). This is a full year Train-the-Trainer fellowship program, jointly sponsored by the International Neuroinformatics Coordinating Facility ([INCF](https://youtu.be/teFJ_W6nVUY)). In this program fellows become trainers in FAIR data, computational basics, reproducible workflows and statistical tools. As part of that, I am creating a course on open science, similar to Transform to Open Science ([TOPS](https://science.nasa.gov/open-science/transform-to-open-science)) but on a smaller scale, for our institute.

When I started out as a PhD student, I remember how lost I felt especially with the organisational part of writing software (folder structure, paths, version control, test coverage, etc.). My aim is thus to share as much of my journey as possible, to help others gain this knowledge early on.

Have you collaborated to extend existing software?
--------------------------------------------------

Collaborating on existing software is quite educational. Let’s face it, any kind of public software is probably more standardised, tested and documented than everything that you will write for yourself. So collaborating forces you to adhere to those standards, write tests, etc. And it can teach you quite a bit about how to write good code on the way.

I have contributed to Open Source Projects on various occasions. The most recent one is the [INCF Mathworks Toolbox Summer Project](https://www.incf.org/blog/summer-project-collaboration-between-incf-and-mathworks), where I contributed to the [Physio toolbox](https://www.tnu.ethz.ch/en/software/tapas/documentations/physio-toolbox) for physiological noise correction during fMRI.

What best practices for quality software do you implement in your work?
-----------------------------------------------------------------------

I have a set of standards that I have collected over the time that I find useful and that I try to adhere to:

1.  Write tests (unit and integration).
2.  Fail hard, early. Your tests should be written in a way that errors cannot be dragged through the running of a script or a pipeline undetected (and cause a chain of dependent errors down the way)
3.  Have at least 2 branches in a project on git: one dev(elopement) branch and one main branch. New stuff NEVER goes into the main.
4.  One function, one functionality.
5.  Good naming of your variables
6.  Write documentation
7.  NEVER save the output of a script (this forces you to make your work flows 100% reproducible).
8.  Try to get someone to review your code. Already the thought that someone will have a look at it will make you write better code in the first place.
9.  Refactor your code if it’s bad or error prone. Even if that means a major re-design of your code structure, you will 100% save more time if you set it up clean once than if you drag messy code through your project life.
10.  Try to write generic code - so no hard coding of variables, paths etc. Again one of the habits that will take a bit of time at the beginning, but save a lot of time in the end

Which research software communities do you recommend?
-----------------------------------------------------

[**The OHBM Open Science Group (OSSIG)**](https://ossig.netlify.app/)  
The OSSIG is a global special interest group of the [Organisation for Human Brain Mapping](https://www.humanbrainmapping.org/i4a/pages/index.cfm?pageid=1), focusing on Open Science. We organise a [hackathon](https://ohbm.github.io/hackathon2022/) and the [Open Science Room](https://ohbm.github.io/osr2022/). We are all volunteers, but the motivation and drive of this group has always been fantastic. You can also follow us on twitter [@OhbmOpen](http://twitter.com/OHBMOPEN).

[**Brainhack.org**](https://brainhack.org/)  
Even more decentralised than the OSSIG, brainhack.org organises hackathons related to brain data around the year and around the world. During a Brainhack global event several hubs around the world hold their own local hackathon around brainy stuff. Read more about the [philosophy of brainhack](https://pubmed.ncbi.nlm.nih.gov/33932337/). Also, keep your eyes peeled for the Australia Asia Hackathon that we are going to host this year, details coming soon!

[**The Turing Way**](https://the-turing-way.netlify.app/welcome)  
Lastly, I want to highlight a non neuro related community: The Turing Way Project is an open source, community driven handbook to reproducible, ethical and collaborative data science. Contributing to the Turing Way Book does not require any coding background and is a great way for beginners to start with contributing to Open Source. The Turing Way holds weekly Community Calls via zoom and FireSide Chats (both of which are usually at rather inconvenient times for the Australian time zone), but you can join the slack to get you started and oriented. View [the Slack and all resources](https://hackmd.io/@turingway/demo-intro).

Keep in Touch
-------------

You can connect with Johanna via [Twitter](https://twitter.com/likeajumprope?lang=en), [LinkedIn](https://www.linkedin.com/in/johanna-bayer) and [Github](https://github.com/likeajumprope).

If you’d like to be part of the growing community of research software engineers in Australia, become a member of the [RSE Association of Australia and New Zealand (RSE-AUNZ)](https://rse-aunz.github.io/) (it’s free!). Remember that September is the month when RSEs come together, join us for the New Zealand [conference](https://www.rseconference.nz/) and the Asia Australia [unconference](https://rse-aunz.github.io/2022-Asia-Australia-unconference/).

In our previous RSE Story we talked with the [winners of the Venables Award](https://ardc.edu.au/news/shaping-research-software-interview-with-lydia-lucchesi-and-sam-nelson/), which was established by the Statistical Society of Australia in partnership with the ARDC. The winners will present their software in a public talk, on Thu Sep 8, 1-2pm, you can [register now](https://www.eventbrite.com.au/e/ssa-venables-award-winners-2022-seminar-tickets-407730612237).

Stay tuned for our next interview in the Shaping Research Software series, coming out in November.

**Learn more about the [ARDC’s Research Software Agenda for Australia](https://ardc.edu.au/collaborations/strategic-activities/a-research-software-agenda-for-australia/).**

_The ARDC is funded through the National Collaborative Research Infrastructure Strategy (NCRIS) to support national digital research infrastructure for Australian researchers._

Johanna Bayer was interviewed by Dr Paula Andrea Martinez, ARDC. Reviewed by Jo Savill (ARDC).
