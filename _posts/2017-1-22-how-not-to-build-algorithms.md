---
title: How Not to Build Algorithms
updated: 2017-1-21
---

In the summer of 2016, President Duterte won the Philippine election by a landslide. The months before the election were grueling for many of us Filipinos, particularly on social media. Organized  pro-Duterte efforts to skew perceptions of candidates sprang up from seemingly nowhere, and online bots, trolls, and Facebook pages formed an army [exploiting Facebook News Feed algorithms](http://www.rappler.com/newsbreak/148536-facebook-algorithms-impact-democracy).

Websites containing fake or heavily biased news grew in number and were and rampantly shared by Facebook pages with followings in the millions. Bots and trolls propagated posts and pages and threatened those who retaliated. Through this phenomenon, people were siloed into echo chambers devoid of productive conversation, and our efforts to fight online trolls and encourage conversation were futile by the end of the election. The [plight and frustration of many Filipinos](http://www.manilatimes.net/duterte-is-pnoys-real-legacy/258365/) had gone too deep.

There were similarities to the [US election](https://www.nytimes.com/2016/08/28/magazine/inside-facebooks-totally-insane-unintentionally-gigantic-hyperpartisan-political-media-machine.html) as well, where News Feed algorithms reinforced cognitive biases and failed to filter out fake news. While [Facebook claimed not to be a media channel](https://qz.com/770743/zuckerberg-says-facebook-will-never-be-a-media-company-despite-controlling-the-worlds-media/), many of its users use it as such while unaware of the mechanisms behind it.

What are the News Feed algorithms like? Before 2012, the algorithm used to rank articles was called [EdgeRank](https://en.wikipedia.org/wiki/EdgeRank), which can be simplified into this equation:

![](../latex/ds-ethics/latex-image-1.png)<br>
where:

![](../latex/ds-ethics/latex-image-2.png): edges <br>
![](../latex/ds-ethics/latex-image-3.png): relationship and proximity of user and content <br>
![](../latex/ds-ethics/latex-image-4.png): weight of user reaction <br>
![](../latex/ds-ethics/latex-image-5.png): decay parameter for time content was posted


More recently however, the number of features of their News Feed machine learning algorithm increased to the hundreds.
[Facebook now calculates a relevancy score](http://www.slate.com/articles/technology/cover_story/2016/01/how_facebook_s_news_feed_algorithm_works.html), which is assigned to a post given a particular Facebook user. Then, on each user's News Feed, the algorithm sorts Facebook posts by their relevancy scores. These scores are based on features such as interactions with other users, the user's previous reactions to posts, and virality of the post - many of which limit a person's Facebook experience to certain patterns rather than diversifying their experience.

It's not just on the News Feed that algorithms have social or political (or other) implications. Mathematical models and machine learning algorithms are, more than ever, used to make decisions that impact a large number of people.

I recently came across a [podcast](https://cdt.org/blog/tech-talk-weapons-of-math-destruction/) of the Center for Democracy & Technology (CDT) on Cathy O'Neil's research and book entitled, _Weapons of Math Destruction: How Big Data Increases Inequality and Threatens Democracy_. Here she discusses how models and algorithms are imperfect and can create biased decisions (humans create them after all).

In the podcast, she talks about the 2008 financial crisis. The mathematical models used in subprime lending were carelessly built (you could of course add greed into this equation). The models were created with faulty assumptions like, (1) residential real estate prices would always appreciate and (2) mortgage defaults were independent and identically distributed. Eventually what resulted was the biggest financial crisis since the Great Depression.

She also described how policing algorithms have wrongfully labeled people as high risk offenders. Arrests are used to predict future crimes committed, and police are usually deployed to areas where more arrests took place. But arrests don't necessary equate to crime, and so this whole process contributes to uneven policing.

[Algorithms that calculate recidivism rates](http://www.businessinsider.com/racial-bias-in-criminal-courts-2017-1) also have inherent biases in them. In a number of criminal courts in the United States, black Americans were twice as likely to be wrongfully labelled as high risk offenders as white Americans. This came as a result of biased training data and the ensuing [trade-off between predictive accuracy and level of discrimination](https://mathbabe.org/2017/01/04/recidivism-risk-algorithms-are-inherently-discriminatory/).

Facebook's ["Ethnic Affinity" targeting option](https://cdt.org/blog/a-closer-look-at-the-legality-of-ethnic-affinity/) is also controversial. Facebook's algorithms predict users' ethnic affinity without their consent, and companies are able to use this for targeted marketing. Corinthian Colleges, a U.S. for-profit college, used this method and aggressively targeted a number of low-income black single mothers and other vulnerable groups and convinced them that a degree was their shot at a better life. Instead, these people were [left entrenched in student debt](http://america.aljazeera.com/articles/2013/10/11/california-attorneygeneralfilessuitagainstforprofitcollege.html).

These examples are not the only cases where algorithms had or might have negative consequences. [Discrimination in the workplace](https://cdt.org/blog/charting-a-fair-path-forward-on-big-data-algorithms-in-the-workplace/), [experiments without user consent](https://www.theguardian.com/technology/2014/oct/02/facebook-sorry-secret-psychological-experiment-users), among others happen(ed) as well.

We have an enormous responsibility as future data scientists. We'll be creating and wielding algorithms and models that will affect people's lives, so we must be mindful and find good guidelines so that people are protected against harmful decisions and labeling. We should try to avoid pitfalls and keep others' models in check because we might just be heard (after CDT and other civil rights organizations expressed their concerns, [Facebook amended their ethnic affinity policy](https://cdt.org/blog/facebook-announces-changes-to-ethnic-affinity-marketing/)).

We live in a time where data science is widely used and glorified. Companies, people, and institutions increasingly rely on models and algorithms to make even the most important decisions. However, left unchecked, these models and algorithms can inadvertently threaten democracy, increase inequality, and negatively impact people's lives. We data scientists must try our best to prevent that from happening.
