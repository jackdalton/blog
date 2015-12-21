---
layout: post
title: "Engine2D Is Deprecated"
date: 2015-12-21 10:15:17
categories: engine2d,javascript
---

I've recently realized that the way I initially wrote Engine2D is terrible (one big namespace? Really?)

So, I've made an alternative. Meet [E2D](https://github.com/jackdalton/e2d). Unline Engine2D, E2D is not contained in a single source file; rather, E2D is built by gulp, concatenating its many source files.

I started trying to fix my mistakes in [Engine2D's devel branch](https://github.com/jackdalton/engine2d/blob/devel/src/engine2d.js), but I knew it was too late. Besides, there are numerous problems with that branch's approach as well.

TL;DR: Engine2D sucks, [E2D](https://github.com/jackdalton/e2d) is better.