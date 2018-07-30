---
layout: page
title: Data Science
permalink: /ml/
---


Intro
======

I'm excited by the possibility of using data to make better predictions and advance knowledge. I think there's a lot of opportunity to improve allocation systems and make discoveries through better use of data. At MIT one of my primary goals was to give myself the tools to do so. This led me to study core material such as probability theory and linear algebra as well as its applications in machine learning, data science and econometrics. 

I've selected a couple of my favorite projects that show some of the creative ways that data can be used to attack problems. I had a ton of fun working on these projects, and they have produced interesting conclusions. I'm still on the look out for new problems and data sets to play around with.        


Criminology
======

Crime is interesting because it is a complex social phenomenon with many different proposed explanations and plethora of data. I became interested in using arrest data to study crime. However this data is full of unobserved effects and bias, which makes it challenging to use rigorously. Here two of the projects in which I used different techniques understand crime through data.  

In a project for my data science class, we obtained a dataset of arrest records for Quebec during the past decade. Most significantly this dataset contains _co-arrests_, which tell us which criminals have been arrested together. Using this data we attempted to measure the effect of social ties on crime. Specifically we wanted to use social network analysis to predict whether a person would re-offend, who they would be arrested with in the future and what they would be arrested for. Our network models were surprisingly powerful and could reliably predict recidivism and identify criminal communities. 

Here is a the full write up:    

[Predicting Criminal Behavior with Networks](/files/quebec_paper.pdf)

We are also collaborating with Professor Carlo Morselli, a criminologist, to present our findings at the American Criminology Society:
 
[Presentation at the American Society of Criminology](http://tinyurl.com/yba3vxxs)


In a separate project for a class on networks, I used geographic crime data in Chicago to analyze the strategic behavior in crime. This work focused on empirical measurement of the effect of an individual's choice to commit a crime on those around him. Specifically is crime a _complementary_ good, in which one crime creates opportunity for another, or are crimes _substitutes_ for each other, for example when drug dealers sell similar products? We created a network model for crime and then used an instrumental variables approach to try to answer this question. We found that only certain crimes such as narcotics and homicide have strong positive network effects. This could provide evidence for a "broken windows" policy in dealing with crime.  

Here is our paper:

[Is Crime Contagious?](/files/chicago_paper.pdf)


Natural Language Processing 
======

Natural language processing is an area of machine learning focused on computer interaction with human language. It's an interesting field both because of its difficulty and because we know it can be solved (after all you have no problem understanding the meaning of this sentence). I took a stab at it in a graduate course on natural language processing. In the final project for this course, our team attempted to identify the characters from a book using only a spark notes description (with the character name removed) and the plain text. We framed this task as a matching problem and designed and implemented a neural network to perform the matching. We then compared our performance to a simple bag-of-words baseline. 

Overall this problem was very hard - we needed to learn embeddings for words in texts that were centuries apart and written in very different styles. Furthermore our data set was limited to the hundreds of books with spark notes. Our results were not very good, but I still learned a ton  about the topic and it was a fun project. I also got my hands dirty with Tensor Flow and learned how to schedule very large computations on a remote cluster.      

Here is our paper:

[Who's Who](/files/whoiswho_paper.pdf)
