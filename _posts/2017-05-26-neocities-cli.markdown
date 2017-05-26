---
layout: post
title: "Introducing the Neocities CLI"
date:   2017-05-26 00:00:00 -0600
categories: blog
---

We're proud to announce the <a href="https://neocities.org/cli">Neocities CLI</a>, a command line tool for power users that want to quickly make changes to their site from their shell terminal.

Some of it's many features include:

* **Easy to use** - simple design, informative help screens for each subcommand.
* **Push support** - uploads an entire directory. Great for static site generators.
* **HTTP persistence** - the CLI reuses a single HTTP connection, improving performance.
* **Check before upload** - checks if the file data matches before uploading.
* **Gitignore parsing** - automatically skips files in root gitignore file for git repositories.

## Try it out

If you're running OSX or already have Ruby installed, run this command:

    gem install neocities

If you get a "permission denied" error, you may have to run the command as root:

    sudo gem install neocities

After installation, you can run it by executing the `neocities` command, which will display a help screen with a list of subcommands.

If you don't have ruby (or aren't using OSX), [click here](https://www.ruby-lang.org/en/documentation/installation/) to see your options for installing Ruby for your platform.

As with most of our source code, the Neocities CLI is open source and available for review (and pull requests) on [our github repository](https://github.com/neocities/neocities-ruby). Have fun!
