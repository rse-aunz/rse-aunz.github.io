# RSE Australia/New Zealand Unconference 2022
## Accessibility Report

### Liz Hare, Ph.D.

---

The professional conference landscape has changed considerably over the last few years.
We have learned from the COVID-19 pandemic that conference environments can 
evolve to become more diverse and inclusive[^1]. 
Organizing a conference that 
is accessible for colleagues with disabilities is an important way to ensure a large 
group of presenters and participants from all career stages will attend.
Accessibility is the responsibility of the conference organizers and presenters.
Accessibility practices are the steps we take to make sure an event is accessible
to as many people as possible, like transcripts and text captions of speech, 
alternative (alt)-text descriptions of images,
and providing more frequent breaks.

[^1]: Joo R, Sánchez-Tapia A, Mortara S, Bellini Saibene Y, Turner H, Hug Peter D, Morandeira NS, Bannert M, Almazrouq B, Hare E, Ación L. Ten simple rules to host an inclusive conference. PLoS computational biology. 2022 Jul 21;18(7):e1010164.

Moving conferences online has made them more accessible in many ways, but
some barriers to full participation are often overlooked by organizers. 
This report will evaluate the components of the 
[RSE Asia-Australia Unconference 2022](https://rse-aunz.github.io/2022-Asia-Australia-unconference/) 
and make suggestions for removing accessibility 
barriers. Some of these will be easy to respond to for this year's conference, 
while others will require more advance planning and budgeting and can be 
implemented in future years or other conferences.

##  Overall Communication Strategy

The conference will be welcoming if you show that access has been 
considered. This involves

- Avoiding the requirement for people to ask for accessibility practices 
or disclose their disabilities to organizers  

  - Designating an individual contact person (or email address) to answer 
questions about accessibility. 
Answer questions promptly, or update the 
participant about delays in finding the answer.  

  - Describing accessibility practices (like captioning) planned for the 
conference in a section of the conference website or email promotions so potential participants
can find the information easily.  

- Making sure all media (social media posts, emails, and websites) and 
software components (video, chat, and registration) are accessible:  

  - Images must have descriptive alt-text  

  - Accurate captions should be included in all videos  

  - Contrast, text size, and color palettes should make media easily accessible  

  - Media must be navigable with a screen reader  

  - Media can be navigated fully from the keyboard (rather than relying on 
mouse use)  

- Providing frequent breaks in the schedule. long sessions without breaks are a barrier to people with many types of disability. 
This is increasingly relevant 
  in the time of Long Covid. Breaks should occur every hour.  
  
  
- Providing accessibility standards for presenters, listing expected accessibility practices for their talks and providing references about how to implement them (see Section 3).  


- The language used to talk about any group of people is important. 
 Learn and use the words used by individuals or disabled communities to describe themselves.
 
  - Plain, direct communication is preferred. It's fine to say things like 
  "blind," "deaf". and "disabled."  
	
  - Avoid euphemisms like "challenged" or "differently abled."  
	
  - Avoid talking about disability as "inspiring." 
[This is an excellent talk from a disabled Australian woman about "inspiration porn!"](https://www.ted.com/talks/stella_young_i_m_not_your_inspiration_thank_you_very_much/transcript)  

## Software Components and their Accessibility

For this conference, registration is on EventBrite, the website is hosted
on GitHub, and the conference will take place on Zoom. 

### EventBrite

The EventBrite platform is not optimized for screen reader use. 
I have tested the process for other events on Mac and an iPhone with the VoiceOver screen 
reader. 
Signing up for a free event is difficult but I was able to do it.
However, I was not able to get through the process of charging a paid event to a
credit card. As a result, there are likely to be people either giving up 
on attending or contacting the organizers to ask for an alternative
way of paying. 

### Suggestions

For this year, the organizers should find alternative ways for people
who can't use eventBrite to pay. In future years, a more accessible
registration system should be selected. 
We used [Conftool](https://www.conftool.net//index.php)
for [useR! 2021](https://user2021.r-project.org) successfully and the 
developers were even willing to help fix accessibility issues.

### Website

In general, GitHub and Markdown provide an accessible environment to host
the information about the conference. The banner graphic has descriptive 
text, and the table is easy to navigate with a screen reader. The 
conference flyer is in .png format and is inaccessible with 
a screen reader.   

#### Suggestions

For the conference flier, consider another format like markdown/HTML or PDF 
that has been created to be accessible ([Adobe](https://csuf.screenstepslive.com/m/96806/l/1474315-alt-text-for-images-in-adobe-acrobat-pdf) 
and [Microsoft Office](https://support.microsoft.com/en-us/office/create-accessible-pdfs-064625e0-56ea-4e16-ad71-3aa33bb4b7ed)
have facilities for this.

For the conference website, the heading "Accessibility and Inclusivity" on the website would be a perfect place to provide information about
accessibility practices like captions, accessibility standards for presenters, and address other questions potential 
participants might have about disability-related access.  

The website provides an email address for questions, 
which is a good step toward communicating about accessibility.
Consider having a dedicated email address for disability-related 
accessibility communication. Potential participants will need 
these answers before deciding whether to submit proposals
for presentations or to attend the conference. In the future, 
this information should be available when open submissions are 
first announced. Questions about accessibility should be 
answered promptly and not leave the participant wondering
if their query reached anyone who can find answers or fix
problems.  Don't charge late fees if answers could not be 
provided before early registration closes.

### Zoom

Most important features of Zoom are accessible to people with disabilities. 
Zoom has prioritized accessibility more than many other platforms. 
It is in wide use, so some people will be quite familiar with it. 
Others may be less experienced and take more time to find their way around the interface.

Historically, conference presentations rely on the assumption
that the audience receives information on two channels: they look at 
the slide to appreciate some of the information, while listening
to the author explain the content. 
The synthesis of the information from
these two channels leads to comprehension of the presentation. 
For example, in a presentation about statistical analysis code
the slides are likely to contain the precise code while 
the verbalized part of the talk might be more general or 
explanatory. For people with sensory disabilities, there 
are accessibility practices to provide the missing information.  

Accurate captions are critical for the participation of people who are deaf or 
hard-of-hearing. They also benefit people who are logging in
from noisy environments or whose primary language is not English. Zoom 
provides automatic captions at no cost, however, they are not accurate
enough for specialized or technical language. They cannot properly recognize 
vocabulary like software package and function names, code, and 
terms related to data science or statistics. (Deaf people call these
"craptions.") 

#### Suggestions

Captions should be provided by humans who have an 
opportunity to familiarize themselves with the field in advance. There are 
many services that provide these "live captions." One that has been effective in the R
community is [White Coat Captioning](https://whitecoatcaptioning.com).

Since some deaf people use sign language as their first language, it can
be an ideal accessibility practice. Interpreters should also have an opportunity to become familiar with the field and its vocabulary. One 
complication with sign language interpretation is that each country
has its own sign language. Since this conference is focused on Australia, 
Auslan interpretation should be considered.

Both live captions and sign language interpreters can be integrated easily 
into Zoom presentations. The Zoom environment should be set up 
so the user can make the presenter, the slides, and the interpreter visible
(not small images).

Live captions and sign language interpreting are intensive work and 
are likely to be the most expensive accessibility practice for a
conference. They are important and their price requires advance planning both logistically (scheduling) and raising funds through either
sponsors or registration fees. Some universities can help with logistics.

For people who are blind or have low vision, the missing part of a
Zoom presentation is the slides. Screen reading software only works
with static text: it cannot recognize text in videos or describe images in
videos. To provide the details from the slides, the slides should be 
made available in advance so they can be read along while listening to the presentation or in preparation to understand it. 
Presenters should be encouraged to describe images and verbalize the concepts
that their slides show. There is more information in Section 3
about providing presenters with accessibility standards.  

Presenters who are aware of describing all the elements of their slides often 
slow down their talks in a way that benefits people with many kinds of disabilities.  

## Accessibility Standards for Presenters

Providing accessibility standards for presenters accomplishes two goals: 
providing access for participants with disabilities, and educating presenters,
who are usually more structurally privileged, about how to make their material 
more inclusive. We wrote accessibility standards with instructional resources
for [UseR!2021](https://user2021.r-project.org/participation/talks-access/).
Some presenters told us they learned a lot of things about making their work accessible, 
while others ignored the standards. 
In the future, one way the RSE-Australia/New Zealand Unconference could nudge
presenters toward implementing accessibility practices would be to have them
agree to follow accessibility standards as part of the submission process.  

Many of the accessibility standards for presenters are parallel with the 
recommendations for conference organizers. They are presented here with 
some learning resources.  

### The Slides

- Prefer slide formats like .Rmd/HTML or Python Notebooks/HTML. Sometimes source
code is more accessible to screen reader users. Silvia Canelón has
[a great tutorial post about creating Rmd slides using the Xaringan package](https://www.silviacanelon.com/talk/2020-xaringan-basics-and-beyond/).

- Avoid distracting transitions, flashing images, and complicated layouts.

- Ensure that images have alternative (alt) text so screen reader users can access their meaning. 
Some resources for learning about this descriptive text:

  - The [Diagram Center](http://diagramcenter.org/making-images-accessible.html)
  has guidelines and learning tools for writing alt-texts for STEM.  

  - [WGBH](https://www.wgbh.org/foundation/ncam/guidelines/guidelines-for-describing-stem-images) 
  also has guidelines for STEM images.
  For my opinion about their emphasis on brevity (I disagree that that's the #1 priority!), 
  see the next item.  

  - Communicating Science Through Meaningful Alt-Text, presented by Liz Hare to 
  the Time Scavengers Virtual Internship Program, June 2022  

    - [Slides](https://lizharedogs.github.io/TimeScavengersWorkshopAltText/#1) (press PgDn to advance slides)
	- [Video](https://drive.google.com/file/d/1Fj_qJM8bJtnAyd-UTMVeiUNw8cORSnM4/view?usp=sharing )  
  - Revealing Room for Improvement in Accessibility in a Social Media Data Visualization Community,
  Silvia Canelón and Liz Hare, CSV conf, May 2021  
  
    - [Slides](https://spcanelon.github.io/csvConf2021/slides/indexLH.html#1) (press PgDn to advance slides)
	- [Video](https://www.youtube.com/watch?v=DxLkv2iRdf8)
	
	
- Optimize the visibility of your slides by considering:  

  - Enough contrast for visibility
  [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)  
  
  - Color palettes that can be distinguished by everyone
  [How to Make Your Website Accessible for Color-Blind People](https://equalizedigital.com/website-accessibility-color-blind/)  
  
  - Text size large enough to be readable on small screens
  [Font Size on the Web](https://accessibility.psu.edu/fontsizehtml/)  
  
  - Choose fonts for readability
  

- Ensure that PowerPoint or PDF slides are created with accessibility features. 
  MS Office has an accessibility checker. Some instructions:  
  
  - [Adobe](https://helpx.adobe.com/acrobat/using/create-verify-pdf-accessibility.html)_  
	
 [MS Office](https://support.microsoft.com/en-us/office/make-your-powerpoint-presentations-accessible-to-people-with-disabilities-6f7772b2-2f33-4bd2-8ca7-dae3b2b3ef25) 
	Include alt-text and run the accessibility checker before saving slides as PDF.  
	
- Use the speaker notes feature of your presentation to provide further explanation of slides.

### DUring the talk


- Speak clearly and not too quickly. 
  Keeping your face visible will help people understand you by reading your lips or facial expression.
  Faking eye contact is not necessary, since some presenters will find this impossible or uncomfortable.  
  
- Mention slide numbers or headers when switching slides. 
  Use descriptions to help orient people following along with a screen reader.
  
- Avoid assuming that things are "obvious" in your slides. 
  Mention these things aloud.
  
  - 
  