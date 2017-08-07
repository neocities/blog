---
layout: post
title: "IPFS DNS Support"
date:   2017-08-07 00:00:00 -0600
categories: blog
---

I've never been shy about our support for the [distributed web](https://blog.neocities.org/blog/2015/09/08/its-time-for-the-distributed-web.html). As the flaws of today's web continue to lead to increased centralization, and with Net Neutrality being gutted, the stakes for a good future for the web have never been more clear to me. That's why we were one of the first organizations to start doing implementation work with [IPFS](https://ipfs.io), which I continue to believe is the next version of the web, and the logical successor to HTTP.

Continuing down this adoption path, **I'm happy to announce that Neocities now has support for IPFS DNS records!** That means that most of the 140,000+ sites that have a neocities.org subdomain can now be accessed through IPFS via DNS.

You can see it in action at [https://ipfs.io/ipns/testipfs.neocities.org](https://ipfs.io/ipns/testipfs.neocities.org), or if you have [IPFS installed](https://ipfs.io/docs/install/), you can view it locally at [http://127.0.0.1:8080/ipns/testipfs.neocities.org](http://127.0.0.1:8080/ipns/testipfs.neocities.org).

This works by using TXT records with our DNS servers. You can run<br><code>dig TXT testipfs.neocities.org</code> in a command prompt to see it in action:

<pre><code>dnslink=/ipfs/QmdJtiWqGEDsUJqW41aTQcds7U2PzmLDWs8qQ346mNoPkF</code></pre>

Right now we're only supporting IPFS immutable hashes (not IPNS/keypair ones), which means there is a short delay before DNS records update with site changes through IPFS, but we'll reduce this time lag soon. In the interim, this gives our IPFS implementation its first taste of mutability.

The distributed web is still in the foundation stages, and things are constantly changing. We'll keep testing new things and see how we can help improve the distributed web. Enjoy!
