---
title: "Posting from iOS"
date: 2019-01-04T12:46:00+01:00
author: "Jens-Christian Fischer"
image: "/img/writing.jpg"
categories: ["code"]
tags: ["tech", "blog", "iOS"]
language: en
slug:
type: post
---

Having a git based blog makes it slightly 
difficult to post while on the go. 
I have read at least [two](#) [accounts](https://schnuddelhuddel.de/switching-from-wordpress-to-hugo/)  of people who pulled that off, but neither workflow quite worked for me.

Here's where I'm at:

* use [WorkingCopy](https://workingcopyapp.com) to clone this sites [jcfischer/invisible_ch](https://github.com/jcfischer/invisible_ch) repository 
* use a Siri shortcut to [convert urls to markdown links](/files/Create%20Markdown%20Link.shortcut)
* use a Siri shortcut to [export images from Photos to WorkingCopy](/files/Copy%20Foto%20To%20Working%20Copy.shortcut)
  by saving it through the Files app in the repository that WorkingCopy hosts
* Using [iA Writer](https://ia.net/writer) to edit files that are stored in A git repository (add WorkingCopy as a file provider in iA Writer)

{{< figure src="/images/working-copy.png" title="working in Working Copy" >}}

Things I tried that didn't work: 

* using [Git2Go](https://git2go.com/) - app not available on Swiss AppStore. Update: Actually the app is no longer 
  on the AppStore at all, [said the developer](https://twitter.com/pietbrauer/status/1081158855608946688)
* using [Editorial for iOS](https://omz-software.com/editorial/) to edit posts. Looks nice, but crashes when trying to open a file from WorkingCopy (also not adapted to iPhone X screen)

Will update this post as I learn more. 
