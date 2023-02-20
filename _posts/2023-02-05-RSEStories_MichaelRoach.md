---
layout: post
title:  "RSE Stories: An Interview with Michael Roach"
from:   2023-02-05 1:00:00
tags: ["RSE", "RSEStories", "ARDC", "2023"]
published: true                     
---

Posted by Paula Martinez on 5 February 2023

This post was originally published as a news item on the [Australian Research Data Commons website (30 January, 2023)](https://ardc.edu.au/article/shaping-research-software-an-interview-with-michael-roach/).

Shaping Research Software: An Interview With Michael Roach
==========================================================

We interview Dr Michael Roach, the winner of the ARDC-sponsored ABACBS ‘Torsten Seemann’ award for an Outstanding Bioinformatics Software Developer.

**Published:** 30 January 2023

![Michael Roach is the winner Torsten Seemann Outstanding Software Developer award.](https://ardc.edu.au/wp-content/uploads/2023/01/interview-with-michael-roach-583-x-345-580x345.png)

As part of our [Research Software Agenda for Australia](https://ardc.edu.au/collaborations/strategic-activities/a-research-software-agenda-for-australia/), the ARDC is working with the research community to shape better research software in order to recognise it as a first-class output of research. This interview is the [eighth in a series](https://ardc.edu.au/news-and-events/news/?_keyword=%22Shaping%20Research%20Software%22&_categories=research-software) about research software engineers in Australia. Each month we talk to a leading research software engineer about their experiences and best-practice tips in creating, sustaining and improving software for research. 

Continuing the series, we spoke with the winner of [The Australian Bioinformatics and Computational Biology Society (ABACBS)](https://www.abacbs.org) who won the [‘Torsten Seemann’ award for an Outstanding Bioinformatics Software Developer](https://www.abacbs.org/awards). This award is sponsored by the ARDC in recognition of the value of their software to their community and with a view to promoting further efforts to develop and share bioinformatics methodologies broadly.

Meet [Dr Michael Roach](https://www.flinders.edu.au/people/michael.roach), a Research Fellow bioinformatician at Flinders University, [Flinders Accelerator for Microbiome Exploration (FAME)](https://fame.flinders.edu.au/about/) who develops and maintains the open-source and freely available bioinformatics tool [Hecatomb](https://fame.flinders.edu.au/software/2021/05/25/hecatomb).

How did you become a research software engineer (RSE)?
------------------------------------------------------

I had no formal training in software engineering and am self-taught. My delve into research software engineering was born out of necessity. During my PhD I had to perform some scripting but it wasn’t until my first post-doc at the Australian Wine Research Institute ([AWRI](https://www.awri.com.au/)) that I found myself doing a lot more coding. My main project was the [Chardonnay genome project](https://bioplatforms.com/projects/chardonnay-sequencing/). We needed to create a novel pipeline to identify markers for different clones of Chardonnay using our new assembly. My time at the AWRI made all the difference in developing my skills and experience in software development as I was given a lot of freedom to pursue these interests. Since joining the Flinders Accelerator for Microbiome Exploration (FAME) I’ve continued to devote a lot of my energy to research software engineering. Viral metagenomics is still somewhat in its infancy and there is no shortage of opportunities for research software engineering projects in this field.

What is your contribution to ‘Hecatomb’ and what is the impact of this tool for your community?
-----------------------------------------------------------------------------------------------

[Hecatomb](https://github.com/shandley/hecatomb) was originally designed as a tool for read-based annotation of viral sequences. Our collaborator Scott Handley at Washington University in St. Louis created the original pipeline as a collection of bash and R scripts. Shortly after I joined FAME, in January 2021, I took on the role of developing Hecatomb to get it ready for [publication](https://doi.org/10.1101/2022.05.15.492003). I overhauled most of the pipeline to make it more efficient, robust, and user-friendly. I also included thorough [documentation](https://hecatomb.readthedocs.io/en/latest/) and tutorials in R and Python performing the data analysis. I wasn’t completely happy with manually kicking off a Snakemake pipeline, so I created a command line interface that makes running the pipeline a breeze. It’s still early days for Hecatomb, but we’ve already used it in [several publications](https://scholar.google.com.au/scholar?cites=2557935544862184627&as_sdt=2005&sciodt=0,5&hl=en) and many other ongoing projects. We’ve also run a few workshops on Hecatomb and have had a lot of interest from the community.

![Logo of Hecatomb, where the letter 'o' is a virus](https://ardc.edu.au/wp-content/uploads/2023/01/hecatomblogo.png)

What does winning the ‘Torsten Seemann’ award for an Outstanding Bioinformatics Software Developer mean to you and your career?
-------------------------------------------------------------------------------------------------------------------------------

I was blown away to learn that I had won the [‘Torsten Seemann’ Outstanding Software Developer Award](https://www.abacbs.org/awards). It was [Torsten](https://findanexpert.unimelb.edu.au/profile/704966-torsten-seemann)’s talk at BioInfoSummer 2016 on developing bioinformatics software that motivated me to publish my first pipeline and I’ve been hooked on writing software ever since. I would love to pursue a career in academia as a group leader. There is unfortunately a lot of attrition at my career level, especially given the current state of research funding, but this award will go a long way in helping me to realise this dream. 

At FAME we understand the value of awards for students and ECRs. We spend a lot of time and effort helping the lab members polish their posters and talks ahead of conferences and we’ve been quite successful so far. It’s exciting to see ABACBS and the ARDC supporting research software engineering with these awards and I’ll be doing everything I can to promote them in the years to come.

What have you learned through your experience developing workflows?
-------------------------------------------------------------------

Great question! Our paper “Ten simple rules and a template for creating workflows-as-applications” tackles a lot of these and it ships with example templates ([read the article](https://doi.org/10.1371/journal.pcbi.1010705)). 

The biggest lesson if you’re just starting out in bioinformatics would be to use a workflow manager like [Snakemake](https://snakemake.readthedocs.io/) or [Nextflow](https://www.nextflow.io/). They do so much heavy lifting for very little effort. Even when I’m doing a one-off analysis, I’ll make a Snakemake pipeline because it’s easier overall than dealing with bash scripts and it makes sharing your code more [FAIR](https://doi.org/10.15497/RDA00068). 

Also, don’t be afraid to reach out and ask for help. After Hecatomb, I decided to write the 10 simple rules paper based on what we had done with our command line interface for the Snakemake pipeline. I saw that [Titus Brown’s group](http://ivory.idyll.org/lab/) were already doing the same thing with their pipelines and had much better ways of incorporating some of the features. I also reached out for help with Nextflow and overall the paper was much better because of these awesome collaborators. 

Which research software communities do you recommend?
-----------------------------------------------------

I’m a member of a few societies that I would highly recommend. [The Australian Bioinformatics And Computational Biology Society (ABACBS)](https://www.abacbs.org/) is the premier society for anything biology plus computers. If you use workflow managers often you should consider the [BioCommons workflow community](https://www.biocommons.org.au/events/workflows-community-meeting). 

While not specifically software-focused, software is becoming ever more crucial in all facets of research and the more traditional societies have a growing representation of software creators. I’m the state representative for South Australia for [the Australian Society for Biochemistry and Molecular Biology (ASBMB)](https://www.asbmb.org.au/) and I’m on the committee for [the Adelaide Protein Group (APG)](https://apg.asn.au/) which is a special interest group of ASBMB. If you like microbes, check out [the Australian Society for Microbiology (ASM)](https://www.theasm.org.au/) and [the Joint Academic Microbiology Seminars (JAMS)](https://jams.org.au/). 

Keep In Touch
-------------

You can connect with Michael via [GitHub](https://github.com/beardymcjohnface), [Twitter](https://twitter.com/BeardyMcFace), [Mastodon](https://mastodon.social/@BeardyMcJohnFace@genomic.social), and [LinkedIn](https://www.linkedin.com/in/michael-roach-33327340/).

If you’d like to be part of the growing community of research software engineers in Australia, become a member of [the RSE Association of Australia and New Zealand (RSE-AUNZ)](https://rse-aunz.org) (it’s free!). 

Research Software Awards Open for Submissions
---------------------------------------------

### For Astronomy

The Astronomical Society of Australia (ASA) has launched the Emerging Leaders in Astronomy Software Development Prize, sponsored by the ARDC, which is now open for nominations with a closing date of Wednesday 15 February 2023. [Apply now >](https://asa.astronomy.org.au/prizes_and-grants/prizes-awards/astronomy-software-development-prize/)

### For Ecology

The Ecological Society of Australia has an ARDC-sponsored award for New Developers of Open Source Software in Ecology. Find out about last year’s winner [in our recent interview](https://ardc.edu.au/article/shaping-research-software-an-interview-with-fonti-kar/). If you are creating or maintaining research software for ecology. [Apply now >](https://www.ecolsoc.org.au/awards/ardc-award-for-new-developers-of-open-source-software-in-ecology/)

### For Statistics

Entries for the 2023 Statistical Society of Australia (SSA) Bill Venables Award for new developers of open source software for data analytics, sponsored by the ARDC, will open in early March 2023. [More information >](https://statsocaus.github.io/venables-award/)

### Eureka Prize for Excellence in Research Software

Entries to the 2023 Australian Research Data Commons Eureka Prize for Excellence in Research Software will open on Monday 13 February. [More information >](https://australian.museum/get-involved/eureka-prizes/enter/research-software/)

Start planning your submission now!

Stay tuned for our next interview in the Shaping Research Software series, coming out in March. 

**Learn more about the ARDC’s [Research Software Agenda for Australia](https://ardc.edu.au/collaborations/strategic-activities/a-research-software-agenda-for-australia/).**

_The ARDC is funded through the National Collaborative Research Infrastructure Strategy (NCRIS) to support national digital research infrastructure for Australian researchers._

### Author

Dr Paula Andrea Martinez, ARDC

### Reviewed by

Jo Savill, ARDC and Dr Tom Honeyman, ARDC

Follow RSE-AUNZ
---------------

*   [Twitter](https://twitter.com/RSE-AUNZ)
*   [Linkedin](https://www.linkedin.com/groups/13836034/)
