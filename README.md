<h1 align="center">dis-troll.js</h1>
<p align="center">
<img src="https://data.jsdelivr.com/v1/package/gh/kammt/dis-troll.js/badge"> 
<img src="https://auchenberg.github.io/volkswagen/volkswargen_ci.svg?v=1" alt="Volkswagen Build Status">  
<img src="https://github.com/kammt/dis-troll.js/actions/workflows/main.yml/badge.svg">  
<p align="center"> A JS script that starts to play discord ping/call sounds after site inactivity </p>
</p>

## I love my website visitors: So how do I add this on my website?
Easy peasy! 
1. Add the script to your site:
   ```html
   <script src="https://cdn.jsdelivr.net/gh/kammt/dis-troll.js/dis-troll.js"></script>
   ```
2. Wait for happy customer reviews

Any click or scroll by the user will reset a timer ranging from 4 and 10 minutes (the exact time is chosen at random).
When the user stops interacting with the site, the timer will eventually run out, and discord sounds will start to haunt them.

## I don't like the autosetup, can I do it manually?
Sure! Do the following:
1. Add the script, with autosetup disabled:
   ```html
   <script src="https://cdn.jsdelivr.net/gh/kammt/dis-troll.js/dis-troll.js" data-autosetup="false"></script>
   ```
2. Every time you want to trigger the timer, call the `startDistrollTimer` function
3. Wait for happy customer reviews

## But wait, my browser blocks auto-playing content
Well, if you interacted with the website, then playing content is allowed (e.g. playing a video by pressing the play-button). As the "sound-playing" is a direct result of a website interaction (with a delay), it is not blocked by default. 

This was tested on Firefox and Brave. If you find incompatibilities, feel free to report them!

## What can I customise?
- `data-min-minutes` - the minimum time that elapses until a timer runs out
- `data-max-minutes` - well.. the maximum time that elapses until a timer runs out
- `data-autosetup` - whether to run the autosetup or not

## Used by
- The MemeAssembly documentation (https://memeassembly.wtf/)
- The Artemgus Generator by xarantolus (https://artemgus.010.one/)
- ..you? If you use this script on your site, let me know and I'll add you to this wall of fame!

## A quick word about the security of your website
When you use dis-troll.js, you trust me that this script does not do anything malicious.
This is something you can verify from the source code.

However, since it is possible to update the script, I could sneak in anything I want, which would then be executed on the computer of every visitor of your website.
I will not do malicious updates, but you can't truly trust me (and any publisher of auto-updating software) on that.


If you want to be 100% sure and without needing to trust 
me, you have two options:
1. Download the current version of the script and embed this file into your website
2. Pin a specific version using jsdelivr, e.g.
   ```html
   <script src="https://cdn.jsdelivr.net/gh/kammt/dis-troll.js@v1.0.1/dis-troll.js"></script>
   ```
