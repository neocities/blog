---
layout: post
title: "Cleaner links for web pages"
date:   2022-12-30 00:00:00 -0600
categories: blog
---

Today we're rolling out a pretty big change to Neocities: cleaner links, by automatically loading the __.html__ files without the extension.

So for example if you have a __/my-favorite-songs.html__, you can now load it with your browser by just typing __/my-favorite-songs__. Previously you could do this by creating a directory called "my-favorite-songs" and then adding an index.html to it (__my-favorite-songs/index.html__), but this will make that step optional. Every link to a web page with the __.html__ on the end will still (and always) work, and will automatically redirect to the cleaner URL, so there shouldn't be any issues with search engines or links breaking.

The main drawback to this is that it may affect local site editing. But if you edit your site locally and the cleaner links don't work with your local server, you can still use __.html__ in your links and they will redirect automatically on Neocities. You should also still use __.html__ for the actual files when you create them on Neocities.

For the edge case where there is both a directory index and a root page, such as __/my-favorite-songs.html__ and __/my-favorite-songs/index.html__, the slash will be used to denote the directory, so __/my-favorite-songs__ and __/my-favorite-songs/__ will load each respective page.

This change also makes it slighty harder to move to other static web site hosting, but it's easy to configure other servers to support this. If you run your own server and use [nginx](http://nginx.org/) for this, this is the code you can use to make it work the same way (in the server {} section of your config):

```
if ($request_uri ~ ^(.*/)index$) {
  return 301 $1$is_args$args;
}

if ($request_uri ~ ^/(.*/)index\.html?) {
  return 301 /$1$is_args$args;
}

if ($request_uri ~ ^/(.*)\.html?) {
  return 302 /$1$is_args$args;
}
```

Enjoy the cleaner, easier to type in web page links! Happy New Year!