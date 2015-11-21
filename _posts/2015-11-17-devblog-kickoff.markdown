---
layout: post
title: "Engine2D Devblog Kickoff"
date: 2015-11-17 19:35:4
categories: javascript,engine2d
---

Over the course of the past couple of weeks I've been doing a lot of work on my [Engine2D](https://github.com/jackdalton/engine2d) game engine. Everything had been going pretty well.

I was quite satisfied with how easy it is to write extensions, like a [time delta extension](https://github.com/jackdalton/engine2d/blob/master/extensions/engine2d.deltatime.js), or a [sound player extension](https://github.com/jackdalton/engine2d/blob/master/extensions/engine2d.sound.js).

When I started work on this, I had planned to just make the bare minimum, not forcing the user to use canvas rendering, or WebGL. I figured people could write their own extensions, and just share them with others.

But, I've run in to a bit of a problem: **How can extensions be aware of each other**?

After some consideration, I've realized that an extension which would add a new object type would need to be recognized by, for example, another object type extension.

If both extensions registered as `Engine2D.TYPE.TRIANGLE`, we'd have a bit of a problem.

This issue has really derailed Engine2D's extension development.

I had a sprite extension in the works, but until I sort this out it's not getting anywhere.