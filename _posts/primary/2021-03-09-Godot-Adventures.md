---
layout: post
title: Godot Adventures
---

A journal of my journey building a 2D/2.5D game in Godot.

Summary: Godot is a 2D and 3D, cross-platform, free and open-source game engine released under the MIT license. My friends and I happened upon this engine one day and decided to build our own little game. The other two, Tanner and Gabe, immediately started and built up a pretty basic game/concept before I even started watching the tutorial, so I decided to work on the animation portions of the game.

*March 9th, 2021*

**Download, installation, and setup**

Today at work I watched the first couple videos of the [tutorial for Godot](https://www.youtube.com/playlist?list=PL9FzW-m48fn2SlrW0KoLT4n5egNdX-W9a). It introduced how the 2D world worked, how to set it up, and place objects and a player in the scene. It was a relatively easy process, taking less than half an hour to do altogether. I also coded in some basic movement for the player, so it can move in any direction. No animation of the player yet I'm afraid, as I will do that another day. Below is a screenshot of the scene and objects I have set up. Once I figure out how to do GIFs and record my screen I'll be putting that up - but for now a still image will have to do.

![GodotAdventures001](/images/GodotAdventures001.PNG)

*March 13th, 2021*

**Animation research**

After rewatching the animation tutorial videos, I decided to implement it and test it in our game. After creating a new branch in the repo, I created a new player class to test named TestPlayer. I used the tutorials example sprite and implemented the animation player. Before I implemented the animation tree, I realized after discussing with Tanner and Gabe that our game was currently a full 2D, top down game, and the tutorial was closer to a 2.5D game. This means that currently in our game the character models are only seen from the head down, as shown in the examples pictures below.

![GodotAdventures002](/images/GodotAdventures002.jpg)

So now the plan is for me to create some basic top down sprites to get some experience in creating custom sprites and animating them, then once we have decided what kind of characters we want, I can begin creating the sprite sheets for inevitable transition to 2.5D. So currently, I will be watching the rest of the Godot tutorial videos to understand the code in our game, then figure out how to make top down pixel art, then full sprite sheet pixel art.