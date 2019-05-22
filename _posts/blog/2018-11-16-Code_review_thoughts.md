---
layout: post
title: "To be a pushover or a nitpicker, It's a question."
author: me
excerpt: "What’s happening with engineering code reviews?"
categories: blog
tags: [Tech, PM]
modified:
image:
  feature: mushroom.jpg
  <!-- credit: WeGraphics -->
  <!-- creditlink: https://wegraphics.net/downloads/free-ultimate-blurred-background-pack/ -->
share: true
comments: true
---


Recently my team is getting to be a hot potato around in the eng department since a lot of customer features/issues raised up to leadership during our SAFe Planning Conference. The solely purpose to have a team here is for better customer/developer experience. Is that super cool? It’s just my thing to get insights from frontier with real users.Nothing change too much in my daily routine except being hustler around more often. But I noticed a subtle interesting process, which is our code review. This post is aiming to share some helpful thoughts from multiple hats, like developer’s mind and product owner’s mind.(assume I’m in his shoes.)
 
![Bless Code review](https://memegenerator.net/img/instances/37612347/im-chuck-norris-i-approve-of-this-code-review.jpg)

Definitely not the best practice on my team, but what’s the root cause for non-effective way and why we cannot get rid of it earlier on, and most importantly --- how can we do it better in the future?

I try to summarized into a few aspects we might need to highlight and to face it honestly as a whole development team.
 
##### A bit political stings can emerge even worse.
Probably this is the worst part in a harmony of engineering life, but it does happen…kind of easy in real life example. I mean no one is originally trying to bully a junior by intimidating him/her to do A or B,  or to show off how fancy Streaming in Java 9 or how solid Promise in ES6 to save all legacy callback hell. But once this loop starts rolling on the road, it hardly has an immediate stop without coming back and forth. And in my experience, It’s such a waste to get distracted from getting more important things done, how about we just even have a beer then have a kickback in the cafe area? I really want, sometimes.

##### Security review is often-undervalued and bite us back
We always take pride a lot as owning “Security is a first” as engineering creed here. We can’t just follow behind Transunion, not even need to mention tech giant — Facebook.(Sorry, my friend in FB lol…you’re not on the third-party API team though.) When it comes to code review, however, developers are inclined to have a mindset like a gang of hackers inadvertently crack things down and fix it up in the build pipeline, and even feeling awesome which is a classical false impression for software engineer, especially  not-well-seasoned ones. but we need to be tougher on sausage-baking process in case of owning security compliance  (we do have our internal security guideline for engineering teams). Self-defending code is always good even it’s not in very lean and smart way.

##### Lower documentation coverage is what triggers confusion
Reduce more explicit question in the comments and drag a big conversation frequently. Especially a huge benefit for new hire (or one is not much involved with a certain product’s recent feature, but is a member of PR’s approval list), In my opinion, good coder could have been writing down the clear technical specs such as architecture design doc/key defects report and etc, based upon our code style guidance.

There are several basic ideas came out of my mind and I think it’s noteworthy following it at least myself:
1. Focus on the code itself but ignore who wrote the code.
2. Raise kind question without sarcastic/joke attitude to make a suggestion.
3. Keep conversation as lean as possible but also informational. (Make this meaningful...)
4. Implement Code Lint tools (We are considering SonarQube integrated into Gitlab pipeline after 2 weeks I wrote this post. Yah!)
5. Encourage team members to get some data or insights through the code review and expand transparency, which could possibly reduce process shit in the long run.
 
From PO’s point of view, It’s likely getting highly subjective things to evaluate the incentives that development team deliver. Are we still great software engineers if we ship the sloppy hacky code when we don’t have too much runway? or we are just sticking around the standards by writing beautiful code given loads of time.
![bless code review](https://jameelnabbo.com/wp-content/uploads/2018/05/1_nxXw5ViikNF2tIzIs21qlw-1000x559.png)

There are tons of solid materials could be a gold guide, I mean generally for code reviews in most cases. But I am not going to draft a email with a long list of hyperlinks then spread to the team. (I know it doesn’t always work even if you do a funny engineering survey or questionnaire.) I want to figure out why and really talk to key team members and discuss a viable approach for us.
