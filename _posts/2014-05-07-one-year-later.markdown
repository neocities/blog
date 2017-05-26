---
layout: post
title:  "Neocities, one year later"
date:   2014-05-07 12:00:00 -0600
categories: blog
---
It's been almost a year since we launched [Neocities](https://neocities.org). We haven't done a blog update in a while, and I wanted to give a status update on some of the improvements and features we've added recently. My bad blogging prowess aside (I tend to focus on giant, epic blog posts rather than simple ones that convey frequent changes) **Neocities is still going strong**, and we've been working hard on the site.

Initially worrying the site would be a fad and only last a few months (or become a cesspool of phishing sites), Neocities has turned into a strong and vibrant community for people building amazing stuff. At the time of this post, we now have over <strike>19,300</strike> 19,500 websites on Neocities, ranging from [the delicious](http://mitz.neocities.org) to the [artistic](http://solvallagata-braedraborgarstigur-cinema.neocities.org), and the [immensely creative](http://fauux.neocities.org/consciousness.html). I could add a lot of awesome Neocities sites I love, but I would run out of adjectives. This isn't 1995 Geocities junk - there are thousands of really impressive sites on Neocities.

There are also a lot of teachers using Neocities in classes to teach HTML, because aside from being easy to set up, it provides an important feature that learning HTML on a local computer doesn't - the ability to share your web site you made with the entire world. That's what makes the web interesting, and that's what makes it exciting for people to learn HTML. And because HTML is an excellent branch for learning JavaScript, you have a great way to get people started in programming, with something that they can enjoy the results of immediately.

So yes, Neocities is very much alive and well. We've been making small changes throughout the year, like improving our site screenshot code, fixing bugs, adding little new features here and there, but nothing huge.

As a result of the strong continued interest in the site, and some careful planning we've been doing over the last year, we have recently started a major new push to continue building out the site to provide a much better experience, make it easier for users to work with their sites, and start working on a way to sustain the site indefinitely, without resorting to dumping ads on people's sites or removing the free site option - something that we said we would never do, and we meant it.

### Double the free space

First, news that every Neocities site will love: We've raised the Neocities free space to 20MB, from it's original 10MB limit. Now that we know the amount of space people use and how we can start scaling things in a sustainable way, we can start raising the limits. This is just the beginning. Long term, we want to raise the amount of space a lot more. I can't give concrete numbers yet, suffice to say that we're talking about numbers that are just as easily measured in gigabytes as megabytes. But before we do that, we have some non-space improvements we need to make first. Bear with us while we continue to build up the infrastructure to facilitate this. It's not easy to scale these things (affordably and sustainably), but I'm confident we'll get it done.

### A New Dashboard

![](/assets/newdashboard.jpg)

Our initial site manager worked, but it wasn't great. The interface was clunky, and difficult to work with. There wasn't a way to easily see your content, and the way the content was arranged didn't scale well for sites with a lot of files. It worked, but it wasn't very good.

Our new dashboard (designed by [Victoria Wang](https://twitter.com/violasong)) is a great improvement. Now you can see a thumbnail for all the images and HTML files on your site. Uploading files is now as simple as dragging files from your computer's file manager to the dashboard, where it is automatically uploaded (and there's a progress indicator). It's cleaner, it's easier to work with, it's just better. Try it out!

### Cleaned up design

Not really a huge news-worthy announcement, but we cleaned up the site design a lot, and it looks a lot nicer now. For every major news announcement about a crazy new feature at a startup, there's an unmentioned hero that works on the little things that make the experience better. Here's to you, unsung hero.

### Improved site screenshots

We've updated the screenshot renderer. Our first implementation had some issues with rendering certain sites, and had fringe issues with things like Japanese fonts. We've corrected this, and now site rendering should be much more faithful to the look of the actual site. A lot of credit goes to improvements to PhantomJS and a recently released screencap gem for ruby that has much better screenshot code than we were using before.

### Neocities Supporter Program

We received a lot of requests for a way to contribute to the site, so we have introduced a [Neocities Supporter](https://neocities.org/plan) program. Being a Supporter is an (optional) way to help us sustain Neocities in a long-term, recurring way. It's basically a pay-what-you-want plan, but it starts at $1/mo (billed at $12/year, because credit card fees suck). In addition to helping maintain the site, as our way of saying thanks, supporters will receive 200MB of space for their site (and we'll be raising that amount a lot soon). You can cancel at any time, and if you do, you can keep the space.

We also accept Bitcoin, Dogecoin and PayPal through our [donation](https://neocities.org/donate) page, and will happily upgrade your account for you manually if you contact us.

To those that have already upgraded, thanks! To those that haven't, please consider. A little goes a long way to the site, and it helps us to improve the site and ensure that things keep running.

### More great improvements to come

Currently, we get about 1,000 new sites every month, a growth rate that has been rising quickly. Neocities users are fun, smart, creative, and friendly. We love them a lot, and want to continue to improve their experience. We're working on a major new version of the site that we hope to release within the next month or two, that will make it easy to follow, donate, and comment on sites, and create a community of sites based on tags (our solution to the "web ring" requests). We won't need to inject code into Neocities sites to do any of it. It's a big change, and we're really excited about it. We'll have a lot more information about this coming shortly, suffice to say that nobody has ever done what we're about to do, and I'm expecting it to re-define what it means to make a web site.

Neocities' goal is to make the web fun again. To bring back the notion that you should be able to control your web presence on the internet, instead of filling details about your life into pre-defined boxes. To bring back the notion of web surfing, of sharing our dreams and creations with eachother, in the way that each of us wants to, manifested in the greatest knowledge distribution system we have ever come up with: the web. Stay tuned for further updates, and thank you for continuing to make the web fun again.

What are you waiting for? [Go make your web site!](https://neocities.org/new)

-- Kyle
