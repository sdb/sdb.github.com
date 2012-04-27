---
layout: post
title: "Copy bookmarks from Read It Later to Instapaper"
description: ""
category: 
tags: [readitlater, instapaper, script]
---
{% include JB/setup %}

I've just copied all of my -i'll read them later- bookmarks from the [Read It Later](http://readitlaterlist.com/) (RIL) service to [Instapaper](http://www.instapaper.com/) (IP) using their API's. For this I wrote a small Python script that fetches all my bookmarks from RIL and posts them to Instapaper.

The script takes 5 arguments: the RIL API key, username and password, and a username and password for Instapaper.

I've copied 219 bookmarks with this script. Note that it doesn't handle HTTP errors, so if anything goes wrong, you're screwed :P

Check out [this gist](https://gist.github.com/866772) for the complete script.