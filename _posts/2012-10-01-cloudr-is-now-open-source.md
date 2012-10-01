---
layout: post
title: "Cloudr is now Open Source"
description: "Cloudr, an unofficial CloudApp client application for the Android platform is now Open Source."
category: 
tags: [sbt, android, scala]
---
{% include JB/setup %}

I recently open sourced Cloudr, an unofficial [CloudApp](http://getcloudapp.com) client application for the Android platform. The CloudApp service allows you to share images, links, music, videos and files.

The Cloudr client applciation currently has the following functionality:

* share images, videos and other files from a file manager, the Gallery, ...
* share bookmarks
* navigate and browse your drops collection
* delete and restore drops

Cloudr might be of interest to other Android developers for the following reasons:

* mostly written in [Scala](http://www.scala-lang.org)
* built with [sbt](https://github.com/harrah/xsbt) with the help of the [android-plugin](https://github.com/jberkel/android-plugin), an sbt plugin for Android projects
* uses [RoboGuice](http://code.google.com/p/roboguice/) and [RoboSpecs](https://github.com/jbrechtel/robospecs) for unit tests

The [source code](https://github.com/sdb/cloudr) is on GitHub.

By the way, The appplication is [available for free](https://play.google.com/store/apps/details?id=be.ellefant.cloudr) from the Google Play store.