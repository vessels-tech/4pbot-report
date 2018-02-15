---
date: '2018-02-10T21:30:10+10:30'
published: true
title: What is 4Pbot?
weight: 3
---

_todo: include screenshots and transcripts_

4Pbot is a virtual assistant for Filipinos on the nation's social welfare program, Pantawid Pamilyang Pilipino Program, or 4Ps. 4PBot talks with clients of the 4Ps program over Facebook Messenger, and is available for free on Facebook Free Basics.

_or It serves as place where people can ask questions, report issues and receive advice privately and securely._

_TODO: make into table_

### Features:

_todo: expand on these points, give more background_

- Payment date estimates
  - We crowdsource paydays across the Philippines to give accurate estimates of when the next payday will occour.
- Anonymous reporting system
  - Clients can make complaints and report issues they are having with 4Ps. We try to help find a solution, while keeping their information secure and private.
- Payment calculator
  - Helps beneficaries to know how much they should be recieveing every 2 months, and helps them take action if they are being underpaid.
- 4Ps news
  - 4PBot knows what's going on in the community, with the latest news stories about 4Ps.

### Audience

Filipinos speak a multitude of different langauges, a challenge that we have had to embrace from the start. 4Pbot

- Langauges: Cebuano, Tagalog, English
- Clients (mostly women) who recieve 4Ps payments for their families

### Platform
- Facebook Messenger
- Facebook Free Data users

Why facebook?
  - good test bed, easy to build bots
  - over 20,000 benefiaries actively on facebook, in unofficial 4ps groups


## Technology
- Open source from the core
- uses Botkit, an open source bot development platform
  - ensures 4pbot is easily moved to new platforms (we're looking at SMS and IVR next)
- runs on Firebase functions, using NoSQL database (woo hoo)
- Uses Google Sheets along with Zapier to build some super agile features out quickly, and make data collected easily visible and infinetly shareable
