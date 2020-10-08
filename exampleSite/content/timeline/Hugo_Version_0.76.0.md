---
author:
  name: "John Doe"
date: 2020-10-07
linktitle: Hugo Version 0.76.0
type:
- post
- posts
title: Hugo Version 0.76.0
eventname: Hugo Release 
eventlocation: GitHub
weight: 10
---

## Abstract

In Hugo 0.76.0 you can now have a list of cascade blocks per page and a new _target keyword where you can select which pages to cascade upon using Glob patterns for a Page's Kind, Lang and/or Path:

```
title ="Blog"
[[cascade]]
background = "yosemite.jpg"
[cascade._target]
path="/blog/**"
lang="en"
kind="page"
[[cascade]]
background = "goldenbridge.jpg"
[cascade._target]
kind="section"
```
Tasks that were earlier hard/borderline impossible to do are now simple. One common example would to apply a different template set to nested sections; you can now apply a custom Type to these sections using path="/blog/*/**" and similar.

A related improvement is that the build option render is now an enum. In addition to turning on/off rendering of a given page you can tell Hugo to not render, but you want to preserve the .Permalink, useful for SPA applications.
 

[Link](https://github.com/gohugoio/hugo/releases/tag/v0.76.0) 