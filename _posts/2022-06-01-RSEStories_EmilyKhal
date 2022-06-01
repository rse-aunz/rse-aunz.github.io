---
layout: post
title:  "RSE Stories: An Interview With Dr Emily Kahl"
from:   2022-06-01 00:00:00
tags: ["RSE", "RSEStories", "ARDC", "2022"]
published: true                     
---

![Banner show A rendering of a simulation of butane molecules flowing through a carbon nanotube. Credit: Dr Emily Kahl](/assets/2022-06-01__butane_nanotube.png)

Posted by Paula Martinez on 1 June 2022

<em>This post was originally published as a news item on the 
    <a href="https://ardc.edu.au/news/shaping-research-software-an-interview-with-dr-emily-kahl/"
target="_blank" rel="noopener noreferrer">Australian Research Data Commons website (1 June, 2022)</a>.
</em>

As part of the [Research Software Agenda for Australia](https://ardc.edu.au/collaborations/strategic-activities/a-research-software-agenda-for-australia/), the ARDC is working with the research community to shape better research software in order to recognise it as a first-class output of research.

This interview is the first one in a series about research software engineers. Each month we will talk to a leading research software engineer about their experiences and best-practice tips in creating, sustaining and improving software for research.

In our first interview in the series, we talk to [Dr Emily Kahl](https://aibn.uq.edu.au/profile/7681/emily-kahl), a Scientific Programmer aka research software engineer at the Australian Institute for Bioengineering and Nanotechnology (AIBN) at the University of Queensland.

## What do you do in your role as a research software engineer?
I work with a **computational chemistry research group**, where my duties are split between directly supporting the researchers in my group and contributing to writing open-source molecular simulation software. Right now, my goal is to incorporate some of the important theoretical techniques developed by my colleagues into pre-existing molecular dynamics software to increase their adoption among the wider computational chemistry community.

## How did you come to work as a research software engineer?
I started considering moving into a research software engineering (RSE) role as I was finishing up my PhD. My research was in computational physics, but I discovered I like the ‘computational’ part more than the ‘physics’ part. I wanted to stay working in research and development because I like working on open-ended, exploratory projects, so the support-focused role of a research software engineer sounded ideal to me. I'm really enjoying the mix of software engineering and theoretical chemistry - the wide variety of problems to solve really keeps me on my toes!

## How does your work as a research software engineer advance research?
I am particularly proud of my efforts towards improving the adoption of new theoretical methods in the widely-used software suites [LAMMPS](http://lammps.org/) and [CP2K](https://www.cp2k.org/).

_The most popular molecular simulation programs are used by thousands (or even tens of thousands) of researchers worldwide, so adding new methods or fixing errors is a huge force multiplier compared to writing your own code from scratch._

As you might expect, the large projects all use different programming languages, design principles and coding styles, so you need to write a new implementation for each codebase you want to contribute to. This is the kind of task that is perfectly suited to an RSE role: letting the researchers research rather than getting stuck in the weeds of software engineering.

## Tell us about a project you have enjoyed working on
Right now, I'm really enjoying writing an interactive graphical front-end for my group's in-house **molecular dynamics software**. In a molecular dynamics calculation, you simulate the motion of individual atoms in a system (usually a liquid solution) using Newton's laws of motion, then use a physics framework called statistical mechanics to link the molecular motion to observable thermodynamic properties, like temperature and pressure. We have some Fortran 77 code to simulate simple fluid flow, but it's got a somewhat intricate command-line interface that can be hard for users to get their head around at first (especially if they've never used a terminal before!).

I have been writing a bare-bones interface in python and Qt that shows the positions of the particles as they evolve over time and lets the user dynamically adjust parameters like temperature and density to observe how they change the atom's movement. It's been an **extremely effective educational tool**: I've found myself learning lots of new things about the physics of liquids, simply because it's so easy to play around with various parameters and get immediate visual feedback on how it changes the behaviour of the system. We've already had an undergraduate summer research student use the program to learn about phase transitions (e.g. freezing and boiling) and even make her own modifications to simulate new kinds of particles. It was very satisfying to see a project make the jump to a fully-fledged tool that people use to do their research.

## What best practices for quality software do you implement in your work?
The biggest "game-changer" for me has been automated software testing, especially the continuous integration (CI) workflow. **Tests drastically reduce the time taken to ensure changes and modifications haven't broken anything.**

The benefit of continuous integration is that the tests are automatically run whenever anyone makes changes in the code repository (e.g. GitHub or GitLab), so you can immediately see whether a particular change passes the tests and if not, which contributor broke the build. This means that bugs are caught much more quickly and reliably than a purely manual process. It takes some time to set up, but has done more to improve our code quality than any other tool I've tried.

If you use GitHub or GitLab for version control, I highly recommend checking out their CI tools: [GitHub Actions](https://github.com/features/actions) and [GitLab CI/CD](https://docs.gitlab.com/ee/ci/), respectively.

## What communities are you part of that you would recommend?
1. The Pawsey Supercomputing Centre has done a tremendous job building and https://pawsey.org.au/pawsey-friends/maintaining a community of supercomputing users and developers over the last few years. They offer a lot of excellent training workshops and their newsletter is a fantastic source of news and links from the supercomputing world. Even if you don’t yet have a project with Pawsey, it's well worth subscribing to the [Pawsey Friends newsletter](https://pawsey.org.au/pawsey-friends/).
2. Speaking of newsletters, I really enjoy [**Jonathan Dursi's weekly newsletter Research Computing Teams**](https://www.researchcomputingteams.org/). It has a great mix of commentary on research software engineering and how to effectively manage RSE teams. The latter topic is a very underserved niche, as there's lots of great information about managing ‘ordinary’ software engineering teams, but it's much harder to find advice focused on the unique aspects of a research environment. Jonathan also regularly engages with readers and their comments, so it feels more like a community than a link-dump.
3. [The Rust programming language](https://www.rust-lang.org/community) has one of the best communities in the field of computer science and is worth participating in, even though it's not (yet) widely used in research computing. The Rust community strongly values inclusivity and diversity, and knowledgeable members put in heaps of effort to on-board new contributors. Even when the discussions are not directly relevant to my work, I still come away with something that changes how I think about some aspect of computing.

You can connect with Emily via her [personal programming blog](https://emilyviolet.github.io/), [GitHub](https://github.com/emilyviolet), her [researcher profile](https://aibn.uq.edu.au/profile/7681/emily-kahl) and [Twitter](https://twitter.com/atomwitch).

Stay tuned for our next interview in the Shaping Research Software series, coming out in July.

If you’d like to be part of the growing community of research software engineers in Australia, become a member of the [RSE Association of Australia and New Zealand (RSE-AUNZ)](https://rse-aunz.github.io/) (it’s free!).

Learn more about the [ARDC’s Research Software Agenda for Australia](https://ardc.edu.au/collaborations/strategic-activities/a-research-software-agenda-for-australia/).

_The ARDC is funded through the National Collaborative Research Infrastructure Strategy (NCRIS) to support national digital research infrastructure for Australian researchers._

Dr Emily Kahl was interviewed by Dr Paula Andrea Martinez, ARDC. Reviewed by Jo Savill (ARDC), Dr Tom Honeyman (ARDC).
