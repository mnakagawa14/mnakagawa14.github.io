---
layout: essay
type: essay
title: "From Curiosity to Understanding: The Goal of Smart Questions"
# All dates must be YYYY-MM-DD format!
date: 2023-09-05
published: true
labels:
  - Learning
---
From Curiosity to Understanding: The Goal of Smart Questions

Communication is one of the most important skills to have in any career. It can be the difference between an efficient development process and hours of troubleshooting and stalled progress. There are many resources available on the web that allow developers to tap into each other's expertise, however StackOverflow is perhaps the most prominent.

StackOverflow, a question and answer website for programmers, has developed quite a reputation for itself. On the one hand, it hosts tens of millions of questions and answers as well as a strong community of experienced developers providing a deep resource to draw upon. On the other hand, it has the reputation of not tolerating dumb, vague, or lazy questions which can result in downvoting and possible question removal.

In his essay [“How To Ask Questions The Smart Way''](http://www.catb.org/esr/faqs/smart-questions.html), Eric Steven Raymond outlines some basic guidelines on how to get the most out of online resources. He makes several seemingly simple yet meaningful observations about what type of questions produces the best outcomes. He notes that all other resources should be utilized before it is posed to one's peers. 

This is for several reasons. Perhaps most importantly it could lead to finding a solution either through documentation, experimentation, or an answer to a previously posted question. Even if no exact solution can be found, research allows you to refine your understanding of the issue and to more precisely pose your question. It also shows a willingness to work and learn, which is much more likely to gain you respect.

To put this new knowledge into practice, I began to examine StackOverflow not on their subject matter but on their quality as questions. I quickly found poorly thought out questions, perhaps the most egregious of which was titled [“how to send 100,000 emails weekly?”](https://stackoverflow.com/questions/3905734/how-to-send-100-000-emails-weekly). 
```
How can one send an email to 100,000 users on a weekly basis in PHP? This includes mail to subscribers using the following providers:
AOL
G-Mail
Hotmail
Yahoo
It is important that all e-mail actually be delivered, to the extent that it is possible. Obviously, just sending the mail conventionally would do nothing but create problems.
Is there a library for PHP that makes this simpler?
```

In this post, instead of having a specific technical question he outlines the ultimate goal of his project. This was to “send an email to 100,000 users on a weekly basis in PHP”. He goes on to list the email providers that should be reached and emphasizes the importance of reliability. This is a bad question because it is clear that the questioner has put in little to no effort in answering his question himself. Anyone attempting to help the questioner would essentially be doing all the work themselves.

To contrast, I found a good question titled [“Dataframe Sample in Apache Spark”](https://stackoverflow.com/questions/37416825/dataframe-sample-in-apache-spark-scala). 

```
I'm trying to take out samples from two dataframes wherein I need the ratio of count maintained. eg
df1.count() = 10
df2.count() = 1000

noOfSamples = 10

I want to sample the data in such a way that i get 10 samples of size 101 each( 1 from df1 and 100 from df2)
Now while doing so,
var newSample = df1.sample(true, df1.count() / noOfSamples)
println(newSample.count())

What does the fraction here imply? can it be greater than 1? I checked this and this but wasn't able to comprehend it fully.
Also is there anyway we can specify the number of rows to be sampled?
```
Even though I know nothing about Apache Spark, it is clear that the questioner has put some effort into solving the problem himself. First he outlines his problem of maintaining a ratio count when taking samples from two data frames. In doing so he provides the code he has attempted to implement. In addition he links two other posts on StackOverflow that were related to his question, but admits to not fully understanding them. The fact that there was a clear attempt to solve the problem as well as being able to pinpoint the issue and area that could use clarification makes this a smart question.

Going forward I hope to ask smarter questions. This will help me to better utilize available resources, as well as to improve my thought process in general.
