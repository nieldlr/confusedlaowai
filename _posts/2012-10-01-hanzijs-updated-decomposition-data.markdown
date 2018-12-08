---
layout: post
title: HanziJS gets updated. Now with more decomposition data!
date: '2012-10-01 09:13:21'
tags:
- chinese-character-decomposition
- chinese-radicals
- hanzijs
---

<a href="http://hanzijs.com">HanziJS</a> is a tool that I created earlier this year to help me find the components (radicals) of Chinese characters. It was rudimentary at best, but I've finally taken time off to update it a bit more. It is part open-source project, part tool. A picture below showing how decomposition looks like now.
<p style="text-align: center;"><a href="http://res.cloudinary.com/daxztt3th/image/upload/v1412837101/Screen-Shot-2012-10-01-at-9_35_06-AM_o2cpfe.png"><img class="aligncenter size-full wp-image-1287" title="HanziJS" src="http://res.cloudinary.com/daxztt3th/image/upload/v1412837101/Screen-Shot-2012-10-01-at-9_35_06-AM_o2cpfe.png" alt="" width="647" height="329" /></a></p>

<h2 style="text-align: left;">So what's new?</h2>
<p style="text-align: left;">- It now decomposes the character a lot further. There has been a LOT of background changes in terms of code (check <a href="https://github.com/nieldlr/Hanzi">the GitHub project</a> for more info).</p>
<p style="text-align: left;">- There are 3 levels of decomposition: Once, Radical &amp; Graphical respectively.</p>
<p style="text-align: left;"><strong>Once</strong> justs decompose it into the two most obvious radicals. This helps for checking out for dictionaries or learning Chinese characters, especially phono-semantic compounds.<strong> </strong></p>
<p style="text-align: left;"><strong>Radical</strong> decomposition decomposes the character into smallest possible "radical" components. This is based on the <a href="http://en.wikipedia.org/wiki/List_of_Kangxi_radicals">KangXi radical list</a>. This can also be a good way to remember how to write characters. Sometimes Level 1 &amp; 2 will show the same decomposition.</p>
<p style="text-align: left;"><strong>Graphical</strong> decomposition takes this a step further and goes down to lowest components, which will often be strokes or the last meaningful pieces. This is not necessarily in the right stroke order. This level of decomposition is still experimental, but still interesting to look at nonetheless.</p>
<p style="text-align: left;">- Redesign. I changed the design a little bit. Nothing big.</p>
<p style="text-align: left;">- Getting rid of "blocks" or glyph errors. I found a way to fix this. You need to download <a href="http://fonts.jp/hanazono/">the correct font</a>! This will allow you to see all the small things, like strokes or uncommon pieces.</p>

<h2 style="text-align: left;">So where to next?</h2>
<p style="text-align: left;">- Add more information, like Pinyin &amp; Definitions. The backend has this functionality already, but needs to be adapted for display purposes.</p>
<p style="text-align: left;">- Sentence segmentation (multiple characters). Dissect more than once character.</p>
<p style="text-align: left;">- API. I can create an API for people who'd want to use this. If you're interested contact me. I'm not sure yet how to approach this yet, but willing to talk.</p>
<p style="text-align: left;">- Your awesome idea!?</p>
<p style="text-align: left;">Yes, I'm looking for more cool ideas on how to improve <a href="http://hanzijs.com">HanziJS</a>. Who you be willing to pay for extra cool features (like being able to compute the regularities as mentioned<a title="5 ways Chinese radicals are sub-consciously trolling you" href="http://confusedlaowai.com/2012/05/5-ways-chinese-radicals-sub-consciously-trolling/"> in this post</a>)? Lemme know either way. I'd love to hear your feedback! Comment forth!</p>
<p style="text-align: left;">P.S. - I just like to say thanks to Gavin Grover again for providing <a href="http://cjkdecomp.codeplex.com/">the awesome data</a> for the decompositions.</p>