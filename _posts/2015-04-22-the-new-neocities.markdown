---
layout: post
title:  "Introducing the New Neocities"
date:   2015-04-22 12:00:00 -0600
categories: blog
---
[Neocities](https://neocities.org) is [almost two years old](https://neocities.org/blog/making-the-web-fun-again), and we're thriving. Initially launched as a quick summer project, we now have **43,500** websites, and we're growing fast.

Along the way, we've made decisions that have allowed us to handle growth while staying on a shoestring budget - solving problems with code rather than burn rate hijinks. We have stayed true to our principles of being [completely open source](https://github.com/neocities), having an [open work process](https://github.com/neocities/neocities/issues), and not shoving advertising into people's sites.

Leave your dancing baby GIFs, Ace Of Base MIDI files and <table> layouts on the backup drive. **We reincarnated free personal web sites for the modern web, and it's working.** Enabled by modern improvements to HTML/CSS/JS, it's never been easier to make [expressive](http://film.neocities.org), [informative](http://louisianawetlands.neocities.org), [helpful](http://mlpfim.neocities.org), [weird](http://hellosorrywrongnumber.neocities.org), and [artistic](http://fauux.neocities.org) web sites that stand the test of time.

We're continuing to work hard to make Neocities even better. Today I'm excited to formally announce the launch of the new Neocities, and show off some of the great new features and capabilities of the site.

### A Fast, Powerful Code Editor

![](/assets/front-editor-screenshot.png)

We put a lot of work into upgrading and improving our code editor, which is based on the amazing [Ace Editor](http://ace.c9.io/#nav=about). The editor is now more integrated, and has support for syntax highlighting, color themes, tag autocompletion, auto indenting, code folding, syntax error detection, and hotkeys (ctrl+s saves your work).

Now on Neocities, you don't even need an HTML editor installed on your computer to make an awesome web site. And we're working on even more enhancements (such as providing a file list panel to quickly access other files from the editor). Try it out, let us know what you think. I'm using it to write this, and I love it, it works great.

### Neocities Site Surfing (Web Rings)

A lot of people asked for us to bring back [Web rings](http://en.wikipedia.org/wiki/Webring). So we did! Except instead of implementing it in an [anachronistic](http://dictionary.reference.com/browse/anachronism) way, we've updated the idea for the modern web.

Neocities now has a Surf Mode, bringing the best of web rings and the modern web together. Our surf top bar quickly allows people to browse sites on Neocities, follow them, and share those sites with others. We've implemented it in a way that will work without compromising security (the frame loads pages from a different domain, which combined with our CSRF protections prevents cross-domain attacks). You can try it out by visiting the [Gallery](https://neocities.org/browse) and clicking on a site screenshot.

We used site tags to allow forming communities of related sites quickly and easily. No special embed code needed, just add a tag to your site, and you're done.

We're working on even more features here, such as curated lists of sites created by users on Neocities, so look for that coming soon. Surf's up!

### Richer, more powerful site browsing

![](/assets/front-browse-screenshot.png)

Being able to quickly browse sites on Neocities is important to us, so we made it easy to quickly find sites you like.

We updated our [website gallery](https://neocities.org/browse) to be cleaner, faster, and have higher quality screenshots. And because we now support site tagging, looking up sites by topic is fast and easy.

### Site Profiles and Activity Feeds

![](/assets/activityfeed.png)

Every site on Neocities now has a site profile, which allows you to follow other sites, see which sites like you, and comment on your site page. We deliberately tried to strike a balance between the [Guestbooks](http://en.wikipedia.org/wiki/Guestbook) of the old internet, and the modern social networks people are accustomed to. The result is a way to communicate that doesn't require embedding code in your site. This prevents "site rot" by reducing dependencies on external services that tend to break or go away.

We also keep track of when sites are updated, and combine all this activity together to create an **Activity Feed**, allowing you to see updates, follows and comments being done by sites you are following. This is a great way to find new sites that your friends sites are interested in, and helps to show all the activity going on at Neocities. There's also a [Global Activity Feed](https://neocities.org/activity) that shows what's going on with the most popular sites on Neocities.

We're quickly making some big improvements here, including a graphical upgrade to our Activity Feed design that will make it look a lot nicer and show more relevant content. It's already looking pretty good, but we'll be adding many improvements to make it even better.

### More Space

Continuing our policy of slowly providing more space as we figure out how to scale sustainably and affordably, **we've increased our free site space to 100MB.** Enjoy!

### Last, but not least: Subdirectory support

When we first launched Neocities, there wasn't support for subdirectories. It took a lot of nasty code refactoring, but we got it to work. This makes it a lot easier to organize your site, and provides support for more static site generator tools. We'll be adding some interesting features for subdirectories in the future (such as RSS feeds for specific subdirectories).

### What's next?

Victoria and I are now working full-time on Neocities at our new office in Portland, Oregon. We're scheduled to add [a lot of new functionality](https://github.com/neocities/neocities/issues) over the next year, so the answer to this question could be it's own blog post. But to highlight a few things:

**Neocities for Educators**. A lot of teachers have been using Neocities to teach HTML to students. We think this is important, so we want to help them by providing special Neocities features for educators. We are also working on developing an integrated tutorial for those learning how to program HTML for the first time.

We believe that everyone should have the opportunity to learn HTML as a way to obtain technical literacy. It's also the perfect first step to learning how to design and code software - one of the few careers that keeps growing fast in our information society.

**Increased space.** We've already increased our free web space 10x since we started. As we work to improve our scale-out strategy, we will be continuing to raise the amount of space we provide for both free and supporter sites. We can't take the easy way out, because services like Amazon S3 are too costly for us to be able to use them, so we've had to think outside of the box and come up with our own solutions. We now think we know how to do this, and we'll be slowly pushing out our infrastructure changes over the year. These changes will also have the benefit of providing us with more mirrors of sites, increasing load time performance for everyone.

### Come see Neocities' first talk!

Today (Weds April 22), we're doing our first ever Neocities talk at [Fluent](http://fluentconf.com) in San Francisco. Stop by Salon 10 at 1:30PM and hear the story of Neocities and our quest to bring back free personal web sites and save the Internet from boring text-box social networks. After, Juan Benet with [IPFS](http://ipfs.io) will be doing a talk on the Permanent Web. Juan is awesome, and we're doing some really cool stuff with his code (more info on that coming soon). Don't miss it!

### Donations Welcome

Right now we're 2/3 of the way to breaking even on our hosting bills. It's decent progress, but we're going to need to increase our income much more to continue working on Neocities full-time, so that's our most important milestone. Our goal is to increase revenue to $50,000 by the end of this year, and I'll be honest, it's going to be tough. The easy route in the web/social space is to start embedding advertising, **but we're never going to force unwanted advertising on sites hosted on Neocities, ever**. So we need your help to sustain the site.

[Donations are very welcome right now](https://neocities.org/donate). I hope showing what we've been capable of with such a meager budget demonstrates that we'll put donations to good use. We also provide a [Supporter Plan](https://neocities.org/plan) that helps sustain the site for everyone.

### Thanks for believing in us

Bringing back the lost art of creating personal web sites makes the internet a better, funner place, and fills a missing hole in the modern web. Thanks for helping us succeed in this effort. We can't wait to see all the awesome things you create.

We hope you enjoy the new Neocities as much as we do.
