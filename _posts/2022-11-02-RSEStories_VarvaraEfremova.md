---
layout: post
title:  "RSE Stories: An Interview with Varvara Efremova"
from:   2022-11-02 1:00:00
tags: ["RSE", "RSEStories", "ARDC", "2022"]
published: true                     
---

Posted by Paula Martinez on 2 November 2022

This post was originally published as a news item on the [Australian Research Data Commons website (31 October, 2022)](https://ardc.edu.au/article/shaping-research-software-an-interview-with-varvara-efremova/).

Shaping Research Software: An Interview With Varvara Efremova
=============================================================

Varvara Efremova shares her best practices for research software engineering.

![Varvara Efremova, research software engineer, photo with abstract data background](https://ardc.edu.au/wp-content/uploads/2022/10/Hero-Block-FEATURE-IMAGE-583--580x345.jpg)

As part of our [Research Software Agenda for Australia](https://ardc.edu.au/collaborations/strategic-activities/a-research-software-agenda-for-australia/), the ARDC is working with the research community to shape better research software in order to recognise it as a first-class output of research. 

This interview is the sixth in a series about research software engineers in Australia. Each month we will talk to a leading research software engineer about their experiences and best-practice tips in creating, sustaining and improving software for research. 

Continuing the series, we talked to [Varvara Efremova](https://www.linkedin.com/in/varvaraefremova), a research software engineer at UNSW. Varvara is developing the research software [opendata.fit](http://opendata.fit/) as part of the ARDC-coinvestment project [Australian Characterisation Commons at Scale (ACCS)](https://ardc.edu.au/project/australian-characterisation-commons-at-scale-accs). Varvara also recently joined the Australian National University as Research Software Engineer for [ACCESS-NRI](https://www.linkedin.com/posts/access-nri_researchsoftwareengineers-ncrisimpact-ncrisimpact-activity-6986486952749412352-G8Y4).

**What do you do as a research software engineer?**
---------------------------------------------------

My research software engineering (RSE) role initially started out as a summer job as a research assistant in a supramolecular chemistry research group tasked with turning a Matlab script into a web application. Fortunately, the web app was a success and it became a more or less continuing role! Today our group has expanded to 3 RSEs working on the successor to the initial web application we developed. 

I now work as part of a small team of developers, building a research software web platform called [opendata.fit](http://opendata.fit/). I do a bit of everything and I really enjoy the variety – backend and frontend development, infrastructure management, graphical and user interface design, as well as liaising with external researchers to integrate their analysis scripts into our platform.

**Tell us about a project you enjoyed working on**
--------------------------------------------------

![A screenshot of the opendata.fit platform. with graphs and a dashboard](https://ardc.edu.au/wp-content/uploads/2022/10/opendatafit_screenshot-1024x640.png)
A screenshot of the opendata.fit platform.

My focus for the last few years has been on building the [opendata.fit](https://opendata.fit/) platform, which aims to be an interdisciplinary [FAIR data](https://ardc.edu.au/resource/fair-data/) analysis and publication platform for the web. The idea for the project grew organically after the success of our predecessor webapp called [Bindfit](http://app.supramolecular.org/bindfit/), which is an online fitting tool we built to simplify the process of calculating binding constants from titration experiment data – a process used in fields like drug research and discovery among many others.

For the last 5 years, I’ve worked together with another RSE to go from initial architecture sketches all the way to deployment (almost!). It’s hard to pick a favourite part of the work as I truly enjoy it all! 

I love being able to work across all domains of software development, which is something you would rarely be able to do in a more traditional role. Through this role I went from being a weekend coding enthusiast to becoming an experienced full stack developer, deploying complex infrastructure setups on AWS, and even playing with compiling things like Numpy for WebAssembly. 

My favourite part of this work is definitely the diversity, as well as getting to work with a huge variety of researchers and provide tools for them that make a difference in their research.

**How does your work as an research software engineer advance research?**
-------------------------------------------------------------------------

The 2 biggest focuses of our platform are: 

1.  Providing a way for researchers to share, execute and reuse analysis scripts
2.  Building reproducibility into the analysis process. 

Since my first undergraduate research position, it has always struck me how much time researchers spend “reinventing the wheel” because things like analysis scripts are either not freely available, not easily accessible, or too specialised to be reused. I’m hoping [opendata.fit](http://opendata.fit/) can go some way towards addressing this problem by providing a useful platform for scientists to publish and execute their analysis scripts on, that builds reproducibility into the process.

**What best practices for quality software do you implement in your work?**
---------------------------------------------------------------------------

*   Design with modularity in mind, including well-defined interfaces between components.
    *   Through our work on the [Bindfit](http://app.supramolecular.org/bindfit/) app and then [opendata.fit](http://opendata.fit/) backends, we went from a [Django](https://www.djangoproject.com/)\-based monolithic app architecture with everything contained in a single codebase, to a [Flask](https://flask.palletsprojects.com/)\-based microservice implementation split across many small [containers](https://ardc.edu.au/resource/how-software-containers-help-researchers/). The end result was a codebase comparable in size to [Bindfit](http://app.supramolecular.org/bindfit/), with much greater functionality, and with useful components that can be easily reused independently of each other if desired.

*   Maintain consistent, readable code with explanatory comments.
    *   This is extremely important for encouraging collaboration and speeding up the development process where multiple developers are working on the same codebase.

*   Enforce style guides with pre-commit pipelines
    *   I am also a huge advocate for using [linters](https://www.testim.io/blog/what-is-a-linter-heres-a-definition-and-quick-start-guide/) and [auto formatters](https://www.kevinpeters.net/auto-formatters-for-python) in combination with pre-commit pipelines to enforce style guides, particularly for languages like Python and Javascript that have a lot of flexibility built into them.

**Which research software communities do you recommend?** 
----------------------------------------------------------

The [RSE-AUNZ](https://rse-aunz.github.io/) mailing list is fantastic and a great starting place to find out about other more field-specific RSE communities.

I work with Ember.js and have found the [Ember.js Discord](https://discord.com/invite/emberjs) server to be one of the most helpful and pleasant open source communities I’ve come across, so that’s something I’d highly recommend for any frontend developers.

**Keep in touch**
-----------------

You can connect with Varvara via [Twitter](https://twitter.com/vrvrfrmv), [LinkedIn](https://www.linkedin.com/in/varvaraefremova) and [Github](https://github.com/echus).

If you’d like to be part of the growing community of research software engineers in Australia, become a member of the [RSE Association of Australia and New Zealand (RSE-AUNZ)](https://rse-aunz.org) (it’s free!). 

In our last [RSE Story](https://ardc.edu.au/article/shaping-research-software-an-interview-with-anthony-truskinger/) we talked with Anthony Truskinger from Open Ecoacoustics. Stay tuned for our next interview in the Shaping Research Software series, coming out in December. 

We will soon announce the winners of the [ARDC Award for New Developers of Open Source Software in Ecology 2022](https://www.ecolsoc.org.au/awards/ardc-award-for-new-developers-of-open-source-software-in-ecology/) and the winners of [Australian Bioinformatics And Computational Biology Society Awards](https://www.abacbs.org/awards) for research software, sponsored by the ARDC.

**Learn more about the ARDC’s** [**Research Software Agenda for Australia**](https://ardc.edu.au/collaborations/strategic-activities/a-research-software-agenda-for-australia/)

_The ARDC is funded through the National Collaborative Research Infrastructure Strategy (NCRIS) to support national digital research infrastructure for Australian researchers._

Varvara Efremova was interviewed by Dr Paula Andrea Martinez, ARDC. Reviewed by Jo Savill, Dr Tom Honeyman, ARDC.

### Author

Dr Paula Andrea Martinez, ARDC

### Reviewed by

Jo Savill, Dr Tom Honeyman, ARDC

Follow RSE-AUNZ
---------------

*   [Twitter](https://twitter.com/RSE-AUNZ)
*   [Linkedin](https://www.linkedin.com/groups/13836034/)
