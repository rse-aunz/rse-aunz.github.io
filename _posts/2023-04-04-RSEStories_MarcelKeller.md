
Shaping Research Software: An Interview With Dr Marcel Keller
=============================================================

We interview Dr Marcel Keller, a cryptographer from CSIRO’s Data61 working on multi-party computation.

**Published:** 3 April 2023

![Dr Marcel Keller from CSIRO's Data61](https://ardc.edu.au/wp-content/uploads/2023/04/interview-with-dr-marcel-keller-feature-image-583-x-345-580x345.png)

As part of our [Research Software Agenda for Australia](https://ardc.edu.au/collaborations/strategic-activities/a-research-software-agenda-for-australia/), the ARDC is working with the research community to shape better research software in order to recognise it as a first-class output of research. This interview is the [tenth in a series](https://ardc.edu.au/news-and-events/news/?_keyword=%22Shaping%20Research%20Software%22&_categories=research-software) about research software engineers in Australia. Each month we talk to a leading research software engineer about their experiences and best-practice tips in creating, sustaining and improving software for research. 

Continuing the series, we spoke with [Dr Marcel Keller](https://mkskeller.github.io/), a Senior Research Scientist at [CSIRO’s Data61](https://people.csiro.au/k/m/marcel-keller). Dr Keller is a cryptographer working on multi-party computation and the maintainer of [MP-SPDZ](https://github.com/data61/MP-SPDZ), a framework implementing multi-party computation. MP-SPDZ is written in C++ and Python.

How would you explain your research focus to a general audience?
----------------------------------------------------------------

Multi-party computation (MPC) is one of the main privacy-enhancing techniques. It allows computing on secret data without revealing it. An example of how it can be used is the millionaire’s problem, where 2 people want to find out who is richer without revealing their actual wealth. There is clearly more information in the wealth difference (several bits of information), than there is in the answer of who is the richest (one bit of information). With MPC, the 2 parties can run a protocol that reveals the answer without revealing any of the inputs. It therefore provides a property called input privacy. In a more practical example, MPC could be used by a number of healthcare providers to find the markers of disease by pooling patient data without revealing the patient data to any other party. 

How did you end up in your current role? 
-----------------------------------------

I used to work as a software engineer and I felt there was something missing. My duties as a software engineer were at times mundane, such as transcribing code from one language to another. Then I started a PhD, in contrast, I sometimes missed hands-on work with software. In my postdoc at the University of Bristol, I could finally combine the two, by focussing on practical applications of MPC and working on [the predecessor of MP-SPDZ](https://github.com/bristolcrypto/SPDZ-2). In my current role at CSIRO’s Data61, I have been given the opportunity to expand this to a broader project where I am wearing even more hats: developer, maintainer, dev-ops engineer, and application support to name a few. It is this diversity of tasks that I really enjoy. 

Why do you think secure multi-party computation (MPC) will continue to be in demand in the future?
--------------------------------------------------------------------------------------------------

I think that the issue of privacy and thus privacy-enhancing technologies (PETs) will only increase in the coming years. In the last year there has been a flurry of documents highlighting the importance of PETs and MPC, be it by the [United Nations](https://unstats.un.org/bigdata/task-teams/privacy/index.cshtml), the [Royal Society of London](https://royalsociety.org/topics-policy/projects/privacy-enhancing-technologies/), the [OECD](https://www.oecd-ilibrary.org/science-and-technology/emerging-privacy-enhancing-technologies_bf121be4-en), or a [joint competition by the UK and US governments](https://petsprizechallenges.com/). In Australia, the Australian Transaction Reports and Analysis Centre (AUSTRAC) is exploring [privacy-preserving analytics to combat financial crime](https://insight.thomsonreuters.com.au/business/posts/australia-unveils-world-first-privacy-preserving-fintel-encryption-project). 

How does your work as a research scientist advance the value and translation of your research tool?
---------------------------------------------------------------------------------------------------

There are a number of frameworks in the space, but I find them rather limited in one way or another. Many of them do not provide a platform for general computation but simply insert MPC functionality into machine learning frameworks like PyTorch, which limits the potential applications. Most frameworks also limit themselves to one or a few MPC protocols (of which there are many, catering to a number of settings in terms of the number of participants and security assumptions). MP-SPDZ is the only framework that offers more than 40 protocol variants and an interface that is both general and relatively easy to use. I believe that this infrastructure approach and the open source is the reason for the rapid increase in its usage and citations. 

Could you highlight a few examples of the use of your tool?
-----------------------------------------------------------

The most high-profile use is by a research lab at Bosch, which has built a [](https://carbynestack.io/)[cloud-native framework](https://carbynestack.io/) around [MP-SPDZ](https://github.com/data61/MP-SPDZ). However, I think the breadth of use is more important than any specific user, because of the flexibility of the  infrastructure I mentioned earlier. On Google Scholar, there are about 90 papers mentioning the use of the software, of which 60 were added over the last 12 months alone. 

What communities or professional networks are you part of that you would recommend?
-----------------------------------------------------------------------------------

In terms of formal networks, I’m a member of the [International Association for Cryptologic Research](https://iacr.org/). They are a volunteer-run organisation that organises a number of conferences in cryptography. However, I would put more emphasis on informal networks that come out of attending conferences and participating in program committees. In particular, I would highlight the [Privacy Enhancing Technologies Symposium](https://petsymposium.org/), where I have been a member of the program committee for over 2 years. 

Keep in touch
-------------

If you’d like to be part of the growing community of research software engineers in Australia, become a member of the [RSE Association of Australia and New Zealand (RSE-AUNZ)](https://rse-aunz.org) (it’s free!). 

You can connect with Marcel via [Linkedin](https://www.linkedin.com/in/mkskeller/), [Github](https://github.com/mkskeller), [Twitter](https://twitter.com/mkskeller), [Mastodon](https://tech.lgbt/@mkskeller).

Research Software Awards Open for Submissions
---------------------------------------------

Eureka Prize for Excellence in Research Software:

Entries to the 2023 Australian Research Data Commons Eureka Prize for Excellence in Research Software is now open. [More information](https://australian.museum/blog/science/excellence-in-research-software/)[, closing on 14 April 2023](https://australian.museum/get-involved/eureka-prizes/enter/research-software/) [>](https://australian.museum/blog/science/excellence-in-research-software/)

For Statistics:

The 2023 Statistical Society of Australia (SSA) Bill Venables Award for new developers of open source software for data analytics, sponsored by the ARDC is now open [Apply now, closing on 22 April 2023 >](https://statsocaus.github.io/venables-award/)

Stay tuned for our next interview in the Shaping Research Software series, coming out in May. 

**Learn more about the ARDC’s** [**Research Software Agenda for Australia**](https://ardc.edu.au/collaborations/strategic-activities/a-research-software-agenda-for-australia/)

_The ARDC is funded through the National Collaborative Research Infrastructure Strategy (NCRIS) to support national digital research infrastructure for Australian researchers._

Dr Marcel Keller was interviewed by Dr Paula Andrea Martinez, ARDC.

### Author

Dr Paula Andrea Martinez, ARDC

### Reviewed by

Jo Savill, Dr Tom Honeyman, ARDC

### Categories

[Research Software](/news-and-events/news/?_categories=research-software)

### Research Topic

[Mathematical-Information and Computing Sciences](/news-and-events/news/?_topics=mathematical-information-and-computing-sciences)

### Related Program

*   [Implementing the Research Software Agenda for Australia](https://ardc.edu.au/program/research-software-program/)

### Related Projects

*   [Shape Research Software](https://ardc.edu.au/project/shape-research-software/)

