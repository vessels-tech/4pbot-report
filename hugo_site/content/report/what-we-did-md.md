---
date: '2018-02-10T21:30:10+10:30'
published: true
title: What We Did
weight: 4
---

This section is an overview of the process we took in building 4Pbot. We talk about the research we conducted, the plan and execution of 4pbot's development, and how we went about assessing the results from this project.



## Initial Research Phase

We began our first phase of research by, concentrating on the Philippines’ 4Ps program _todo: isn't this the entire of what we focused on?_. In this phase, we also researched financial services and financial literacy, in both general terms and their relevance and use in the Philippines.

In order to aid our research, Vessels employed a hired contractor, who was a Filipina, living in Cebu, Philippines. This contractor spoke two of the major dialects in the Philippines (Tagalog and Cebuano), and had connections to families a part of the 4Ps program.

Through this contractor, we were able to distribute 100 surveys across Cebu and Mindanao. None were distributed to Luzon at this time, as most of our contractor’s connections were in middle and southern islands of the Philippines. Later, Vessels was able to conduct online surveys via Facebook, as there appeared to be Facebook groups and communities, dedicated to 4P beneficiaries. In this way, we were able to reach an audience that spanned the entirety of the Philippines, but of course, was still limited in that it only pertained to active Facebook users.

Vessels also corresponded with other botmakers, most notably, Matt Wallace in Myanmar. Wallace has developed a chatbot for the organisation, _Opportunities NOW Myanmar_ [^9]. They use chatbot technology to train people who partake in their microfinance services. Even though the Opportunities NOW chatbot has more of an education application, Vessels was still able to glean valuable lessons in relation to the implementation of the chatbot.

## First Philippines Visit

Vessels embarked on its first Philippines visit in order to meet 4P beneficiaries face to face. At these meetings, the conversations were centered around problems with the welfare program, people’s daily experiences in relation to their finances, and their interaction and/or understanding with formal financial institutions.



![trip_1_line.jpg] (/media/trip_1_line.jpg)


_meeting beneficaries on a payout day - these women spent their entire day in a line for a single atm!_

Another group of people that Vessels met with were stakeholders, in both the Filipino Government and of other social enterprises. The purpose of these meetings was to discuss potential partnerships, and to talk and brainstorm around the application of chatbot technology for other services.



## Implementation

We decided to break down the implementation of 4pbot into 3 roughly defined 'sprints'. Each sprint represented a core part of work on building the bot, and ended with a short evaluation period of 5-10 days. This evaluation period was vital to help us learn quickly what was and wasn't working about the bot, focus on any bugs that needed squashing, or features that needed further tweaking.


## 0.1 Alpha

- The first sprint by far took longest to implement.
  - required building out all of the infrastructure (Zapier + Google Sheets + Google Firebase)
  - decided to build using an open source bot platform BotKit, which stops 4Pbot from being locked in to facebook
  - finding a good way to integrate
  - building our translation and content building pipeline
- Took ideas from trip, and decided to really hone in on these features:
  1. Date estimator
  2. Private reporting feature

  For now, 4pBot addresses 2 key areas that we at Vessels Tech have have identified we might be able to assist with the Filipino social welfare program, known as 4Ps:

      Payout dates are unreliable and unpredictable
      Clients don’t speak up about issues because they are embarrassed or afraid they will lose their payments.


- In addition, as they weren't too much more complicated to do, we built:
  1. Payment calculator (how much is my payout)
  2. 4Ps news - 3 short posts in local language about things going on with 4ps.

- by the time these were done, we launched 4pbot privately
  - This was following the advice of Matt Wallace (bot afficionado) - who had told me you only really get one shot with a bot on facebook. Once a user deletes you, you're gone!

- for the date estimator, we bootstrapped data from public posts about the 4ps and simply asking people on facebook

From our alpha release we had the following info:

Out of our 10 testers, 3 didn't get past the menu, 1 was unable to use a feature because they didn't know their zip code, 1 person didn't like the cover photo (maybe a little too impersonal), and 1 person thought the conversation with 4pbot was too jumpy.



## 0.2

- added a date report section, to help us crowdsource the payout dates
  - this is because other sources we were looking into didn't come through. For example, one of the local DSWD departments were in contact with said they don't even record the past payout date data! Seems a little silly to us.


Version 0.2 really prepared 4pbot for public release. We addressed many of the issues from the private release, and were able to catch and fix a few minor bugs before it went live.

We launched version 0.2 to the public on Nov 10, and promoted it heavily in 4Ps facebook groups; independently run groups of 4ps beneficiaries who get together and share their experiences,


The initial feedback from 4Pbot has been really positive. We have 250 unique users within 2 weeks of launching, with more growing everyday.
We have support from admins in 2 major Facebook groups for 4Ps clients, with >20,000 users and counting.


## 0.3

- removed payout date predictor. It simply wasn't accurate enough.
  - unfortunately this was our most popular feature.
  - Other workarounds were ineffective. We would rather have less users than patently lie to them.

Improved conversation flow and intelligence:
eg:
  - We found friction in the sign up process - not all users were comfortable giving us their phone number
    - added the ability to skip, or it gives up after a couple tries

Our summary for users in November and December is this:

|Indicator|November|December|
|---------|--------|--------|
|0.2 Feedback|😀 x 15 😐 x 5 😣 x 3  | - |
|0.3 Feedback | -  |😀 x 2 😐 x 😣 x 0|
|# of users assisted | 50| 25|
|# of complete vs abandoned conversations   |197/221   |173/195
|MAU   |253   |111   |

We can see the most active users in November when 4Pbot launched to the public. We saw this drop off (as expected) as people either grew bored of 4pbot, or didn't feel the need to come back. The date estimate feature was unfortunately the most popular by far (despite how inaccurate it was depending on the user's location), which also explains the decline in December.  Fortunately though, we saw almost as many conversations in December, and more complete conversations. This implies that the users who stuck with 4Pbot were using it more, and were finding it easier to use, as the ratio of complete conversations in Dec was greater than Nov.



## Second Philippines Visit

Vessels came back to the Philippines, to Toledo City,  and met face-to-face with a small subset of 4Pbot users; 6 middle-aged women. In our conversations, we asked them about their experience with 4Pbot and the 4Ps program. We also simply watched and took record of how the women used the bot.

We also took the opportunity to travel to Bantayan Island to visit a small village project. We did this with the next iteration of this project in mind. On Bantayan, we interviewed people, with the focus of discovering more about people’s financial situations. In doing so, Vessels was able to gain key insights into the different financial services and financial literacy amongst ordinary Filipino people.


![IMG_4659.jpg]({{site.baseurl}}/media/IMG_4659.jpg)
_conducting interviews about financial inclusion on Bantayan_

![IMG_4660.jpg]({{site.baseurl}}/media/IMG_4660.jpg)
_when I asked about whether or not this family had a bank account, this is what this gentleman showed me!_


[^9]:  Opportunities NOW describes themselves as an Entrepreneurship development system that seeks to reduce poverty by providing business training and mentoring in various stages of the business startup: <http://www.onowmyanmar.org/>.
