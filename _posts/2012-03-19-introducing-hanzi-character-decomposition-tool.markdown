---
layout: post
title: Introducing Hanzi - A Character Decomposition Tool
date: '2012-03-19 15:53:30'
tags:
- character-decomposition
- chinese-radicals
- mandarin-radicals
---

I've been a bit busy lately. Doing lots of coding. One of my personal projects this weekend (which will eventually be used in my research) was to create a Chinese character decomposition tool. I've always had this problem. I was never sure how to decompose Chinese characters into their radical components. I set out to solve this problem. Say 你好 to <a href="http://hanzijs.com">Hanzi</a>.

[caption id="attachment_870" align="aligncenter" width="517" caption="Example of decomposing the character 赶"]<a href="http://res.cloudinary.com/daxztt3th/image/upload/v1412837340/Screen-Shot-2012-03-19-at-3_29_29-PM_brqitk.png"><img class="size-full wp-image-870" title="Hanzi" src="http://res.cloudinary.com/daxztt3th/image/upload/v1412837340/Screen-Shot-2012-03-19-at-3_29_29-PM_brqitk.png" alt="" width="517" height="225" /></a>[/caption]

To avoid being overly technical:
<blockquote> Hanzi is a Chinese character dictionary lookup (still in development) and radical decomposition module for Node.js.</blockquote>
It was created using the Node.js coding language. This is for the coders and language learners as I think this could benefit many people out there. It is still very early in its development cycle. So it has a few limitations:

1) Can only lookup one character at a time.

2) Only breaks down the character into two parts.

3) Some characters break down into REALLY weird glyphs, which can't be shown by the average browser.

4) Some character decompositions show numbers instead of their components. This is how the data is structured. It will be solved soon. This is especially apparent in more complex characters and 繁体字 (traditional characters).

5) The decompositions aren't all radicals. They are "parts" rather than radicals. Well most of it. I will set out to show all the radicals eventually.

6) When decomposing a radical it displays an "undefined" next to it. Will remove it in the next update.

But, hey it's a start in the right direction. So try it out at <a href="http://HanziJS.com">HanziJS.com</a>. I still have lots of development to do on this module, but it works good enough already to help you guys out. For more a technical post <a href="http://niel.delarouviere.com/2012/03/introducing-hanzi/">head to my personal blog.</a>