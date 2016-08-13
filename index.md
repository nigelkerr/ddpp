---
title       : Predicting Wages Based On Demographics
subtitle    : Making the Limits of Machine Learning Personal
author      : Nigel Kerr
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---



## Rainbows and Unicorns

Machine learning techniques and the abundant computing power to use them create
many opportunities to make predictions and classifications that have been
difficult heretofore.

Media hype around machine-learning is considerable and sustained, to link only a few:

* [Use Data to Tell the Future: Understanding Machine Learning](http://www.wired.com/insights/2014/03/use-data-tell-future-understanding-machine-learning/), Wired, 2014
* [Immensely powerful’ machine learning has potential to predict the future](http://www.computing.co.uk/ctg/news/2434719/-immensely-powerful-machine-learning-has-potential-to-predict-the-future), Computing, 2015
* [Unlocking The Potential Of Machine Learning](https://channels.theinnovationenterprise.com/articles/unlocking-the-potential-of-machine-learning), Innovation Enterprise, 2016

With appropriate data and techniques, it seems that all kinds of problems can be solved.

--- 

## NOT ALL Rainbows and Unicorns

Like any tool we use, machine learning requires decisions:

1. how are the training data collected?
2. how are the training data tidied?
3. how representative of a populations variations is the training data?
4. what variables will be used for prediction?
5. how are predictions validated after the model is built?
6. how will the prediction be used?

Inattention or negligence on any of these decisions may yield a predictive machine 
learning model with blind-spots and poor prediction, or exerts unaccountable influence
over lives or pubic business.

--- 

## Poor Data Source vs. The Public

We present an app to allow a user to explore these dangers:

<https://attack-plan-r.shinyapps.io/fproject/>

The app accepts user input on some demographic data to make a possibly wildly-inaccurate prediction 
for their annual income.  The `Wage` dataset from the ISLR R package 
is not good for predicting much, for example one of the columns:


```r
summary(Wage$sex)
```

```
##   1. Male 2. Female 
##      3000         0
```

If these data were used to predict for public policy reasons, there are a lot of people who
will be misrepresented on this question alone.  The app describes how the user-input differs
from the model training data.

---

## Where to Go From Here

The example app attempts to show the potential disconnects on a small scale.  
Because statistics and compute power are so easy to use now, machine learning may be going on right now without us knowing it in our everyday life.

As citizens and consumers, we must from now on be alert to what machine learning
may be shaping our health, happiness and well-being, and that of others.  

