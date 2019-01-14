---
title: "More Indieweb"
date: 2019-01-11T21:58:57+01:00
author: "Jens-Christian Fischer"
description: "A few links to more IndieWeb related content and an outlook to FaaS"
image: ""
categories: ["musings"]
tags: ["indieweb"]
language: en
slug:
type: post
---

I wrote about the [Intro to Indieweb](/2019/01/intro-to-indieweb/) yesterday. Reading up on it, starting to
read the people behind it or using it, I feel a similar rush as I did back in the days when I started blogging.
This is the evolution of the Web I remember, this feels right. (And it also feels like a tiny bubble in the 
huge silo dominated web-simulacron we have around us today). Time to beat the drum, I guess and start on working
on making it more accessible for people that aren't as technology savy as the early adopters.

Watching Jeremys video yesterday, I got the idea to write something that would allow me to upload images and 
have them posted to the website. This is a bit of a problem, as this site is a collection of static HTML that 
lives in a Git repository and gets rebuilt whenever I push. I researched the [Github API](https://developer.github.com/v3/repos/contents/#create-a-file) 
and found a way how I might be able to create a commit programmatically. Then I thought that I should be able
to use a serverless approach, using some sort of [FaaS](https://en.wikipedia.org/wiki/Function_as_a_service)
technology. In my day job, I build [SWITCHengines](https://switch.ch/engines), a IaaS cloud. Since a couple of 
months, we are betaing [OpenShift](https://www.openshift.com/) and I saw a presentation on [OpenFaaS](https://www.openfaas.com/) at [GotoCPH](https://gotocph.com/). Turns out, that there is an old way to install it on OpenShift,
but RedHat is favouring [OpenWhisk](https://openwhisk.apache.org/). I managed to install OpenWhisk in a couple
of minutes (Yay), and then found out, that [Netlify](https://netlify.com), where this site is hosted, also supports
[Lambda Functions](https://www.netlify.com/docs/functions/). It probably is more sensible to use that service
than to rolling my own. (Ed: Why not try both?).

Further research led me to the website of [Vincent Pickering](https://vincentp.me/) and specifically his article on [Implementing the Indieweb on a static website](https://vincentp.me/articles/2018/11/14/20-00) - exactly my use case. He uses a JS server, [Master Cntrl](https://github.com/vipickering/mastr-cntrl) that runs on Heroku that handles all the dynamic aspects of Indieweb. A more recent post of his, [Adding a Media Endpoint](https://vincentp.me/articles/2018/12/17/12-00/)
not only describes what I wanted to do, but also [provides code](https://github.com/vipickering/mastr-cntrl/blob/master/app/routes/post/media.js). I will try to see, if something like this
could be ported to the Lambda Functions - either on Netlify or on OpenWhisk.

Finally, via Vincent, I found the [IndieWeb Directory](https://indieweb-directory.glitch.me/), a website that looks
charmingly 90s, and also added myself to it.

There is work to be done, hopefully it will result in some [code](/categories/code) soon.
