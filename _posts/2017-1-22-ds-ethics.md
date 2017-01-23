---
title: How Not to Build Algorithms
updated: 2017-1-21
---

In the summer of 2016, President Duterte won the Philippine election by a landslide. The months before the election were grueling for many of us Filipinos, particularly on social media. Organized  pro-Duterte efforts to skew perceptions of candidates sprang up from seemingly nowhere, and online bots, trolls, and Facebook pages made up an orchestra and [exploited Facebook News Feed algorithms](http://www.rappler.com/newsbreak/148536-facebook-algorithms-impact-democracy). Websites containing fake or heavily biased news were rampant and rampantly shared by Facebook pages with followings in the millions. Bots and trolls propagated posts and pages and threatened those who retaliated. Through this phenomenon people were siloed into echo chambers devoid of any productive conversation, and our efforts to fight online trolls and encourage conversation were futile by the end of the election. The [plight and frustration of many Filipinos](http://www.manilatimes.net/duterte-is-pnoys-real-legacy/258365/) had already gone too deep.

There are similarities to the [US election](https://www.nytimes.com/2016/08/28/magazine/inside-facebooks-totally-insane-unintentionally-gigantic-hyperpartisan-political-media-machine.html) as well, where News Feed algorithms reinforced cognitive biases and failed to filter out fake news. While Facebook claims not to be a media channel, many of its users use it as such and are unaware of the mechanisms behind what they see everyday.

What are the News Feed algorithms like anyway? Before 2012, the algorithm used in ranking articles was called [EdgeRank](https://en.wikipedia.org/wiki/EdgeRank), and could be simplified into this equation:

![](../latex/ds-ethics/latex-image-1.png)<br>
where:

![](../latex/ds-ethics/latex-image-2.png): edges <br>
![](../latex/ds-ethics/latex-image-3.png): relationship and proximity of user and content <br>
![](../latex/ds-ethics/latex-image-4.png): weight of user reaction <br>
![](../latex/ds-ethics/latex-image-5.png): decay parameter for time


More recently however, the number of features of their News Feed machine learning algorithm increased to the hundreds.
[Facebook now calculates a relevancy score](http://www.slate.com/articles/technology/cover_story/2016/01/how_facebook_s_news_feed_algorithm_works.html), which is assigned to a post given a particular Facebook user. Then, on each user's News Feed, the algorithm sorts Facebook posts by their relevancy scores. These relevancy scores are based on features such as interactions with other users, previous reactions to posts, and virality of the post, many variables that limit someone's Facebook experience to particular patterns as opposed to diversifying it. I hoped to describe the algorithm in greater detail, but Facebook has not disclosed much about it.

We live in a time where data science is widely used and romanticized. Companies, people, and institutions increasingly rely on models and algorithms to make decisions on various issues. However, left unchecked, these models and algorithms can have biases that could negatively impact a lot of people's lives.
