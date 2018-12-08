---
layout: post
title: I have a drinking problem
date: '2011-10-23 10:47:45'
tags:
- chinese-character-encoding
- drinking-in-chinese
- he-displaying-differently
- sinosphere
- unicode
- unihan
- variant-characters
---

Heyoooo. Gotta love sensationalist headlines right!? Don't worry this is not a hungover post or drunk blogging, but rather an interesting thing I noticed the other day. I was busy creating a website (which will be online tomorrow, so expect another blog post tomorrow or Tuesday) when I typed the character for drinking. You all know it. It is written as 喝.

However, something strange happened. The character was different. Now let me show you the bigger picture. Here is how the character came out as:

<a href="http://res.cloudinary.com/daxztt3th/image/upload/v1412837435/Screen-Shot-2011-10-23-at-10_18_53-AM_qmpfee.png"><img class="size-full wp-image-677 aligncenter" title="Drinking in Chinese" src="http://res.cloudinary.com/daxztt3th/image/upload/v1412837435/Screen-Shot-2011-10-23-at-10_18_53-AM_qmpfee.png" alt="" width="220" height="202" /></a>

Now, if you know your drinking, you would notice that, that character is not entirely right. It's different. Notice the 匕 radical underneath the 勹 radical. That is not normal. Then I went on a search, for I remembered the character was written differently. I consulted my Hanping Dictionary app on my phone and also checked the Oxford Chinese-English Dictionary on my desk. They both had the version I remember it as. However, now here comes the interesting part. I looked around for that version online. Why was my MacBook displaying it differently? I couldn't find a version online! Then it dawned on me. Maybe it's my browser, but it wasn't, because after copying the character into a simple text editor it still displays the same. Also, my popup dictionary (<a href="http://confusedlaowai.com/2010/04/google-chrome-translator-plugin-zhongwen/">Zhongwen for Chrome</a>, which uses CEDICT) still detected it as 喝. So in essence it was the SAME character.

My investigation went further. I looked up the Unicode for 喝 and found <a href="http://www.unicode.org/cgi-bin/GetUnihanData.pl?codepoint=%E5%96%9D">this in their Unihan database</a>.

<a href="http://res.cloudinary.com/daxztt3th/image/upload/v1412837434/Screen-Shot-2011-10-23-at-10_32_09-AM_mnau92.png"><img class="aligncenter size-full wp-image-679" title="Unicode for 喝" src="http://res.cloudinary.com/daxztt3th/image/upload/v1412837434/Screen-Shot-2011-10-23-at-10_32_09-AM_mnau92.png" alt="" width="425" height="115" /></a>

AHA! I knew I wasn't drunk or something! See there. The Unicode standard is how I remember it. From the dictionaries and during my Uni classes. However, it should be added that it isn't entirely my browser's fault. It is my whole computer. I tested this out and visited the same link on my Windows machine. It matched the Unicode standard.
<h3>Kanji not Hanzi!</h3>
At first I thought it was my browser or even my Pinyin IME, but now it must be my MacBook. It baffles that there is a difference! I'm not a big know-how on Chinese Character encoding, especially Unicode, but I doubt it would work this way. The thing is, it is the SAME character! My pop-up dictionary picks it up. I looked at my text-editor to see if has something to do with the fonts that my MacBook uses. I noticed the font was unfamiliar. It's called Hiragino Mincho. Yes, that's Japanese!

Usually the standard font for Chinese is the Song font. I never installed these fonts. They came with the MacBook. I decided to look up a bit more to see if the Kanji version looked different. Check this <a href="http://en.wiktionary.org/wiki/%E5%96%9D">Wiktionary for 喝</a>. It does! See there. It shows the different variants. I changed my font in the text editor and I got the Hanzi version back, by using the Song font. However, now there's my browser. The weird thing is, looking at the Wiktionary page, it shows both versions of the character. Now this is getting weird.

How can my browser show two versions of the same character? If they are technically the same Unicode!?
<h3>Variant Characters in Unicode</h3>
<p style="text-align: left;">After some more investigation. Yes, I need a drink by now! I found out that Unicode encoding has variants based on the language <a href="http://confusedlaowai.com/2011/09/defining-sinosphere/">in the Sinosphere</a>. Check this article out on Wikipedia, called <a href="http://en.wikipedia.org/wiki/Han_unification">Han Unification</a>. There's a table there that is supposed to show different variants of the same character, with the same Unicode, but different based on language. I checked my settings on my MacBook. I found out that it was giving priority to Kanji over Hanzi.</p>
<p style="text-align: left;">I finally see the correct 喝 now! However, for some reason I still can't get that table to show the different variants in the <a href="http://en.wikipedia.org/wiki/Han_unification">Han Unification</a> page. It only shows me the Hanzi version now. Oh well, that's a problem for another day. I think it might something to do with the type of font. For now I'm glad that I can see the old 喝 again.</p>
<p style="text-align: left;">---------------</p>
<p style="text-align: left;"><em>P.S. - Please visit that Han Unification link and tell me if you are seeing different characters or not in the examples of language dependent characters table!</em></p>