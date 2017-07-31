# Parro

A technical interviewing platform capable of asking both behavioral and technical questions and analyzing a candidate's performance intelligently.

## Table of Contents

- [Project Overview](#project-overview)
- [Demo](#demo)
- [Contributing](#contributing)

## Project Overview

This was an idea that resulted from a number of pivots before we ultimately zeroed in on exactly the problem we wanted
to solve: a technical interview process that's automated from start to finish. We've even added support for a Q&A session at the end of the interview, where candidates can ask Parro about the company for which they're inteerviewing and receive answers. There are platforms that handle the technical side like HackerRank, Codility, and others, but none of them provide support for automating the behavioral side of the hiring process, which really matters to certain startups and companies. That's what Parro was built to do.

**Technical**


**Behavioral**


**Q&A**

## Demo

Let's say I'm the project lead on a team, and I want to reward my coworkers for workind hard the past couple weeks with a Friday afternoon pizza party. I can make the Dominator application listen to me from anywhere inside my Slack channel by typing an order, which it will interpret and ask me for information that I did not provide. It is possible to provide more than just order information when I invoke the bot -- I could also give it my phone number, email, and home address if I wanted to knock it out in one fell swoop. We've illustrated the step-by-step process here for clarity.

![alt text](https://github.com/benhubsch/SlackPizza/blob/master/pics/slack.png "In Slack")

Note a couple of things: for starters, I say I want a pepperoni pizza. The api.ai entity picks keywords out of my request -- most likely "pepperoni" and "pizza" -- and runs those keywords through an algorithm that matches to Dominos menu items behind the scenes. In this instance, it matched my request for pepperoni pizza with Dominos' Ultimate Pepperoni pizza. Not bad! The application was also able to pick my phone number and email out of otherwise perfectly normal English sentences. Lastly, I gave it a really poorly formatted address, and the application was able to churn out a gorgeous, nicely formatted address that will ultimately be passed on to Dominos (1412 Market san fran was converted to 1412 Market St., San Francisco, CA 94102).

I am then forwarded to a link that contains a page where I can enter my credit card information. Slack does not support sending forms through direct messages, nor would it be ideal to put credit card info in-line as a regular message, so the most secure option is to link to an external form:
![alt text](https://github.com/benhubsch/SlackPizza/blob/master/pics/payment.png "Payment Details")
Each of the fields that I fill out are validated to ensure that they are non-empty and contain the correct type. The UI automatically changes color and autofills your credit card company if it is a common provider.

Lastly, the most enjoyable step: my order is complete! I can see how much I spent, and how long I can expect to wait until Dominos is able to deliver to my apartment.
![alt text](https://github.com/benhubsch/SlackPizza/blob/master/pics/final.png "Order confirmation")

If you have any doubts as to whether this actually works, it does! I suppose you'll have to take my word for it. Unless, of course, your stomach starts to grumble, and you can't help but be a little bit curious if the code we wrote actually runs, and you fork it and place an order.

## Contributing

Interested in contributing to this project? Feel free! Create a branch, add commits, and [open a pull request](https://github.com/benhubsch/File-Finder/compare/).