---
layout: post
title:  "RSE Stories: An Interview with Catherine Bromhead"
from:   2023-07-31 0:00:00
tags: ["RSE", "RSEStories", "ARDC", "2023"]
published: true                     
---

RSE Stories: An Interview with Dr Adam Sparks
============================================

July 31, 2023

Posted by Johanna Bayer, 31 July 2023

This post was originally published as a news item on the [Australian Research Data Commons website (30 June, 2023)](https://ardc.edu.au/article/shaping-research-software-an-interview-with-dr-adam-sparks/).

Shaping Research Software: An Interview with Dr Adam Sparks
==========================================================

We spoke with Dr Adam Sparks, a bioeconomic modeller at the WA Department of Primary Industries and Regional Development who leads a team that develops software for agricultural decision making and research.

**Published:** 30 June 2023

![Adam Sparks in front of a computer](https://ardc.edu.au/wp-content/uploads/2023/06/shaping-research-software-an-interview-with-adam-sparks-feature-image-583-x-345-%E2%80%93-1-exclude-optimize-580x345.png)

As part of our [Research Software Agenda for Australia](https://ardc.edu.au/collaborations/strategic-activities/a-research-software-agenda-for-australia/), the ARDC is working with the research community to shape better research software in order to recognise it as a first-class output of research. This interview is part of a [series about research software engineers in Australia](https://ardc.edu.au/news-and-events/news/?_keyword=%22Shaping%20Research%20Software%22&_categories=research-software). Each month we talk to a leading research software engineer about their experiences and best-practice tips in creating, sustaining and improving software for research.

Continuing the series, we spoke with [Dr Adam Sparks](https://www.agric.wa.gov.au/adam-sparks), a bioeconomic modeller with Western Australia’s [Department of Primary Industries and Regional Development](https://www.wa.gov.au/organisation/department-of-primary-industries-and-regional-development) (DPIRD). He leads the Systems Modelling branch in the DPIRD’s Farming Systems Innovation Directorate. In this interview, we talked about the work of his team of 12, which includes data scientists, climatologists, meteorologists, biometricians and software developers.

Tell us about your team, their backgrounds and projects.
---------------------------------------------------------

The Systems Modelling branch has quite a mix of interesting backgrounds. It includes 6 modellers, research software engineers and data scientists – Dr Rodrigo Pires, Anna Hepworth, Matt Foster, Kenyon Ng, Jimmy Ng and Matthew Antulov. Rodrigo and Anna are senior modellers that work on developing agricultural system models and models for agricultural decision support tools. Rodrigo has a background in applied agronomy and plant sciences, and Anna has a statistics background in human health.

Matthew Antulov, on the other hand, programs in Julia in a cloud-hosted environment using Docker to build large Monté Carlo whole-farm simulation models using real farm data. Kenyon is currently a PhD candidate at the University of Melbourne studying statistical machine learning and working with my team on a casual basis to do some machine learning. Jimmy is a student in the University of New South Wale’s Health Data Science postgraduate degree program. He is working with us supporting work we do with R and gaining work experience. Matt has been working with us to convert models from mobile apps, mostly written in Typescript, to APIs written in .NET.

We also have 3 software developers in the team – senior back-end developer Fumie Horiuchi, senior UX/UI developer Steve Collins and full stack developer Liz Mackle, who completed the UWA code camp just before joining the DPIRD as a junior developer. Additionally, 2 biometricians, Dr Karyn Reeves and Tinula Kariyawasam, support the DPIRD’s research by providing statistically sound research trial designs and trial analysis. They also provide training to staff in biometric analysis methods.

What kind of projects does your group develop?
-----------------------------------------------

The team currently maintains a suite of 7 decision support tools for crop disease management, released as mobile apps for free in the Google Play and Apple app stores. They are developed specifically to be used by agronomists and farmers, though other researchers are also using them. Here are 3 examples of our spray decision support tool apps, which were developed as a part of and maintained with support from a [Grains Research and Development Corporation (GRDC) investment](https://grdc.com.au/grdc-investments/investments/investment?code=DAW2112-002RTX):

*   [UCI BlacklegCM](https://www.agric.wa.gov.au/apps/uci-blacklegcm-blackleg-upper-canopy-infection-management-app)
*   [PowderyMildewMBM](https://www.agric.wa.gov.au/apps/powderymildew-mbm-powdery-mildew-management-app-mungbean)
*   [YellowSpotWM](https://www.agric.wa.gov.au/apps/yellowspotwm-yellow-leaf-spot-management).

![Screenshot of the mobile version of the UCI BlacklegCM app](https://ardc.edu.au/wp-content/uploads/2023/06/uci-blacklegcm-mobile-app.png)

_The mobile implementation of UCI BlacklegCM, a tool designed to help growers and consultants with management decisions for canola upper canopy blackleg infections in Australia_. _It factors in grain price, input costs, yield benefits, seasonal conditions, crop circumstances and conditions, state, fungicide strategies and other diseases to give the best-case, worst-case and most likely estimates of financial return from different management strategies_

We also maintain 2 other sibling mobile apps available for free. One being the [PestFacts WA Reporter](https://www.agric.wa.gov.au/apps/pestfacts-wa-reporter-app) app. Anyone can use it to submit quick reports or request identifications of insects and plant diseases in broadacre crops and pasture paddocks anywhere in the WA grainbelt. The second app is for New South Wales and Victoria, the [PestFacts VIC and NSW](https://www.agric.wa.gov.au/apps/pestfacts-victoria-and-new-south-wales) app, also for reporting crop and pasture pests and beneficials. Both are part of the broader initiatives [PestFacts WA](https://www.agric.wa.gov.au/newsletters/pestfacts-wa) (maintained by us) and [PestFacts map](https://cesaraustralia.com/resources/pestfacts-map/) (maintained by Cesar Australia).

Fungal disease in crops is of concern to growers and prompts disease control actions. Kenyon is building an object-detection pipeline in Python for identifying tiny mushroom-like structures from photos taken around WA. The pipeline automates the first review of the photos and curates those that need a second look before decisions are made and alerts are made based on the presence of these structures in the photos, which mean that crop disease will soon start to appear.

Used to counter the effects of soil acidification due to common agricultural practices, lime is vital to agriculture, but costly. One of our major projects is building a Monté Carlo model to simulate whole-farm liming for investment decisions. We’re working with the [Grower Group Alliance](https://www.gga.org.au/), [AxisTech](https://axistech.co/) and Curtin University’s [Centre for Crop and Disease Management](https://www.ccdm.com.au/) to be able to model a whole farm using actual farm data (WA Farm Data Sharing FA099). Using a new DPIRD API platform, called Extrata, we transfer farmers’ data to be used in modelling liming strategies to our Nimbus instance at the Pawsey Supercomputing Research Centre and generate liming strategy reports, which are mainly used by farmers and agronomists. At the heart of it, we’re using Julia to interface with a .NET API that Matt Foster wrote based on the [iLime](https://www.agric.wa.gov.au/apps/ilime) app. We chose Julia because it’s easy to use while also providing high performance. Matthew Antulov is the main architect of the model despite only having learned Julia since he started working with us. The goal of the project is that this model will support investment decisions beyond whole-farm liming in the future. You can read more about it on the [Grower Group Alliance’s website](https://www.gga.org.au/activity/wa-data-exchange/).

We maintain several packages that support agricultural research, and we develop in R, Julia and Python. Most of our daily work is in R, which is certainly what I’m the most comfortable with. We use it in biometrics, especially the [ASReml-R package](https://vsni.co.uk/software/asreml-r) for analysing agricultural research trials. We also use it to conduct Bayesian analysis for plant disease research and evaluate the [state of openness and computational reproducibility in the discipline of plant pathology](https://doi.org/10.1094/PHYTO-10-21-0430-PER). We also have 2 R packages available as open-source-software via the [DPIRD’s Farming Systems Innovation GitHub organisation account](https://github.com/DPIRD-FSI).

How does your team make these tools available?
----------------------------------------------

You could say our development process is unique. As I mentioned, we mainly use R in our day-to-day work. Previously, developing models involved having meetings, maintaining spreadsheets and running executable Mathematica code past experts. The R Shiny apps have been a game changer. We now have R Shiny versions of most of the models for prototyping, testing and validation with plant pathology experts before we release them as mobile apps. We like to keep the R versions up to date. This allows us to implement changes to the model and test with large data sets and get user feedback interactively in a reproducible programmatic environment. The model would be modified by Anna, tested in the R version and then translated into an app using TypeScript by Fumie with Steve putting the finishing touches. This makes it easier to conduct unit testing and quicker to deploy changes to receive expert feedback. After the release, Liz would keep the app up to- date with changes with Steve and Fumie’s guidance.

Moreover, it was a pleasant surprise that some of the Shiny apps have been used for teaching exercises by university instructors teaching plant disease epidemiology courses. This is just [one example of what one of our Shiny apps look like](https://dpird-disease-models.shinyapps.io/UCI-blackleg/).

![Screenshot of the Shiny version of the UCI Blackleg CM app](https://ardc.edu.au/wp-content/uploads/2023/06/uci-blacklegcm-r-shiny-implementaiton.png)

_The R Shiny implementation of UCI BlacklegCM_

What do successful team dynamics look like to you?
--------------------------------------------------

One of the best parts of the job is mentoring the team. Matthew Antulov has been a great asset to the team. He started with us after having only interned with a private mining company and doing some work with Python. It’s been extremely rewarding to see him grow and the quality of his work improve. Some younger early-career members also became mentors to junior members of the team. This led to a strong team dynamic, where someone will always be there to help and there’s no hesitation to ask questions.

We’re relatively lucky to have the entire team based in our main offices in Perth, rather than spread out. That makes it easier to maintain good dynamics as we can spend time together talking about shared interests. But of course not everyone is in the office at all times, so there’s our Teams chat, which has its fair share of silliness as well as seriousness.

What communities are you part of and recommend?
-----------------------------------------------

I’m currently a member of the [Australasian Plant Pathology Society](https://www.appsnet.org/) because of my training in botanical epidemiology and plant disease modelling. I’m also very involved in [rOpenSci](https://ropensci.org/), where I serve as an Associate Editor for code review for both regular peer review and statistical software. rOpenSci has been a fantastic community to be a part of as an R programmer, and serving as an editor is a chance to give back to the community. While I’m not currently a member, I do also recommend the [Statistical Society of Australia](https://www.statsoc.org.au/), if you’re interested in this area.

If you’d like to be part of the growing community of research software engineers in Australia, become a member of the [RSE Association of Australia and New Zealand (RSE-AUNZ)](https://rse-aunz.org/) – it’s free!

Keep In Touch
-------------

You can connect with Adam via [Linkedin](https://www.linkedin.com/in/adam-h-sparks-507b968b/), [Github](https://www.github.com/adamhsparks/) and [Mastodon](https://fosstodon.org/@adamhsparks). You can also learn more about him and his research on his [personal website](https://adamhsparks.netlify.app/).

Research Software Awards Updates
--------------------------------

### Venables Award

The winners of the 2023 Venables Award for New Developers of Open Source Software for Data Analytics have been announced!

*   Winners: Matthew Sainsbury-Dale and Andrew Zammit-Mangion for [Fixed Rank Kriging (FRK)](https://andrewzm.github.io/FRK/)
*   Runners-Up: Rex Parsons, Robin Blythe, Adrian Barnett, Susannna Cramb and Steven McPhail for [predictNMB](https://docs.ropensci.org/predictNMB/index.html)
*   Honorable Mentions: Katie Buchhorn and Lukasz Mentel for [gnnad](https://github.com/KatieBuc/gnnad); Mark Hanly for [daggle](https://cbdrh.shinyapps.io/daggle/)

Presented by the Statistical Society of Australia (SSA) and sponsored by the ARDC, the award encourages new open-source software development from the Australian community with a view to support efforts to develop and share data science and statistics methodology. Learn more on the [SSA website](https://statsocaus.github.io/venables-award/).

**Stay tuned for the August instalment of our Shaping Research Software series, which will feature Matthew and Andrew.**

### Emerging Leaders in Astronomy Software Development Prize

The winner of the inaugural Emerging Leaders in Astronomy Software Development Prize has also been announced!

*   [Dr Manodeep Sinha](https://www.scienceinpublic.com.au/media-releases/asawinners2023), for outstanding contribution to the development of open-source astronomical software by an early career researcher

The prize is presented by the Astronomical Society of Australia (ASA) and sponsored by the ARDC. Learn more on the [ASA website](https://asa.astronomy.org.au/prizes_and-grants/prizes-awards/astronomy-software-development-prize/).

### New Developers of Open Source Software in Ecology

The winners for this year’s New Developers of Open Source Software in Ecology award will be announced at the [2023 Ecological Society of Australia Conference](https://ardc.edu.au/event/2023-ecological-society-of-australia-conference/), which will be held in Darwin from 3 to 7 July.

**Learn more about the ARDC’s** [**Research Software Agenda for Australia**](https://ardc.edu.au/collaborations/strategic-activities/a-research-software-agenda-for-australia/)**.**

_The ARDC is funded through the National Collaborative Research Infrastructure Strategy (NCRIS) to support national digital research infrastructure for Australian researchers._

### Author

Dr Paula Andrea Martinez (ARDC)

### Reviewed by

Jason Yuen (ARDC), Dr Tom Honeyman (ARDC)

Follow RSE-AUNZ
---------------

*   [Twitter](https://twitter.com/RSE-AUNZ)
*   [Linkedin](https://www.linkedin.com/groups/13836034/)


[](/2023/07/0X/RSEStories_DrAdamSparks.html)

### RSE Australia / New Zealand

*   *   [rse-aunz](https://github.com/rse-aunz/rse-au/issues)
    *   [rse\_aunz](https://twitter.com/rse_aunz)

A community for academics and professionals who work with software in the research domain.

Want to keep up to date?    [Sign up here!](https://groups.google.com/forum/#!forum/rse-nz-au/join)
