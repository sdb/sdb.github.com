---
layout: post
title: "Giter8 template for Android apps"
description: ""
category: 
tags: [sbt, xsbt, android, scala, giter8]
---
{% include JB/setup %}

For those interested in developing an Android app with [Scala](http://www.scala-lang.org/) and the [simple build tool](http://www.scala-sbt.org/) (sbt), I just pushed a [giter8](https://github.com/n8han/giter8) template project to my GitHub account. You can find it [here](https://github.com/sdb/android-sbt-quick.g8).

What is giter8? It's a command line tool to generate files and directories from templates published on github.

My Android template (it's called android-sbt-quick) is similar to the [android-app](https://github.com/jberkel/android-app.g8) template, but with a couple of differences:

* your Android resources are in the root of the project to be compatible with the [ADT plug-in](http://developer.android.com/sdk/eclipse-adt.html) for Eclipse
* no separate `tests` project (yet) for Android integration tests
* [specs2](http://etorreborre.github.com/specs2/) support with [robospecs](https://github.com/jbrechtel/robospecs)

Checkout the [README](https://github.com/sdb/android-sbt-quick.g8/blob/master/README.md) for more information.

Please contact me if you have have any questions.