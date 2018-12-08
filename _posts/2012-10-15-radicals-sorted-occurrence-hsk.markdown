---
layout: post
title: Radicals sorted by their first occurrence in HSK
date: '2012-10-15 16:14:10'
tags:
- chinese-characters
- hsk
- sorted-based-on-level
---

I was looking at my blog's web analytics when I saw a few hits coming from <a href="http://www.skritter.com/?siteref=ConfusedLaowai">Skritter's</a> forum. I headed on over and found <a href="http://www.skritter.com/forum/topic?id=222399262">an interesting topic</a>. Is there a list of radicals sorted by their first occurrence in HSK? So, basically, show the components based on their entry into an HSK level. I decided to spend the day and code this up using code from <a href="http://hanzijs.com">HanziJS</a>. It was interesting question and I was curious myself.
<h2>Details</h2>
I used the characters I got <a href="http://blog.nciku.com/blog/en/2011/03/09/hsk-character-list-and-stroke-order-animations/">from Nciku's list</a>. These characters also seemed to be organized by frequency on each level. I then used HanziJS's radical decomposition code and got all the radicals in each character. I then ran each characters components and found the first unique occurrence of each component and noted the level of HSK it occurred in and which character it was found in. With this list of unique components I then compiled this list of radicals based on the <a href="http://en.wikipedia.org/wiki/List_of_Kangxi_radicals">KangXi list</a>. The data was not entirely consistent, as I found some bugs in the decomposition data, but I edited the rest of the code by hand.

Here's how the list works:
<blockquote>Nr of radical according to Kangxi Radical list: HSK Level, First Character Occurrence (additional information)</blockquote>
The additional information is where I listed findings based on bound radicals and simplified forms. This is especially true for some of the "not found" components where most are traditional forms. You won't find them in HSK's six levels.

Here's the list. You can also <a href="http://confusedlaowai.com/hsklistfirstoccurrencesorted.txt">download the .txt file</a> too.
<pre>1) 一: 1, 一
2) 丨: 1, 在
3) 丶: 1, 的
4) 丿: 1, 不
6) 亅: 1, 了
7) 二: 1, 会
8) 亠: 1, 京
9) 人: 1, 人 (亻: 1, 们)
10) 儿: 1, 说
12) 八: 1, 期
13) 冂: 1, 同
14) 冖: 1, 学
15) 冫: 1, 冷
16) 几: 1, 机
17) 凵: 1, 脑
18) 刀: 1, 分 (刂: 1, 前)
19) 力: 1, 五
20) 勹: 1, 的
21) 匕: 1, 些
22) 匚: 1, 医
24) 十: 1, 年
25) 卜: 1, 不
28) 厶: 1, 会
29) 又: 1, 对
30) 口: 1, 中
31) 囗: 1, 国
32) 土: 1, 在
33) 士: 1, 喜
34) 夂: 1, 客
36) 夕: 1, 名
37) 大: 1, 大
38) 女: 1, 好
39) 子: 1, 学
40) 宀: 1, 家
41) 寸: 1, 时
42) 小: 1, 京 (⺍: 1, 学)
44) 尸: 1, 呢
46) 山: 1, 岁
48) 工: 1, 工
49) 己: 1, 起
50) 巾: 1, 师
51) 干: 1, 午
53) 广: 1, 店
59) 彡: 1, 影
60) 彳: 1, 很
61) 心: 1, 想 (忄: 2, 快)
62) 戈: 1, 我
64) 手: 1, 我 (扌: 1, 打)
67) 文: 1, 这
69) 斤: 1, 听
72) 日: 1, 是
73) 曰: 1, 喝
74) 月: 1, 有
75) 木: 1, 来
76) 欠: 1, 欢
77) 止: 1, 些
79) 殳: 1, 没
84) 气: 1, 气
85) 水: 1, 水 (氵: 1, 没)
86) 火: 1, 火 (灬: 1, 点)
88) 父: 1, 爸
96) 玉: 1, 国
99) 甘: 1, 期
100) 生: 1, 生
102) 田: 1, 果
106) 白: 1, 的
109) 目: 1, 看
111) 矢: 1, 医
113) 示: 1, 漂 (礻: 1, 视)
115) 禾: 1, 和
117) 立: 1, 站
119) 米: 1, 米
120) 糸: 1, 系
123) 羊: 1, 样
125) 老: 1, 老
135) 舌: 1, 话
138) 艮: 1, 很
145) 衣: 1, 衣
146) 西: 1, 西 (覀: 1, 漂)
152) 豕: 1, 家
156) 走: 1, 起
158) 身: 1, 谢
166) 里: 1, 里
172) 隹: 1, 谁
173) 雨: 1, 雨
176) 面: 1, 面
189) 高: 1, 高
23) 匸: 2, 望
26) 卩: 2, 迎
27) 厂: 2, 颜
43) 尢: 2, 就
56) 弋: 2, 试
57) 弓: 2, 张
58) 彐: 2, 雪
63) 戶: 2, 所
70) 方: 2, 房
80) 毋: 2, 每
81) 比: 2, 比
83) 氏: 2, 旅
92) 牙: 2, 穿
93) 牛: 2, 件
97) 瓜: 2, 瓜
103) 疋: 2, 蛋
104) 疒: 2, 病
108) 皿: 2, 篮
114) 禸: 2, 离
116) 穴: 2, 穿
128) 耳: 2, 最
130) 肉: 2, 肉
132) 自: 2, 自
133) 至: 2, 到
136) 舛: 2, 舞
137) 舟: 2, 船
139) 色: 2, 色
142) 虫: 2, 蛋
144) 行: 2, 行
157) 足: 2, 足 (⻊: 3, 跟)
175) 非: 2, 非
180) 音: 2, 意
203) 黑: 2, 黑
35) 夊: 3, 夏
54) 廴: 3, 健
55) 廿: 3, 世
82) 毛: 3, 笔
87) 爪: 3, 爬 (⺤: 1, 爱)
91) 片: 3, 片
94) 犬: 3, 然 (犭: 1, 狗)
101) 用: 3, 用
112) 石: 3, 碗
121) 缶: 3, 萄
122) 网: 3, 网 (罒: 2, 慢)
126) 而: 3, 而
129) 聿: 3, 健
134) 臼: 3, 瘦
148) 角: 3, 解
149) 言: 3, 信 (讠: 1, 说)
150) 谷: 3, 容
151) 豆: 3, 短
164) 酉: 3, 酒
171) 隶: 3, 康
177) 革: 3, 鞋
185) 首: 3, 道
186) 香: 3, 香
209) 鼻: 3, 鼻
11) 入: 4, 入
45) 屮: 4, 塑
65) 支: 4, 技
66) 攴: 4, 敲
68) 斗: 4, 科
71) 无: 4, 无
78) 歹: 4, 列
98) 瓦: 4, 瓶
107) 皮: 4, 被
124) 羽: 4, 翻
141) 虍: 4, 虑
143) 血: 4, 血
153) 豸: 4, 貌
165) 釆: 4, 播
167) 金: 4, 金 (钅: 1, 钱)
160) 辛: 4, 辛
184) 食: 4, 食 (饣: 1, 饭)
200) 麻: 4, 麻
207) 鼓: 4, 鼓
5) 乙: 5, 乙
52) 幺: 5, 率
105) 癶: 5, 登
110) 矛: 5, 矛
118) 竹: 5, 竹 (⺮: 2, 第)
127) 耒: 5, 籍
131) 臣: 5, 藏
161) 辰: 5, 震
188) 骨: 5, 滑
190) 髟: 5, 髦
193) 鬲: 5, 融
194) 鬼: 5, 魅
208) 鼠: 5, 鼠
47) 巛: 6, 巡
89) 爻: 6, 攀
95) 玄: 6, 蓄
155) 赤: 6, 赤
140) 艸: not found (艹: 1, 菜)
147) 見: not found (见: 1, 现)
159) 車: not found (车: 1, 车)
162) 辵: not found (辶: 1, 这)
163) 邑: not found (阝: 1, 都)
169) 門: not found (门: 1, 们)
170) 阜: not found (阝: 1, 院)
174) 靑: not found (青: 1, 请)
183) 飛: not found (飞: 1, 飞)
187) 馬: not found (马: 1, 吗)
154) 貝: not found (贝: 2, 员)
168) 長: not found (长: 2, 长)
181) 頁: not found (页: 2, 题)
195) 魚: not found (鱼: 2, 鱼)
196) 鳥: not found (鸟: 2, 鸡)
182) 風: not found (风: 3, 风)
178) 韋: not found (韦: 4, 围)
210) 齊: not found (齐: 4, 济)
211) 齒: not found (齿: 4, 龄)
199) 麥: not found (麦: 5, 麦)
205) 黽: not found (黾: 5, 绳)
212) 龍: not found (龙: 5, 龙)
90) 爿: not found
179) 韭: not found
191) 鬥: not found
192) 鬯: not found
197) 鹵: not found
198) 鹿: not found
201) 黃: not found
202) 黍: not found
204) 黹: not found
206) 鼎: not found
213) 龜: not found
214) 龠: not found</pre>
There might be some errors here somewhere. If you spot anything let me know!