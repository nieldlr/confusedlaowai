---
layout: post
title: Phonetic Sets in Chinese Characters
date: '2013-03-12 07:03:02'
tags:
- chinese-radicals
- hanzicraft
- hanzijs
- phonetic-sets
---

You might have noticed that a few weeks ago I added a feature to <a href="http://hanzicraft.com" target="_blank">HanziCraft</a> that automatically tries to find pronunciation clues in each character. Using this tool, I decided to create phonetic sets using the 6800 most frequent Chinese characters.
<p style="text-align: center;"><a href="http://res.cloudinary.com/daxztt3th/image/upload/v1412837063/Screen-Shot-2013-03-12-at-12_54_18-PM_auaptr.png"><img class="aligncenter  wp-image-1478" alt="Phonetic Sets" src="http://res.cloudinary.com/daxztt3th/image/upload/v1412837063/Screen-Shot-2013-03-12-at-12_54_18-PM_auaptr.png" width="506" height="334" /></a></p>

<h2>What is a phonetic set?</h2>
I quote from <a href="http://hanzicraft.com/lists/phonetic-sets" target="_blank">HanziCraft</a>
<blockquote>A phonetic set is a list of characters where a component produces the same pronunciation clue towards each character.

For instance, the component 马, which is pronounced as 'ma3', can be found in these characters: 吗,玛,码,蚂,犸. They all have the same pronunciation 'ma3'.</blockquote>
I decided to generate two lists. One where components have the exact same pronunciation as the character, and two, where the component has the same syllable but differs on tone.

You can see both lists <a href="http://hanzicraft.com/lists/phonetic-sets" target="_blank">here</a>.
<h2>Interesting Findings?</h2>
令(ling2) is awesome! Just look at this list of all the characters that have the exact same pronunciation:
<blockquote>零,玲,铃,鈴,龄,齡,伶,翎,聆,羚,苓,蛉,呤,泠,囹,瓴,鸰,鴒,舲</blockquote>
And this one where it includes all the characters with 令, but with different tones.
<blockquote>领,領,零,玲,铃,鈴,龄,齡,岭,伶,翎,聆,羚,苓,蛉,呤,泠,囹,瓴,鸰,鴒,舲</blockquote>
You'll see some characters overlap, because some characters have multiple pronunciations.
<h2>Combinality</h2>
As I mention on the page, combinality is still another variable to consider when you look at these lists. How trustworthy is a component in providing those clues to the character?

Read my post on <a title="5 ways Chinese radicals are sub-consciously trolling you" href="http://confusedlaowai.com/2012/05/5-ways-chinese-radicals-sub-consciously-trolling/">sub-conscious variables in Chinese characters</a> for more info. This is a variable that HanziCraft is working on trying to find. It's not that hard, but just needs some more coding.