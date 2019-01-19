---
title: "Handling Responsive Images"
date: 2019-01-19T16:36:00+01:00
author: "Jens-Christian Fischer"
categories: ["code"]
tags: ["tech", "blog", "images"]
language: en
slug:
type: post
---

Displaying images responsively can be done with the `figure` shortcut:

{{< figure src="size-before.png" alt="Crystal Caves" caption="some nice caption">}}

This is based off of work by 
[Laura Kalbag](https://laurakalbag.com/processing-responsive-images-with-hugo/), 
[Adam Wills](https://www.adamwills.io/blog/responsive-images-hugo/) and
[Nils Norman Haukås](https://nilsnh.no/2018/06/10/hugo-how-to-add-support-for-responsive-images-trough-image-processing-and-page-bundles-3/) and
looking up [Responsive Images](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images)

The figure tag is able to look up both in the local page bundle (as shown in the 
picture above) as well as in the global asset directory (see below)

{{< figure src="/img/crystal_caves.jpg" alt="Crystal Caves" >}}
