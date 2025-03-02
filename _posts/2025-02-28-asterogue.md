---
title: ASTEROGUE, and How I Won The Game Jam
description: Game jams are fun--and this was my first!
author: kylie
date: 2025-03-01 21:50:00 -0600
categories: [self promotion, games]
tags: [shameless self promotion, asterogue, indie games, interactive]
image: 
  path: /assets/img/posts/ASTEROGUEtitlecard.png
---

<script src="https://cdn.jsdelivr.net/gh/ncase/nutshell/nutshell.js"></script>
<script>
Nutshell.setOptions({
    startOnLoad: true, // Start Nutshell on load? (default: true)
    lang: 'en', // Language (default: 'en', which is English)
    dontEmbedHeadings: true, // If 'true', removes the "embed this as a nutshell" option on headings
});
</script><!-- enables Nutshell by Nicky Case -->

> This article uses Nutshells by Nicky Case. If you see 
> [:underlined text like this](#x-nutshell-guide), tap it for some extra information!
{: .prompt-info }



## Prelude
As a kid, like most, I loved playing games. Board games, video games, imaginary games with friends. I even made a couple: I remember a Monopoly knock-off crafted from cardboard and Legos, and a card game (strikingly similar to Magic the Gathering, now that I think about it) played with friends in lunch periods. But in the fifth grade, I was introduced to a magical new outlet for my creativity: Scratch.

[:Scratch](https://en.wikipedia.org/wiki/Scratch_(programming_language)) is an online, block-based programming language made to teach kids how to code. As a kid who drew Mario levels on graph paper, this was a gold mine to me! I learned basic logic and platforming scripts, and learned the rest by looking through other users' projects and video tutorials. Through my years in school, I continually experimented in the environment, posting over a hundred projects in total. Some of those did very well in the proto-social-media environment, too: my most famous project was a [recreation of Celeste](https://scratch.mit.edu/projects/601239856/), with nearly 40,000 pageviews.

About last year, I found an open-source extension of Scratch called Turbowarp. Turbowarp removes limits set in the original browser-based system, and it's what I used to create Asterogue.


## The Game Jam

Earlier this month, a club at my university called ACM Game Dev had a miniature arcade cabinet set out during a club-promotion event. Intrigued, I joined the club, learning that they had a [:game jam](#whats-a-game-jam) fast approaching. So, as you could probably guess, I joined the club!

This specific game jam was of the theme "Breakups", and lasted one week. The winning game is then ported to the full-size arcade machine in the Computer Science building, for any and all to play.


## The Idea

The idea I had for the theme was a classic: Asteroids. In Asteroids, you fly around in a spaceship and shoot the namesake obstacles to break them up into smaller namesake obstacles. But, with my eyes on the prize, I wanted to make it as replayable as possible, if it were to win the jam and be arcade-ified. How do you add replayability? Turn it into a roguelike game, with random upgrades granted as you progress.

To add more depth to the gameplay, I added a dash that allows the player ship to move through asteroids without being damaged (similar to Undertale Yellow), and different weapons.


## Early development and demos

> Note: all demos run in 30fps instead of 60fps, for some arcane reason. The final build of Asterogue doesn't suffer from this issue; only the web demos.
{: .prompt-warning }

I wasn't working from a blank slate: I had an old demo from years ago I decided to freshen up and turn into a legitimate game. This project was made from a tutorial, with my own embellishments. Here's what it looked like:

### keyboard lemonoids.sb3
<iframe src="https://scratch.mit.edu/projects/620124691/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" allowfullscreen></iframe>
(Controls: WASD and all arrow keys; numbers 1-4 to switch weapons) 

The WASD keys are used to move the ship, left and right arrows are used to turn, up arrow to shoot, and down arrow to dash. In these demos, different weapons can be accessed by pressing the number keys.

### asterogue 0,0,1.sb3
<iframe src="/blog/assets/scratch/asterogue001.html" width="640" height="408" allowtransparency="true" frameborder="0" scrolling="no" allowfullscreen></iframe>
(Controls: WASD and all arrow keys; numbers 1-4 to switch weapons) 

After some style updates, this is what the first draft of Asterogue looked like. I had added a pixelizing filter, screenshake, and particle effects--all of which I hadn't implemented in a game before but now could thanks to Turbowarp's features.

### asterogue 0,0,4.sb3
<iframe src="/blog/assets/scratch/asterogue004.html" width="640" height="408" allowtransparency="true" frameborder="0" scrolling="no" allowfullscreen></iframe>
(Controls: WASD and all arrow keys; numbers 1-7 to switch weapons)

By the weekend, I had implemented more weapons, a simple [:HUD](https://en.wikipedia.org/wiki/HUD_(video_games)), and a player health system. In addition, gems will now explode out of asteroids as they're damaged and destroyed. I wanted destroying asteroids to feel satisfying; this is a good way to do that.

### asterogue 0,0,7.sb3
<iframe src="/blog/assets/scratch/asterogue 0,0,7.html" width="640" height="408" allowtransparency="true" frameborder="0" scrolling="no" allowfullscreen></iframe>
(Controls: WASD and all arrow keys; numbers 1-7 to switch weapons; T to spawn asteroid)

Skipping ahead a few more versions: a title sequence has been added, as well as the full HUD! I spent an entire night working out how I wanted the HUD to look, as it needs to convey information at a glance: I settled with large, colored bars that you can catch at the edges of your focus.

## Finishing up

From the last demo, it's just a hop, skip, and a jump to implement the weapon pickups, menus, and level progression systems. When I found time, I'd work in an upgrade or two from my list--small but satisfying problems to solve. I found fitting music online that I could use with credit, and from there Asterogue was complete. I submitted with a few hours to spare, and waited anxiously for the voting period to complete.

15 upgrades, 7 weapons, and 7 different color palettes traded for a whole week's worth of free time. I was really nervous...

But... I won it! I Won the Game Jam!! :D

![Desktop View](/assets/img/posts/ASTEROGUEtrophy1.png){: width="380" }{: .normal }
![Desktop View](/assets/img/posts/ASTEROGUEtrophy2.png){: width="380" }{: .normal }

The organizers even made a little trophy for the winner--it stays on my desk now.

## Arcade Version

The satisfaction I felt at winning was put off-kilter as I knew there were things to improve. I had to port the game to the arcade machine, and I took that opportunity to fix those small issues: calibrating controls, flipping and moving around the HUD to fit the vertical cabinet, adding upgrade descriptions, and tuning up weak weapons were all on the docket. I backported these changes into the horizontal version, and I'm happy with the result. If and when I release that version to the public, I'll be sure to add it here.

You can download the original jam version here:

<iframe frameborder="0" src="https://itch.io/embed/3324217?linkback=true&amp;border_width=0&amp;bg_color=000000&amp;fg_color=ffffff&amp;link_color=ff0000&amp;border_color=ffffff" width="510" height="165"><a href="https://goombasinastack.itch.io/asterogue">Asterogue by goombasinastack</a></iframe>


<br> <br>
> *Am I machine?* <br>
> *Are my feelings just programmed inside me?* <br>
> *Are destinies binary?* <br>
> *Are we just copies of copies of copies?* <br>
> *What am I feeling?* <br>
> *Am I really feeling anything?* <br>
> *Reminding myself that I am breathing* <br>
>
> Hey, ILY - Machine?

<BR>
<BR>
## Nutshells
[:What's a nutshell?](#-nutshell-guide)

### :x Nutshell guide
  Nutshells are snapshots of sections from other pages, or other parts of the same page. You can use them in your own sites: visit [here](https://ncase.me/nutshell/)!

  Self-referential nutshells congregate at the bottom of the page, much like footnotes--except you don't need to scroll all the way back up, since they're embedded in the text. Score!

  (The table of contents preview breaks a bit, though.)

### : What's a game jam?
  A game jam is a competition to create video games. Teams or individual developers will have a set amount of time to come up with, develop, test, and publish a game. 

  It's pretty hard.
