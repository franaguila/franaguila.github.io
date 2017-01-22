---
title: How Not to Build Algorithms
updated: 2017-1-21
---

In the summer of 2016, President Duterte won the Philippine election by a landslide. The months before the election were grueling for many of us Filipinos, particularly on social media. Organized efforts to skew perceptions of candidates sprang up from seemingly nowhere, and online bots, trolls, and Facebook pages made up an orchestra and [exploited the Facebook News Feed algorithm](http://www.rappler.com/newsbreak/148536-facebook-algorithms-impact-democracy). Websites containing fake or heavily biased news were rampant and rampantly shared by Facebook pages with followings in the millions. Bots and trolls upped [Facebook relevancy scores](http://www.slate.com/articles/technology/cover_story/2016/01/how_facebook_s_news_feed_algorithm_works.html) of the pages and threatened those who opposed them, driving some opposition to silence. Million of Filipinos, however, were tired of the old administration, of poverty, crime, and incompetence. But through this phenomenon they were siloed into echo chambers devoid of any productive conversation. Our efforts to fight online trolls and encourage more constructive conversation were futile by the end of the election.

You could draw some similarities to the [US election](https://www.nytimes.com/2016/08/28/magazine/inside-facebooks-totally-insane-unintentionally-gigantic-hyperpartisan-political-media-machine.html) as well, where the News Feed algorithm reinforced cognitive biases and failed to filter out fake news. Unfortunately, while Facebook claims not to be a media channel, many of its users use it as such, and are unaware of the mechanisms behind what they see everyday.

I recently started reading up on the News Feed algorithm. Before 2012, it was called [EdgeRank](https://en.wikipedia.org/wiki/EdgeRank), and could be simply put in this equation

$\sum_{e} u_e w_e d_e$


We live in a time where data science is widely used and romanticized. Companies, people, and institutions increasingly rely on models and algorithms to make decisions on various issues. However, left unchecked, these models and algorithms can have biases that could negatively impact a lot of people's lives.
