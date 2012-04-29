---
layout: post
title: "Filtering resources in SBT projects"
description: ""
category: scala
tags: [sbt, xsbt, scala, plugins]
---
{% include JB/setup %}

I've just open-sourced a simple plugin for [SBT](https://github.com/harrah/xsbt), [xsbt-filter](https://github.com/sdb/xsbt-filter), which you can use for filtering your project's resources. The plugin's functionality is similar to Maven&rsquo;s [resource filtering](http://maven.apache.org/plugins/maven-resources-plugin/examples/filter.html) mechanism.

This plugin scans your resources (e.g `src/main/resources`, `src/test/resources`) for variables (surrounded by `${` and `}`) and replaces them with values which can come from the system properties, your project properties and filter resources.

The plug-in comes with sensible defaults, but there are lots of configuration options. Here's a sample configuration:

{% highlight scala %}
import FilterKeys._

seq(filterSettings: _*)

filterDirectoryName := "my-filters"

includeFilter in filters := AllPassFilter -- HiddenFileFilter

includeFilter in filterResources ~= { f => f || ("*.props" | "*.conf") }

extraProps += "author" -> "Foo Bar"

projectProps ~= { _ map (p => ("project." + p._1, p._2)) }
{% endhighlight %}

Check out the [README](https://github.com/sdb/xsbt-filter/blob/master/README.md) for more information.

Enjoy!