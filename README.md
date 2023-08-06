<h1 align="center">dis-troll.js</h1>
<p align="center">
<img src="https://data.jsdelivr.com/v1/package/gh/kammt/dis-troll.js/badge"> 
<img src="https://auchenberg.github.io/volkswagen/volkswargen_ci.svg?v=1" alt="Volkswagen Build Status">  
<img src="https://github.com/kammt/dis-troll.js/actions/workflows/main.yml/badge.svg">  
</p>
A JS script that starts to play discord ping/call sounds after site inactivity

## I love my website visitors: So how do add this on my website?
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

## What can I customise?
- `data-min-minutes` - the minimum time that elapses until a timer runs out
- `data-max-minutes` - well.. the maximum time that elapses until a timer runs out
- `data-autosetup` - whether to run the autosetup or not
