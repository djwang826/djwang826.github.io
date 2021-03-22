---
layout: post
title: Godot Devlog
---

A journal of my journey building a 2D/2.5D game in Godot.

Summary: Godot is a 2D and 3D, cross-platform, free and open-source game engine released under the MIT license. My friends and I happened upon this engine one day and decided to build our own little game. The other two, Tanner and Gabe, immediately started and built up a pretty basic game/concept before I even started watching the tutorial, so I decided to work on the animation portions of the game.

*March 9th, 2021*

**Devlog #1: Download, installation, and setup**

Today at work I watched the first couple videos of the [tutorial for Godot](https://www.youtube.com/playlist?list=PL9FzW-m48fn2SlrW0KoLT4n5egNdX-W9a). It introduced how the 2D world worked, how to set it up, and place objects and a player in the scene. It was a relatively easy process, taking less than half an hour to do altogether. I also coded in some basic movement for the player, so it can move in any direction. No animation of the player yet I'm afraid, as I will do that another day. Below is a screenshot of the scene and objects I have set up. Once I figure out how to do GIFs and record my screen I'll be putting that up - but for now a still image will have to do.

![GodotAdventures001](/images/GodotAdventures001.PNG)

*March 13th, 2021*

**Devlog #2: Animation research**

After rewatching the animation tutorial videos, I decided to implement it and test it in our game. After creating a new branch in the repo, I created a new player class to test named TestPlayer. I used the tutorials example sprite and implemented the animation player. Before I implemented the animation tree, I realized after discussing with Tanner and Gabe that our game was currently a full 2D, top down game, and the tutorial was closer to a 2.5D game. This means that currently in our game the character models are only seen from the head down, as shown in the examples pictures below.

![GodotAdventures002](/images/GodotAdventures002.jpg)

So now the plan is for me to create some basic top down sprites to get some experience in creating custom sprites and animating them, then once we have decided what kind of characters we want, I can begin creating the sprite sheets for inevitable transition to 2.5D. So currently, I will be watching the rest of the Godot tutorial videos to understand the code in our game, then figure out how to make top down pixel art, then full sprite sheet pixel art.

*March 17th, 2021*

**Devlog #3: More animation research/actual testing**

The plan changed again, and we decided to just go ahead to 2.5D immediately, but with basic sprites in only 2 directions (left/right) for testing/proof of concept. So I watched two beginner pixel art tutorials, one about the [overall process](https://www.youtube.com/watch?v=o_EKrg2fIuc), and the other about [character design](https://www.youtube.com/watch?v=vXm5VjZA4Ys). The overall tutorial talked about the basics, such as some pixel placement, color palettes, other pixel art tutorials, starting simple, and software to use. It gave an extremely concise and detailed [pixel art tutorial blog](https://blog.studiominiboss.com/pixelart), recommended [LoSpec Color Palettes](https://lospec.com/palette-list) for people who don't understand colors, and talked about Aseprite, Pyxel Edit, and Piskel for software. I ended up using Piskel for the character sprites as the app is simple to use and more importantly, free.  So I opened up Piskel and realized I didn't know the first thing about actual drawing/designing a character - which lead me to the second tutorial. It explained the process of character design, which was simplified to looking for references, drawing the silhouette, and finally filling the character with your style/details. This is how I ended up with my two new character sprites, the first a temporary main character sprite, and the other the temporary generic enemy sprite.

![GodotAdventures003](/images/GodotAdventures003.png)

I used knight pixel art as my reference for this. Also, the characters have no arms as we decided that it would be easier to not include arms and have attack animations separate, as this would cut down on a lot of animation time.

![GodotAdventures004](/images/GodotAdventures004.png)

I used bandit pixel art as my reference for this. Also, I used the Fruity-26 color palette for these characters.

Next update will hopefully have the sprites animated and some tiles made.

*March 19th, 2021*

**Devlog #4: Tile sets, more planning**

I created a general rock wall tile set using Piskel to create the general base and then used the [Tilesetter program](https://www.tilesetter.org/) to generate the actual tile set. At first the sides were too thick, which made the tiles look too 2D when the character sprites stood next to it. This was fixed by thinning the tile on the sides and making the wall a more uniform color. Below is a comparison of the first version compared to the (more) finalized version.

![GodotAdventures005](/images/GodotAdventures005.png)

![GodotAdventures006](/images/GodotAdventures006.png)

I then created a quick grass tile set, and if you don't look too closely, the grass looks pretty ok!

![GodotAdventures007](/images/GodotAdventures007.png)

*March 22nd, 2021*

**Devlog #5: Water tile set, sprite updates**

I created a water tile set, and now the plan is to recreate the character sprites at 24x24 px and compare to the 32x32 px sprites before starting animation. I'm also watching more Godot tutorials in order to help more with the coding.