---
layout: post
title: Introducing HanziCraft
date: '2013-01-11 05:22:58'
tags:
- chinese-character-decomposition
- chinese-character-dictionary
- chinese-radicals
- hanzicraft
- hanzijs
---

Today, I introduce <a href="http://hanzicraft.com">HanziCraft</a>. It's a project that I've been working on for some time now. It started with my thesis, where I needed to easily decompose Chinese characters for my research. I then found data and wrote a little decomposition tool for myself. This was called <a href="http://hanzijs.com">HanziJS</a>. However, as time went on I realized I wanted more than just decomposition data. Why not create a site that pushes the value of Chinese character dictionaries to a new level?
<p style="text-align: center;"><a href="http://confusedlaowai.com/2013/01/introducing-hanzicraft/screen-shot-2013-01-10-at-9-52-36-am/" rel="attachment wp-att-1434"><img class="aligncenter  wp-image-1434" alt="HanziCraft" src="http://res.cloudinary.com/daxztt3th/image/upload/v1412837067/Screen-Shot-2013-01-10-at-9_52_36-AM_bscgyr.png" width="557" height="171" /></a></p>
What I mean by this, is that when I want to look up a Chinese character to learn (especially for something like the <a title="Chinese Character Challenge – Level up!" href="http://confusedlaowai.com/2013/01/chinese-character-challenge-level-up/">Chinese character challenge</a>) I want as much information possible to help me learn that character, especially regarding how some <a title="5 ways Chinese radicals are sub-consciously trolling you" href="http://confusedlaowai.com/2012/05/5-ways-chinese-radicals-sub-consciously-trolling/">radicals affect your reading on a sub-conscious level</a>.

Questions that come up:
<ul>
	<li>What are the radicals?</li>
	<li>How does the decomposition traverse itself?</li>
	<li>Is there any phonetic information available?</li>
	<li>Does this character have many definitions? How is it pronounced?</li>
	<li>Now that I know more of the character, where does it fit into vocabulary?</li>
	<li>Is the vocabulary useful?</li>
</ul>
Those questions are the ones that I want answered when it comes to a Chinese character dictionary. I have found some sites that can serve such a goal, but they are either badly designed, don't have all the answers and/or is in Chinese only.
<h2>What will become of HanziJS?</h2>
<a href="http://hanzijs.com">HanziJS</a> is the code behind <a href="http://hanzicraft.com">HanziCraft</a>. It is an <a href="http://github.com/nieldlr/hanzi">open-source module</a> for Node.js. This is the backbone. HanziCraft is thus an application of the code itself (hopefully other people will create their own apps with the HanziJS code in the future!).

If you are a coder, go check out the <a href="http://github.com/nieldlr/hanzi">github repo</a>. There's quite a lot of updates to it, as well as quite a bit of refactoring (thanks <a href="https://plus.google.com/114101734864850163495/posts">Dusan</a>!). I'm busy writing proper documentation for it.
<h2>Introducing HanziCraft</h2>
I think the best you can do, is to just visit the site and see for yourself. Check the info for the character <a href="http://hanzicraft.com/character/魔">魔</a> for instance:
<p style="text-align: center;"><a href="http://confusedlaowai.com/2013/01/introducing-hanzicraft/screen-shot-2013-01-11-at-11-16-13-am/" rel="attachment wp-att-1442"><img class="aligncenter  wp-image-1442" alt="魔" src="http://res.cloudinary.com/daxztt3th/image/upload/v1412837065/Screen-Shot-2013-01-11-at-11_16_13-AM_lelsqh.png" width="580" height="335" /></a></p>
Delicious juicy info!

If you want to know how I determine the example words, find the question in the <a href="http://hanzicraft.com/about">FAQ</a>.

<strong>P.S. - If you see any question marks or blocks, then you need to install the proper font to display all the components. Download the font <a href="http://hanzicraft.com/about#font" target="_blank">here</a>.</strong>
<h2>Beta</h2>
HanziCraft is now in it's beta phase. There will be bugs! But with this beta phase, you'll get a discounted <a href="http://hanzicraft.com/buy">premium account</a>. What do you get with a premium account? (Besides my eternal gratitude)
<ul>
	<li>Lookup more than one character at a time</li>
	<li>Favorite lists</li>
	<li>Your own user dashboard (currently showing your lookup history. I will implement character analytics in the future)</li>
	<li>No ads</li>
	<li>All future premium features forever free.</li>
	<li>AND Less hassle in learning Chinese characters (and who doesn't want that!?)</li>
</ul>
<h2>Future Features</h2>
I've got quite a bit more features planned for HanziCraft. Some premium &amp; some free. Here's what to expect:
<ul>
	<li>Display potential phonetic information in the radicals</li>
	<li>Display similar characters based on components (if a character shares more than 50% similar components)</li>
	<li>Text Analysis (this will be a premium feature that will take a group of characters, perhaps an article and compute what you need to know from the text. This will include unique characters, unique radicals, frequency counts and other cool information)</li>
</ul>
With all this being said, I think <a href="http://hanzicraft.com">HanziCraft</a> is a <strong>tool that I created for myself, mainly because I had trouble finding all the useful information I needed</strong>. I was eager, like a crazy addict, trying to find the information I craved, and after countless hours <a href="http://hanzicraft.com">HanziCraft</a> was born.

I hope HanziCraft becomes your goto Chinese character dictionary. I'm building it to be my own goto dictionary, so tell me, what do you need to make it the ultimate Chinese character dictionary? I'll try my best to implement the features you need. Happy learning!