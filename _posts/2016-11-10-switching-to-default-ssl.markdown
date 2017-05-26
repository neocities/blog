---
layout: post
title:  "We're switching to default SSL"
date:   2016-11-10 12:00:00 -0600
categories: blog
---
![]({{ site.url }}/assets/edsnowden.jpg)

**Starting January 1st, 2017, Neocities will be defaulting to SSL on all sites.** This could possibly lead to some sites breaking, so it's important that you read this if your site links to any third party content that's not on Neocities.

### Why are you doing this?

I'm not getting into specifics right now, suffice to say there's recently been a troubling rise in political extremism around the world. To protect your users, it's critical that we switch to default encryption and make it harder to violate your user's privacy.

In addition, search engines have recently said they will start penalizing unencrypted sites in search results, meaning that without default SSL, your site will be less likely to show up on search results. We obviously don't want that to happen, so that is another large motivator.

### What's going to break?

Basically, anything that embeds content (such as images and videos) from a third-party site using `http` instead of `https`. For example, if you have an embedded image with `<img src="http://example.com/image.png">` instead of `<img src="https://example.com/image.png">` (see the **s** in http?). The problem is that web browsers will block loading of `http` content because it is considered [Mixed Content](https://developer.mozilla.org/en-US/docs/Web/Security/Mixed_content). If your browser is expecting an HTTPS connection, it refuses to load any unencrypted HTTP content because it "leaks" the encryption.

The fix for this is to make sure your site does not have any embedded content that uses `http` instead of `https`. You can also strip out the protocol part of the link (http:) like this, and it will automatically assume HTTPS: `<img src="//example.com/image.png">`

### Is there any way to automatically fix this?

Most browsers will auto upgrade HTTP connections to HTTPS using a special [Upgrade Insecure Requests](https://www.w3.org/TR/upgrade-insecure-requests/) header we'll enable on our servers. This will take care of a lot of it for most users. However, if the third-party site does not provide HTTPS in addition to the unencrypted HTTP, it will still break. And unfortunately, there are still [some older browsers](https://developer.mozilla.org/en-US/docs/Web/Security/CSP/CSP_policy_directives#upgrade-insecure-requests) that don't yet have support for it. Sadly, this also includes the latest versions of Internet Explorer. That's why we've been waiting before doing this transistion. But given the political environment, I don't think we can afford to wait to make this change anymore.

### Will this include Custom Domains?

Yes. We're already using [Let's Encrypt](https://letsencrypt.org/) for all custom domains, and it should already be working. The only difference is that we will be defaulting to it for all incoming traffic.

### Why not just directly fix the code on the sites?

I've pondered this, but we've never made any changes to other people's HTML before, and I'm not comfortable changing that policy now. I feel like not modifying our user's sites is part of our trust model, and I'd really rather not go down that slippery slope.

I apologize in advance for any issues this may bring up. But I hope you understand why it's important to do this, even if there will be some temporary migration pains associated with it. Thanks for your understanding.

-- Kyle
