---
layout: post
title: "File moving/renaming, faster web sites"
date:   2019-03-06 00:00:00 -0600
categories: blog
---

Just a quick update on some recent small improvements for Neocities we're thrilled to roll out!

## Support for file moving / renaming

For a long time if you wanted to change the path or name of a file on Neocities, you had to re-upload it. This was inconvenient for a lot of people, so it has been our most requested feature.

The reason this was lacking was because most upstream file storage providers don't support renaming, only copying files. For sites with a lot of large files, this would have been difficult to implement and taken a lot of time for simple operations to complete.

We have put together a solution for file storage that prevents this problem from happening, allowing for file renaming and moving without having to do a full copy. So there is now support for file/directory renaming and moving, which you can do directly from the dashboard. The interface doesn't yet support drag and drop, but we'll be looking at implementing that soon.

## Faster loading web sites: TLS 1.3, Brotli

We recently rolled out some upgrades to how we serve Neocities web sites that will improve both performance and security. [TLS 1.3](https://www.ssl.com/article/tls-1-3-is-here-to-stay/) reduces the "handshake" time of establishing connections, improving the speed of initial connection by up to 100ms in some edge cases. We also turned on [Brotli compression](https://medium.com/oyotech/how-brotli-compression-gave-us-37-latency-improvement-14d41e50fee4) support, which reduces the size of the data that needs to be transferred to web browsers by using better compression algorithms. This helps web sites load faster, particularly on lower bandwidth connections such as mobile phones.

Enjoy!
