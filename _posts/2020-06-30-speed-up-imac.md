---
layout: post
title:  "How I dramatically sped up my 2017 iMac"
date:   2020-06-30
excerpt: "How I managed to turn my almost unusably slow iMac into the high-performance machine it was meant to be.
Spoiler alert: It had nothing to do with how many Chrome tabs I had open!"
image: "/media/cover photos/imac-speed-up.png"

categories: [How-To]
---

## My 2017 iMac was dreadfully slow - Right out of the box.
It was my first Apple purchase. I hadn't intended to drop $1400+ on a desktop, but the sleek metallic design caught my eye one day while wandering my local Best Buy showroom floor.

<span class="image right"><img src="/media/mac beachball.png"></span>
The "honeymoon phase" with my new desktop lasted about a week. That's how long it took me to load all of my data and software onto it and begin picking up on subtle hints that this machine was struggling. Loading Microsoft Office or my favorite graphics editing software, GIMP, was painfully slow. Sometimes upwards of 5 minutes would go by while I sat in front of the gorgeous "retina" screen, just watching the dreaded beachball rotate.

I sometimes wonder how many hours of my life I've wasted just waiting on this computer to perform whatever simple task I was asking of it to do? Not a day went by when I didn't curse the day I ever bought an Apple product.

I had suspected something was wrong. On multiple separate occasions, I lugged this heavy computer (in its original packaging) to a genius bar to have a professional diagnose any problems. After about the 4th trip in 2019, an exasperated genius bar employee told me what I had suspected all along. "Sir, the particular specs of this iMac were not intended for your use case. I suggest you upgrade to a new iMac with a better processor." So there you have it, my iMac was basically obsolete to me the day I came home with it just 2 short years ago. And as for my "use case," I mostly used this computer for basic word processing and email. It's not like I was pushing the envelope here.

So I resigned myself to continued use of what became known as my "apple" snail, all the while lamenting to my Apple-loving friends about the terrible, no good, awful purchase I had made. Many suggested I had a lemon on my hands, although none had the same model year as me.

Fast-forward a few months and the engineer in me couldn't let it go. I examined every component of this computer, thinking to myself that if I could just find the largest performance bottleneck and solve that then I would at least experience some sort of performance gain, maybe a big enough boost to reduce the amount of time I spent contemplating my life's decisions while waiting for my Gmail account to load.

### So what did I find?
This iMac is equipped with the following drive. Using a free software called "Disk Speed Test" I was able to quantify just how bad the performance of this drive really is.

<span class="image left"><img src="/media/DiskSpeedTest.png"></span>
<pre>
Capacity:	1 TB (1,000,204,886,016 bytes)
Model:	APPLE HDD HTS541010A9E632               
Revision:	JA0AB5N0
Serial Number:	JD8002D82LRWJD
Native Command Queuing:	Yes
Queue Depth:	32
Removable Media:	No
Detachable Drive:	No
BSD Name:	disk0
Rotational Rate:	5400
Medium Type:	Rotational
</pre>


I did quite a bit of research and formulated the hypothesis that this drive's slow rotational rate of 5400 rpm might just be the bottleneck I was looking for (for reference, most drives are between 5400-7200 rpm). To test this out I had two options:
1. Purchase and install a new internal drive, or
2. Purchase an external drive and connect it via Firewire or USB.

Since I prefer to take the most cost-effective approach in any situation, I went with option 2. More specifically, I went with an external SSD (solid-state drive) that is connected via USB 3.1. The benefits of an SSD are obvious, and since I wasn't sure this would work I went with the USB connection so I could at least use the drive with my aging Windows laptop.

Using my mac's recovery software, I cloned my internal drive to the external SSD and set the machine to boot from it.

### Results
<span class="image right"><img src="/media/DiskSpeedTest3.png"></span>
492% INCREASE!

That's how much faster the R/W speeds are using this external drive as my primary boot media. And boy does it make a difference! Check out the final speed test and compare it to the image above.

For a mere $90 and a few hours of my time I now have a working computer that should (hopefully) last me several more years.

As a side note: Why Apple put such a low-speed drive in this mac model is beyond me. For $1400 I would've expected much better.
