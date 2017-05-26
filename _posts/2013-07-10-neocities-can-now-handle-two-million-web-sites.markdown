---
layout: post
title:  "Neocities can now handle two million web sites"
date:   2013-07-10 12:00:00 -0600
categories: blog
---
![]({{ site.url }}/assets/newdesign.jpg)

A few weeks ago, I put together a [blog post](http://neocities.org/blog/making-the-web-fun-again) describing my goals for NeoCities, and why I thought it was an important project. And [I asked for your help](https://neocities.org/about), because we needed the funding to get the servers to put the site on solid footing.

And wow, did you respond. Thanks to all the donations we received, we now have enough resources to run the site (at its current configuration) **for two million web sites, for up to two years!** Which is just in time, because NeoCities popularity is exploding: **We're at almost a million hits for the first two weeks.** On behalf of myself, the sites, and the people helping to build NeoCities, thank you very much. Your generous contributions mean that we'll be able to work to sustain the project for a long time, **and focus on building even better features and functionality**.

Your donations have already gone to good use. Last night, I migrated NeoCities off the crappy dedicated server I was using for a [weird unrelated project](http://bestofnhk.tv), and onto its own powerful, state-of-the-art server with plenty of room to grow. The move went seamlessly, and the site is now very stable and running smoothly.

I've also added SSL, so you can access all the sites with HTTPS ([like this one](https://suppilulemur.neocities.org)). Screw you NSA, figure out how to beat Sokoban on your own.

I also wanted to note quickly that the servers are now being run in Germany. This was more pragmatic (great offer from a good hosting company there) than political (the erosion of United States due process), but I would be lying to you if I said I wasn't breathing a little easier at night knowing that the server is now being hosted in a country that strongly believes in the rule of law, and [isn't just going to storm in like a bunch of uneducated thugs and trash the place, and put up an MS Paint of their ugly government logos](http://www.wired.com/threatlevel/2012/05/weak-evidence-seizure/).

As you can imagine, there is a lot more to do. I want to give you a highlight of some of the new features and functionality we are working on implementing right now.

### New NeoCities Site Design

I will admit, I'm a lousy web designer, so I grabbed a [themed bootstrap](http://bootswatch.com). But we need a real site design now. [Victoria Wang](https://twitter.com/violasong) came to the site's (and my) rescue: she designed [a beautiful front page](https://raw.github.com/kyledrake/neocities-web/master/files/wireframes/homepage03x.png) for the NeoCities site, that will make it look a real web site, and not just a hacked-together thing like it is right now. And [Scott O'Hara](https://twitter.com/scottohara) has been working on contributing to it and HTMLizing it. They both have contributed a lot of their time, effort and ideas to this project, and I can't possibly thank them enough (seriously, please help me thank them). I think this will help a lot with getting more people interested in making their own sites.

### More Space

**We will soon be raising the space size to 20 Megabytes**. I realize that this is still pretty small, but I want to be careful to ensure that we don't make a promise we can't deliver. It has been suggested that [the limitation may be a good thing](http://10mbmanifesto.neocities.org). My plan is to stick with 20MB for now. I will have a blog post to announce this when it happens, so stay tuned.

### Domain Names

`yourname.neocities.org` is pretty good, but there's nothing more powerful than owning your own domain. When you own your own domain, you are in control. I want to make it easy for people to add their domain name to NeoCities, and just as easy to move their content elsewhere if they decide they don't want to use us (or want to step to something more powerful like their own server).

I will be implementing domain support eventually. I'm not sure what the timeline on this is yet, it's a more difficult thing to implement, but I think it's important. So we're going to do it. Domains themselves cost money, but **we will not be charging for linking domains to NeoCities sites** because I feel that having your own identity that you control is important.

### Visual HTML Editing (and text editor improvements)

Though there is a focus on learning and understanding HTML here, I thought it would be neat to implement a visual HTML editor. This is a bit more difficult, because while there are a lot of WYSIWYG editors available for HTML, but most of them don't do layout, they are designed to be embedded in existing page layouts. I need to think about this more, but there is a [pull request](https://github.com/kyledrake/neocities-web/pull/15) in the repository for a visual editor and I will be taking a look at it soon.

I will also be looking at ways to improve the text editor, and possibly coming up with a better way for mobile users to edit their sites.

### More powerful interfaces for file uploading

The initial file upload interface is.. not so great. I'm going to be working to improve it. First with things like drag-and-drop file uploading, and then with an API to allow developers to write tools to upload files. I've also decided to remove the file type whitelisting, and instead switch to a blacklist that contains the names of common executables. There's just too many custom file formats to whitelist them all.

A few people have asked for FTP and GIT support, but we won't be implementing them. I like GIT, but if you want to make a static site with it, [there is already a great site for doing that](https://github.com). We are trying to solve a different problem. Also, FTP is anachronistic. Nobody uses it anymore and it's going to be very difficult for me to lock down the security on it.

### Better Browsing of Sites

Before launch, the site browsing was kindof an afterthought. You know, one of those afterthoughts that you eventually realize is the most important part of the site.

Right now it only really sorts by time last updated. I'm going to fix in a few ways. First, I'm going to put together a Hacker News style algorithm that creates a list from a combination of multiple metrics, such as time created, time updated, number of visits, and popularity (upvotes). Then I'm going to allow you to search based on criteria. I'm also going to make it so you can view the sites flagged as NSFW (sorry for the delay on this, and double thank you for not retaliating based on my slow response).

### Missing Bits and Pieces

There are some remaining unexciting bits and pieces that got lost in the noise. Things like being able to reset your password and change your e-mail address, which is a bigger problem than I realized. I will be fixing these shortly as well.

### Final Thoughts

If it takes me a while to finish some of this, I apologize. This is a side project for me (and the rest of us) right now, so I have to balance my time with my other work, namely my work on the [Coinpunk project](http://coinpunk.org). That work is awesome for a completely different set of reasons (When it's finished, it may be the most secure and efficient Bitcoin wallet service in the world, and definitely the best fully open-source one).

I'm pondering ways to generate recurring income for the site, just so that the site can be sustainable for a long time even if donations stop happening. One thing I have been pondering is having an affordable account for people that want a lot more space (100MB or more). Or just having a "tip" plan, similar to the way iPhone apps will have a free and a "$1.00 tip" version. If anyone has other ideas I could try here, let me know. I will be adding the above features before considering this, though.

What are you waiting for? **[Go make your web site!](http://neocities.org/new)**

-- [Kyle](https://kyledrake.net)
