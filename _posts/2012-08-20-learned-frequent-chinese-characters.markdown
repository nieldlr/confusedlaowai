---
layout: post
title: What do you know if you learned the most frequent Chinese characters?
date: '2012-08-20 20:39:57'
tags:
- chinese-character-frequency
- chinese-characters
- chinese-corpus-linguistics
- chinese-vocabulary
---

I have developed an interest in Chinese characters and statistics recently. This interest comes from my research into Chinese orthography and spaced repetition systems for my Master's degree. For instance the effects of <a href="http://confusedlaowai.com/2012/05/5-ways-chinese-radicals-sub-consciously-trolling/">radicals on sub-conscious level on recall of Chinese characters.</a> One question popped into my head the other day on the ratio between Chinese character knowledge versus Chinese vocabulary knowledge.

As you might know, most Chinese words are formed with the combination of two characters. So, by obvious deduction, your character knowledge would produce more vocabulary knowledge. For instance, knowing the characters 饭，商 and 店, not only gives you three single character words, but also two more words: 饭店 and 商店.

Now, this beneficial relationship between character knowledge and vocabulary knowledge isn't always that apparent. We don't always learn all the words afforded by all the characters we know. We just don't have the time and resources to check up these relationships. It would also get very interesting once the character knowledge becomes more. It would essentially start getting exponential. Any new character to your knowledge of characters would then have the opportunity to form words with any of the previous ones.

Out of curiosity I decided to just play around with the most frequent Chinese characters and see what and how many words are created using them.
<h3 dir="ltr">How it was done</h3>
I used some code from <a href="http://hanzijs.com/">HanziJS</a> to do dictionary lookups using the open source <a href="http://www.mdbg.net/chindict/chindict.php?page=cc-cedict">CC-CEDICT</a> dictionary. I then used the <a href="http://lingua.mtsu.edu/chinese-computing/statistics/">character frequency list</a> from Junda as a source for the characters.

Using some terrible coding skills I then computed all possible two/three/four character combinations and used those to lookup in the dictionary if such words existed. I also counted the single characters as words themselves.

At first I only ran tests with up to max of 2 characters combinations. The lookups went quite quick. Then I increased it to three and four character combinations. It slowed down dramatically especially if you increase the amount of characters. I contemplated only looking at two character combinations, but then I might miss some opportunities for chengyu to appear.

So I decided to apply an assumption to reduce the amount lookups：

<strong>Assumption:</strong> Words with three repetitions of the same character next to each other are discarded. So for example: "得得得x" where 'x' is any other character from the list. I have not encountered words in my four and half years of Chinese study where characters repeat three times. The same can thus be said for 'x得得得'.

But that wasn't very efficient. It only removed a few hundred lookups for instance at the 25 character level.

Something needed to change. The CC-CEDICT has over 100,000 entries. I did not need to look at all the entries to see if there are possible word combinations. So I manually checked the file and created indexes for each character. For instance all dictionary entries starting with ’的' is very little. Only 11!

This reduced the lookup times by a major factor.

For the curious coders out there, I used Node.js. Also at the end of the post I've added a Google Doc link to all the words per category that was generated along with their meanings.
<p style="text-align: left;">I should also note, that the lookups only produce one dictionary entry. For instance, according to CC-CEDICT,<strong id="internal-source-marker_0.37326906085945666"> </strong>has two dictionary entries. I only chose to stop at one, because I want to equate character knowledge versus possible word combinations, not necessarily all the different meanings.</p>

<h3 dir="ltr">The Short Graph Version</h3>
[caption id="attachment_1178" align="aligncenter" width="614"]<img class=" wp-image-1178" title="wordchart" src="http://res.cloudinary.com/daxztt3th/image/upload/v1412837174/wordchart1_weou3e.png" alt="" width="614" height="356" /> Amount of characters by frequency and how many words they form.[/caption]

[caption id="attachment_1174" align="aligncenter" width="614"]<a href="http://res.cloudinary.com/daxztt3th/image/upload/v1412837175/charactertowordratio_tjrcg0.png"><img class=" wp-image-1174" title="charactertowordratio" src="http://res.cloudinary.com/daxztt3th/image/upload/v1412837175/charactertowordratio_tjrcg0.png" alt="" width="614" height="356" /></a> Character to word ratio[/caption]

[caption id="attachment_1180" align="aligncenter" width="614"]<a href="http://res.cloudinary.com/daxztt3th/image/upload/v1412837173/characterswords_srrhzs.png"><img class=" wp-image-1180" title="characterswords" src="http://res.cloudinary.com/daxztt3th/image/upload/v1412837173/characterswords_srrhzs.png" alt="" width="614" height="356" /></a> Amount of words per amount of characters in a word.[/caption]
<h3 dir="ltr">The Long In-Depth Version</h3>
<h3 dir="ltr">10 Characters</h3>
<blockquote>Characters: 的,一,是,不,了,在,人,有,我,他

Total Dictionary Lookups (with assumption): 11,010

Total Dictionary Entries Found: 25

Percentage of Entries Found: 0.23%

Ratio of characters to words: 1:2.5

Total Computing Time Before Index: &lt;1min

Total Computing Time After Index: &lt;1sec</blockquote>
I did not expect very interesting results from only 10 characters. Most of the first 10 characters are grammatical characters and pronouns. Some interesting words that came out were 不在了 (to be dead/to have passed away), 我人 (we) &amp; 他人 (another/sb else/other people). The latter two is the first time I've seen 人 used in the same way as 们. Quite cool.<strong><strong>
</strong></strong>
<h3 dir="ltr">25 Characters</h3>
<blockquote>Characters: 的,一,是,不,了,在,人,有,我,他,这,个,们,中,来,上,大,为,和,国,地,到,以,说,时

Total Dictionary Lookups (with assumption): 406,275

Total Dictionary Entries Found: 106

Percentage of Words Found: 0.026%

Ratio of characters to words: 1:4.24

Total Computing Time Before Index: 28min

Total Computing Time After Index: 8secs</blockquote>
Immediately the exponential nature is apparent. We gained a few more words with the increase from 10-25. So the additional 15 characters created 81 more words. The first four character dictionary entries arrived: 中国人大 (China's National People's Congress) &amp; 大有人在 (there are plenty such people). They aren't idioms yet though. <strong><strong>
</strong></strong>
<h3 dir="ltr">50 Characters</h3>
<blockquote>Characters: 的,一,是,不,了,在,人,有,我,他,这,个,们,中,来,上,大,为,和,国,地,到,以,说,时,要,就,出,会,可,也,你,对,生,能,而,子,那,得,于,着,下,自,之,年,过,发,后,作,里

Total Dictionary Lookups (with assumption): 6,375,050

Total Dictionary Entries Found: 326

Percentage of Words Found: 0.005%

Ratio of characters to words: 1:6.52

Total Computing Time Before Index: 7 hours

Total Computing Time After Index: 1min 30 secs</blockquote>
Ooh boy. The possible combinations is surely hitting massive proportions now. I did not expect 50 characters to take this long to compute. Luckily the second time around it went by a lot quicker.
<h3 dir="ltr">100 Characters</h3>
<blockquote>Characters: 的,一,是,不,了,在,人,有,我,他,这,个,们,中,来,上,大,为,和,国,地,到,以,说,时,要,就,出,会,可,也,你,对,生,能,而,子,那,得,于,着,下,自,之,年,过,发,后,作,里,用,道,行,所,然,家,种,事,成,方,多,经,么,去,法,学,如,都,同,现,当,没,动,面,起,看,定,天,分,还,进,好,小,部,其,些,主,样,理,心,她,本,前,开,但,因,只,从,想,实

Total Dictionary Lookups (with assumption): 101,000,100

Total Dictionary Entries Found: 1128

Percentage of Words Found: 0.001%

Ratio of characters to words: 1:11.26

Total Computing Time Before Index: NA

Total Computing Time After Index: 31min</blockquote>
Things seemed to have escalated quickly. I did over 101,000,100 (yes, that 100 million!) dictionary lookups. Through some more heuristics of character combinations I could've brought that number down, but I'm not a pro on natural language processing just yet. You'll also need to do quite the analysis.

Besides the big numbers involved. I'm glad we finally crossed the 1000 word mark.

Furthermore, the ratio of characters to words from 50 to 100 characters went up by 73%. From 25 to 50 that increase was closer to a 53.7% increase. It would be interesting to see this ratio played out across higher ranges (200 characters, 400 characters, 800 characters) to see if there is a similar exponential trend.

There are quite a few four character words that popped up. Here are my favourites: 有人想你 (bless you!), 自我实现 (Maslow's Hierarchy of Needs), 自然而然 (Involuntarily) and 同道中人 (Kindred Spirit).
<h3 dir="ltr">Other Findings</h3>
I decided to run further analysis on the 1128 words that were generated with the 100 characters. Here's some interesting stats:
<blockquote>Characters that start the most words: 不 (59 words), 大 (47 words) and then surprisingly 自 (30).

Number of two character words: 785

Number of three character words: 180

Number of four character words: 63

New order of character frequency based on only the words generated (highest to lowest): 不,人,大,一,家,有,事,心,来,得,学,中,上,下,自,当,生,理,好,地,分,道,子,行,看,时,天,出,说,国,过,成,年,小,面,要,用,本,对,会,为,法,想,多,动,前,是,方,在,所,作,了,起,样,然,同,发,以,个,没,可,能,开,定,这,着,现,从,主,实,之,去,到,后,部,进,的,而,种,就,如,那,我,只,些,于,里,因,其,经,都,还,和,么,们,你,他,但,也,她</blockquote>
It's interesting to look at the new frequency of the characters. Like, 他, which places among the highest in frequency according to Junda's corpus, which takes a lot of novels and texts into account, is now lowest among the 100 most characters only based on the frequency of vocabulary.

One could almost say that there are two kinds of character frequencies: frequency of occurrence in texts vs frequency of occurrence in vocabulary. I wonder if there are interesting correlations to be made here. Maybe if we one wants to be efficient in learning Chinese characters, one needs to look at both frequencies, because they both can create good angles of approach.

We all have learned 他, 她 and 你 as some of the first characters we encounter. It makes sense. So looking at frequency only isn't the necessarily the best approach, but I think there are definitely interesting ways to use frequency to your advantage.

Like, 不, here above for example. It is high in both frequencies and has created the most words, thus it is awesome character.
<h3>Conclusion</h3>
It was a fun experiment. Perhaps there are interesting experiments like this to be made. Most of words are obscure though. I'm not sure of their usefulness, like 成说 (accepted theory or formulation), 天年 (Natural Life Span), 心经 (The Heart Sutra) and 地心说 (geocentric theory) among many others.

I was curious to see how many words there are actually when one takes the most frequent characters. To think about it, if you know 100 characters, you could potentially know 1128 words. That's kinda cool. Whether that translates to useful words, like I mentioned above, is probably not likely.

Ultimately, it would be really cool to take one's own character knowledge and compute that. Unfortunately, it's hard to get that exact knowledge (perhaps from <a href="http://ankisrs.net">Anki</a> or <a href="http://www.skritter.com/?siteref=ConfusedLaowai">Skritter</a>?), but also to do those potential vocabulary lookups past 100 characters can get very very expensive in computation.

I'll see if I can create a little app that looks up character combinations for characters a user manually provides.

Anyhoo, here is the list of all the words per character category (10, 25, 50 and 100) + all four character combinations: <a href="https://docs.google.com/document/d/1mkcNHhXsPumKZo5Iy07i8xCIeLqrC04Dh63t1Ylffi4/edit">Google Doc Link</a>. Have fun!

<em>EDIT: I got a comment on reddit (and here) from Rob who also did a similar experiment. He used the most frequent characters from Harry Potter up to 6000 characters! Check the <a href="http://pastebin.ca/2196978">data here</a>. Awesome stuff.</em>