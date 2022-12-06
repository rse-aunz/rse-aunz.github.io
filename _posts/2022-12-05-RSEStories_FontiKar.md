---
layout: post
title:  "RSE Stories: An Interview with Fonti Kar"
from:   2022-12-05 1:00:00
tags: ["RSE", "RSEStories", "ARDC", "2022"]
published: true                     
---

Posted by Paula Martinez on 6 December 2022

This post was originally published as a news item on the [Australian Research Data Commons website (28 November, 2022)](https://ardc.edu.au/article/shaping-research-software-an-interview-with-fonti-kar/).


Shaping Research Software: An Interview With Fonti Kar
======================================================

We spoke to Dr Fonti Kar, who won the Ecological Society of Australia's award for New Developers of Open Source Software in Ecology

**Published:** 28 November 2022

![Fonti Kar and AusTraits logo](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%20580%20345'%3E%3C/svg%3E)

![Fonti Kar and AusTraits logo](https://ardc.edu.au/wp-content/uploads/2022/11/interview-with-fonti-kar-feature-image-583-x-345-580x345.png)

As part of our [Research Software Agenda for Australia](https://ardc.edu.au/collaborations/strategic-activities/a-research-software-agenda-for-australia/), the ARDC is working with the research community to shape better research software in order to recognise it as a first-class output of research. 

This interview is the [seventh in a series](https://ardc.edu.au/news-and-events/news/?_keyword=%22Shaping%20Research%20Software%22&_categories=research-software) about research software engineers in Australia. Each month we will talk to a leading research software engineer about their experiences and best-practice tips in creating, sustaining and improving software for research. 

Continuing the series, we talked with the winner of the [Ecological Society of Australia](https://www.ecolsoc.org.au/) [Early-career Ecologist Award](https://www.ecolsoc.org.au/awards/early-career/) for [New Developers of Open Source Software in Ecology.](https://www.ecolsoc.org.au/awards/ardc-award-for-new-developers-of-open-source-software-in-ecology/) This award is sponsored by the ARDC in recognition of the valuable contribution made by software to ecological research. The winning team is the {[austraits}: R package](https://traitecoevo.github.io/austraits/) which allows users to access, explore and wrangle data from the AusTraits database in R. 

[AusTraits](https://austraits.org/) is a national data asset quantifying the traits of Australia’s flora, which comprises approximately 26,000 different plant species. It is a co-investment [project](https://ardc.edu.au/project/austraits/) of the ARDC through the [Australian Data Partnerships program](https://ardc.edu.au/program/australian-data-partnerships/), and the University of New South Wales, Western Sydney University and Royal Botanic Gardens, plus 15 others. The [{austraits}: R package](https://traitecoevo.github.io/austraits/) has been developed over the last 2 years and its code is [open source](https://github.com/traitecoevo/austraits/). One of the core maintainers is [Dr Fonti Kar](https://github.com/traitecoevo/austraits/graphs/contributors).

Meet [Dr Fonti Kar](https://fontikar.wordpress.com/), a Postdoctoral Research Associate at the [Evolution & Ecology Research Centre](https://www.unsw.edu.au/research/eerc) based at the University of New South Wales, Sydney. Fonti is also a teaching assistant of Biostatistics, a Data Analyst of the [Atlas of Living Australia (ALA)](https://www.ala.org.au/), a [Software Carpentry](https://carpentries.org/) Instructor, a co-founder of the [UNSWcodeRs](https://unsw-coders.netlify.app/) and engages in a variety of [science outreach activities](https://fontikar.wordpress.com/outreach/). 

![Rosie Hicks presents the Ecological Society of Australia Award for new developers of open source software in ecology to Dr Fonti Kar from AusTraits. ARDC and ESA banners in the background.](data:image/svg+xml,%3Csvg%20xmlns='http://www.w3.org/2000/svg'%20viewBox='0%200%201024%20648'%3E%3C/svg%3E)

![Rosie Hicks presents the Ecological Society of Australia Award for new developers of open source software in ecology to Dr Fonti Kar from AusTraits. ARDC and ESA banners in the background.](https://ardc.edu.au/wp-content/uploads/2022/12/ecocommons-launch_003_rosie-and-fonti-web-1024x648.jpg)

ARDC’s CEO Rosie Hicks presents the ARDC-sponsored Ecological Society of Australia Award for New Developers of Open Source Software in Ecology to Dr Fonti Kar from AusTraits. Credit: ARDC / Josh Brightman.

Fonti, tell us about your role as the main {austraits} R package developer.
---------------------------------------------------------------------------

The most exciting part of developing {austraits} is seeing people use the package. I enjoy hearing people’s experiences with the package as this ultimately leads to improvements to the software. It’s been a really fulfilling experience to work on a research tool that can facilitate the research of others and allow the community to better understand plant ecology at a broader scale.

As a biologist myself, it’s been an insightful process to think about how a typical user would want to interact with our package. This has guided many package development decisions from the tone of the documentation; to the functionality of the package; and even the naming of functions. It is important to me to help create a tool that can be used by many people from students to budding ecologists. 

Who do you work with day to day?
--------------------------------

Maintaining an R package like {austraits} is a constant work-in-progress! More often than not, solving one problem will lead me to make adjustments elsewhere. When I am not addressing bug reports flagged by myself and other users, I am writing tests or combing through the package to streamline processes. This sometimes involves improving documentation and the overall ‘look’ of the package.

Having said that, I think I have it quite easy compared to the rest of the [AusTraits team](https://austraits.org/team_subpage/). I work mostly with Dr Daniel Falster, a core contributor to the R package and one of the masterminds that was inspired to start compiling data for [AusTraits](https://austraits.org/team_subpage/), and Dr Elizabeth Wenk, the resident expert and custodian of the AusTraits database. Dr Falster offers coding support and big-picture feedback on my implementations, whereas Dr Wenk supports me with essential knowledge to help me develop code to navigate the AusTraits database. It takes a village to create a high-quality, relational database; maintaining this R package is one small part of it. 

What does winning the ESA Open Source Software in Ecology award mean to you and your team?
------------------------------------------------------------------------------------------

Open access to an extensive and unified plant trait database was not possible prior to the release of the AusTraits database. One considerable benefit of the {austraits} R package is the ability for users to seamlessly download specific versions of the AusTraits database so that the entire workflow from data processing, to analysis and visualisation can be fully integrated and reproducible with R code. I hope my contributions to the R package will facilitate curious scientists to ask more ambitious questions and deepen our understanding of Australian plant ecology. 

Receiving the award is a massive confidence boost! It reaffirms that I should continue following my interests in R programming and facilitating research as a software developer. It will allow me to upskill certain aspects of package development and provide me opportunities to connect with other R developers to share ideas and experiences.

Could you mention what best practices for quality software have you implemented in your work?
---------------------------------------------------------------------------------------------

I consider myself a novice R package developer. There is so much to learn and every R package requires very different needs. I’m very lucky to work with a code-savvy team and have access to open source resources such as [The R Packages book by Hadley Wickham and Jenny Bryan](https://r-pkgs.org/) and the [rOpenSci’s Packages Book](https://devguide.ropensci.org/). These reference texts have helped me create {austraits} and other packages to the best current practices in the R community.   
  
One thing I am proud of learning and implementing for {austraits} is [GitHub Actions](https://docs.github.com/en/actions). It ensures that an R package is stable and up-to-date as contributors make changes to the code. GitHub Actions has automated many aspects of my package development workflow such as testing and website deployment. At the moment, resources for implementing GitHub Actions are a little spread out, I’ve consolidated what I’ve learned in a [recent workshop](https://github.com/fontikar/DIY_Rpkg_GHA) to help aspiring R package developers get started. 

What communities or professional networks would you recommend? 
---------------------------------------------------------------

The R programming community is vast. I try to stay up-to-date with the latest R developments via Twitter. One account I really like that amplifies the voices of people from all walks of life is [@WeAreRLadies](https://twitter.com/WeAreRLadies).  
  
I have really enjoyed participating in [rOpenSci’s community activities](https://ropensci.org/community/). I’ve learned about many package development best practices from watching their community calls, including [tips on writing tests](https://ropensci.org/commcalls/2019-12-05/) and how to set up a R package to [welcome community contributions and engagement](https://ropensci.org/commcalls/apr2021-pkg-community/). If timing permits, I try to join in on rOpenSci’s social coworking hours. This is where I’ve connected with fellow R package developers who have shared valuable perspectives about their roles and projects. 

Empowering others
-----------------

It has been an intimidating and humbling experience entering the research software development space with no computer science or software engineering background. I came into my role with a PhD in evolutionary biology and an aptitude for R programming; I didn’t feel particularly qualified to help write research software. I second-guessed myself a lot and took coding blockages quite personally. My outlook shifted for the better when I approached my role with a ‘learning on the job’ and ‘work in progress’ mentality.  
  
There is a dismaying lack of diversity in the research community, and the research software development community is no exception. I found connecting with R programmers that have been historically or systematically excluded from this space has helped me build a sense of belonging. My experience has encouraged me to foster a welcoming space in the [UNSW R user group](https://unsw-coders.netlify.app/) I co-founded and in the workshops I run. I hope these efforts can empower others to see themselves in the research software development community.

Keep in touch
-------------

You can connect with Fonti via [Twitter,](https://twitter.com/fonti_kar) [LinkedIn](https://www.linkedin.com/in/fonti-kar/) and [GitHub.](https://github.com/fontikar)

If you’d like to be part of the growing community of research software engineers in Australia, become a member of the [RSE Association of Australia and New Zealand (RSE-AUNZ)](https://rse-aunz.org) (it’s free!). 

In our last [RSE Story, we talked with Varvara Efremova](https://ardc.edu.au/article/shaping-research-software-an-interview-with-varvara-efremova/) from [opendata.fit](http://opendata.fit/). Stay tuned for our next interview in the Shaping Research Software series, coming out in February 2023. 

Do you create or maintain research software for ecology? Applications for the ARDC-sponsored award for New Developers of Open Source Software in Ecology open on 1 February 2023! [Learn how to apply](https://www.ecolsoc.org.au/awards/ardc-award-for-new-developers-of-open-source-software-in-ecology/). 

**Learn more about the ARDC’s** [**Research Software Agenda for Australia**](https://ardc.edu.au/collaborations/strategic-activities/a-research-software-agenda-for-australia/)

_The ARDC is funded through the National Collaborative Research Infrastructure Strategy (NCRIS) to support national digital research infrastructure for Australian researchers._

### Author

Dr Paula Andrea Martinez, ARDC

### Reviewed by

Jo Savill and Dr Tom Honeyman, ARDC

Follow RSE-AUNZ
---------------

*   [Twitter](https://twitter.com/RSE-AUNZ)
*   [Linkedin](https://www.linkedin.com/groups/13836034/)

