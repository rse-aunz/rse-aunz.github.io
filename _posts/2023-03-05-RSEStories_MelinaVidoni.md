---
layout: post
title:  "RSE Stories: An Interview With Melina Vidoni"
from:   2023-03-03 0:00:00
tags: ["RSE", "RSEStories", "ARDC", "2023"]
published: true                     
---

Posted by Paula Martinez, 3 March 2022

This post was originally published as a news item on the [Australian Research Data Commons website (3 March, 2023)](https://ardc.edu.au/article/shaping-research-software-an-interview-with-melina-vidoni/).

Shaping Research Software: An Interview With Melina Vidoni
==========================================================

We interview Dr Melina Vidoni about her interests that intersect technical debt and the development of scientific software.

**Published:** 28 February 2023

![Dr Melina Vidoni photo with green data visualisation in the background](https://ardc.edu.au/wp-content/uploads/2023/02/melina-vidoni-feature-image-583-x-345-580x345.png)

As part of our [Research Software Agenda for Australia](https://ardc.edu.au/collaborations/strategic-activities/a-research-software-agenda-for-australia/), the ARDC is working with the research community to shape better research software in order to recognise it as a first-class output of research. This interview is the [ninth in a series](https://ardc.edu.au/news-and-events/news/?_keyword=%22Shaping%20Research%20Software%22&_categories=research-software) about research software engineers in Australia. Each month we talk to a leading research software engineer about their experiences and best-practice tips in creating, sustaining and improving software for research. 

Continuing the series, we spoke with [Dr Melina Vidoni](https://researchers.anu.edu.au/researchers/vidoni-m), a Lecturer at the Australian National University. Dr Vidoni’s main research interests intersect technical debt and the development of scientific software, explored through real-world analyses of open source software in combination with human-centred studies. She is currently a member of the Editorial Board of “[Information and Software Technology](https://www.sciencedirect.com/journal/information-and-software-technology)”, was a recipient of the [ACM Distinguished Reviewer Award](https://melvidoni.rbind.io/publication/msr22-vidoni-distinguishedreviewer.pdf) for her peer-reviewing efforts at the International Conference of Mining Software Repositories 2022 (MSR’22), and has been on the Program Committee for [a number of top-ranking conferences](https://melvidoni.rbind.io/service/) in the broader area of software engineering, such as FSE, ASE, MSR, ICPC, and EASE.

What is your interest in researching software engineering practices?
--------------------------------------------------------------------

I completed an engineering degree in Information Systems, and was then offered a scholarship to complete a PhD. Both of these education paths got me very deep into the development of cutting-edge software, but always with a scientific/domain-specific angle. In particular, the university where I graduated (Universidad Tecnológica Nacional) had plenty of interdisciplinary research intersecting software engineering and operational research. When I began my postdoc, I became more interested in data science and the large-scale mining of repositories, which led me to uncover the many issues that scientific software developers encounter. Then, when I had the opportunity to start building my own team and lab, I focused on the practices and human-centred aspects of software development. After all, everything that is coded depends on a human’s decision, choice, and/or expertise.

What can you share about technical debt in scientific and data science software?
--------------------------------------------------------------------------------

Technical debt is the consequence of software developers choosing a low-quality solution due to time constraints (e.g., wanting to release faster/earlier). The term was coined by Ward Cunningham and later expanded by many authors of the Agile Manifesto. It was originally studied in mostly object-oriented, traditional statically-typed languages such as Java or C, and has recently expanded to scientific software.

Through my investigations, I have uncovered that technical debt exists in scientific software, although it has its nuances:

*   RSEs ‘admit’ incurring in technical debt knowingly or unknowingly just like traditional developers do, and in the same places, such as code comments, commit messages, GitHub issues.
*   There are scientific-specific Debts such as _Algorithm Debt_. One of my PhD students at ANU, [Iko-ojo Simon](https://twitter.com/Ikoojo_S), is investigating this type of debt. Algorithm Debt are low-quality programming choices related almost exclusively to the logic of a scientific algorithm–which could have severe consequences for the investigations depending on such faulty software, by directly threatening the validity, reproducibility, and robustness of such research.
*   _Documentation Debt_, also severely affects scientific software, e.g lacking or outdated documentation.

Most of my papers are freely available on [my personal website](https://melvidoni.rbind.io/).

![Dominic Yang  stands with his research presentation at the School of Computing at the ANU.](https://ardc.edu.au/wp-content/uploads/2023/02/dominic-yang-copy-2-1024x764.jpg)

_Dominic Yang, an undergraduate research student who studied with Dr Melina Vidoni in 2022, stands with his research presentation at the School of Computing at the ANU._

How do software engineers differ from research software engineers, in your opinion?
-----------------------------------------------------------------------------------

This is actually quite a complicated question. On the one hand, contrary to popular belief, they are the same: software developers. The difference is in which _domain_ they work. One could argue that RSE requires more specific or domain knowledge, but the same argument applies to ‘traditional’ developers. For example, have you ever seen the amount of maths involved in video game development? Think of classical games like Angry Bird (purely maths) or Portal (plenty of physics involved).

On the other hand, I would argue that what changes is their self-perception. RSE tend to repeatedly state that “they are not software developers”, and after researching quite a bit about them (and also reading other researchers’ findings), the arguments that often come up are: 

1) RSE do not generally have a computer science-related degree

2) they do not develop general-purpose applications (think of note-taking apps, e-commerce platforms, games, and so on). 

Through the many surveys I’ve conducted, it became clear that this self-perception biases what RSEs are do, and how they perceive their responsibility over the long-term quality of the code they develop. All in all, this self-conception has several repercussions, and one is particularly difficult: RSEs generally self-select out of research studies claiming that, ironically, “they are not software developers”. This is problematic because how can we advance the knowledge of RSE’s challenges, pain points, reasons to act, and needs, if they select-out of studies?

Tell us about your team
-----------------------

[Sewire](https://twitter.com/SEWIRE3) is an international list of [Women doing Software Engineering research](https://www.margaretstorey.com/sewire/), you can also be listed and join the community. Through there, I met two excellent collaborators from Canada, with whom I have published and co-supervised students. [Dr Fatemeh Fard](https://cmps.ok.ubc.ca/about/contact/fatemeh-hendijani-fard/) (University of British Columbia), and [Dr Zadia Codabux](https://www.cs.usask.ca/people/faculty%20profiles/Zadia-Codabux.php) (University of Saskatchewan). I also collaborate with [Dr Nicolás Díaz Ferreyra](https://www.ndiaz-ferreyra.com/), from the University of Technology Hamburg in Germany, at the intersection of privacy and software engineering. 

In terms of students, at ANU I generally have 4-6 undergraduates conducting research under my supervision each semester. Their work is generally a combination of software-related data mining (from code, to comments, documentation, etc.) and data-science/machine learning. Additionally, this year I’ll be hosting two students from abroad thanks to the Future Research Talent program (for students of [India](https://science.anu.edu.au/study/scholarships/future-research-talent-awards-india) and [Indonesia](https://science.anu.edu.au/study/scholarships/future-research-talent-awards-indonesia)) to work on developer-centric documentation of scientific software.

![Manas Prasad](https://ardc.edu.au/wp-content/uploads/2023/02/manas1-2-1024x528.jpg)

_Manas Prasad, who completed an Honours under Dr Vidoni’s supervision, graduating with 1st class honors in 2022. He was part of Co-Lab, a partnership between the Australian Signals Directorate (ASD) and the Australian National University (ANU)._

Keep In Touch
-------------

You can connect with Melina via [Twitter](https://twitter.com/melvidoni).

If you’d like to be part of the growing community of research software engineers in Australia, become a member of the [RSE Association of Australia and New Zealand (RSE-AUNZ)](https://rse-aunz.org) (it’s free!). 

Research Software Awards Open for Submissions
---------------------------------------------

For Ecology:

The Ecological Society of Australia has an ARDC-sponsored award for New Developers of Open Source Software in Ecology [Apply now, it closes on 31 March 2023 >](https://www.ecolsoc.org.au/awards/ardc-award-for-new-developers-of-open-source-software-in-ecology/)

For Statistics:

The 2023 Statistical Society of Australia (SSA) Bill Venables Award for new developers of open source software for data analytics, sponsored by the ARDC is now open [Apply now, closing on 22 April 2023 >](https://statsocaus.github.io/venables-award/)

Eureka Prize for Excellence in Research Software:

Entries to the 2023 Australian Research Data Commons Eureka Prize for Excellence in Research Software are now open [More information](https://australian.museum/blog/science/excellence-in-research-software/)[, closing on 14 April 2023](https://australian.museum/get-involved/eureka-prizes/enter/research-software/) [>](https://australian.museum/blog/science/excellence-in-research-software/)

Stay tuned for our next interview in the Shaping Research Software series, coming out in April 2023. 

**Learn more about the ARDC’s** [**Research Software Agenda for Australia**](https://ardc.edu.au/collaborations/strategic-activities/a-research-software-agenda-for-australia/).

_The ARDC is funded through the National Collaborative Research Infrastructure Strategy (NCRIS) to support national digital research infrastructure for Australian researchers._

### Author

Dr Paula Andrea Martinez, ARDC.

### Reviewed by

Jo Savill, Dr Tom Honeyman, ARDC.

Follow RSE-AUNZ
---------------

*   [Twitter](https://twitter.com/RSE-AUNZ)
*   [Linkedin](https://www.linkedin.com/groups/13836034/)
