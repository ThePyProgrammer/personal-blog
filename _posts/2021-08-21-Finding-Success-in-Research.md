---
toc: false
layout: post
description: I once thought I would never pursue research in my life. But times have changed, and so have I.
categories: [research]
title: Finding Success in Research
---
<p align="center"><img src="https://miro.medium.com/max/875/1*AwEWQ9jU9IIIad0QIGGl4g.jpeg" />
<br>Photo by <a href="https://unsplash.com/@anniespratt">Annie Sprat</a> on <a href="https://unsplash.com/">Unsplash</a></p>

Reading the title, you must be thinking: “what does a high-schooler in a country like Singapore know about research?”. And you’d be right. I don’t know everything about research. I don’t understand some complex paper titles and I’m certainly unable to read them. But that’s besides the point.

## My First Research Project
A while back, I took part in a small research project. At that time, I was just starting Secondary 3, otherwise known as the 9th grade, at NUS High School, and I was extremely nervous. Seniors had always warned me that Secondary 3, or Year 3, as we call it, was the worst year of our 6-year high-school experience.

And so, when I started to take part in that research project, I was decidedly apprehensive. While we did have the option of taking a research-related module in our course curriculum back in Year 2, I had pass on that in favour of a Math module, where we learnt some interesting stuff like LaTeX and what, at that moment, I didn’t know was known as mathematical research. I had no experience with creating research posters, or writing realistic research papers. I had nothing.

But that wasn’t the only thing.

While we were deciding a project, we came across a relatively mundane project, which combined some of the interests that my groupmates, who unlike me hated Computer Science and coding, and my own. The problem was that the project required experience with Machine Learning. Whereas I was slightly familiar with Data Analytics modules like Numpy and Matplotlib at the time, I was nowhere near the level of a professional Data Analyst.

I had been getting myself involved in GUI Development with Python at the time, spending my entire December Holidays on what was but a slightly functional PyCharm clone, but that was before our school brought us into what I like to call the ‘Brown Ages’.

## The Brown Ages
The ‘Brown Ages’ represented the two semesters wherein our school really went all in to teach us, wait for it… **Java**. Java, in my opinion, is still one of the worst languages I’ve ever learnt, to the point that I’d rather code shell scripts than Java. Whereas I started to warm up to the language over the course of Year 3, my respect for the language drops every passing month, especially after witnessing the powers of Scala and Kotlin, which, mind you, are built on the same exact system as Java, that being the Java Virtual Machine (JVM).

## The Covid Protocol
But soon, things took a turn for the worse. And maybe for the best. Last year started with a global pandemic that swept many nations of their feet, and thrust most, inclusive of me, into a closed-off situation. Entire schools were shut down, and students like me were left astray, locked into a cramped space with little hope of the future.

But that turned out to be a cloud with silver lining. In the meantime of a month-long lockdown, I participated in the prolific Machine Learning course by Andrew Ng on Coursera, and familiarised myself with many of the most important algorithms in Machine Learning, like the ideas of regression (linear, polynomial, ridge, lasso, logistic), K-Means and even, to some extent, Neural Networks. We learnt all this in MATLAB Octave, which is basically a paid specialized data science language. Python basically managed to duplicate many of the specialized features of MATLAB Octave, with the powerful libraries of `numpy` and `matplotlib` , hence explaining the decline in popularity of this language. In summary, it didn’t take long to convert it into Python.

This truly helped me with my research project, but timing was always an issue. I was a victim of poor sleep schedules, catching only 4 hours of sleep daily, and huge amounts of stress, that too besides my research project. So I left it in stasis. For 6 months.

## 6 Months Later
I started off relatively inexperienced, and decided to tinker around with a little dataset to find possible patterns. I decided to process the data with Signal Processing algorithms, and decided to look up possible techniques. Unfortunately, my ArXiv reading was relatively poor, and I was left scraping for possible option to code the Fast Fourier Transform (FFT) based algorithms we used in the project.

We came across a paper that did something very similar to us, but it was a bit more complex and the code was written in MATLAB Octave. Although I had learnt MATLAB Octave before, I felt that doing the project in Python would be better. And hence, I spent a whole gruesome week converting and debugging the code, continuously and incessantly. It was absolutely terrible, but ultimately it helped me a lot.

In case you wanted to see, the following was the data we already had:

![](https://miro.medium.com/max/875/1*nakcqxgmE2jn_vZQtB-WnA.png)
<p align="center">Graph of Accelerometer Data as it evolves through time.</p>

And this was what we got after the Signal Processing had been performed:

![](https://miro.medium.com/max/875/1*grxzEFSOBFSIZWELPyJCpA.png)
<p align="center">Graph of the Postulated Freeze Index Values, the products of the Signal Processing Algorithms.</p>

## Week 2
Following this, with the help of some of my group mates, I was able to find out that Support Vector Machines (SVMs) would be the most efficient Machine Learning model based on the data available. But there was an imminent problem. There were 10 million data points. If we used Scikit-Learn’s SVM utility, we would have to wait for hours and hours of training, possibly days or weeks. We needed to find an efficient form of creating a model. Everything depended on this.

And then I stumbled upon a little contraption called ThunderSVM. ThunderSVM allowed me to do exactly what I wanted: run a non-deep machine learning model on a GPU. And thus, I continued to use ThunderSVM. Until I ran into a problem. I didn’t have a GPU that supported CUDA. Oh god.

So I tried to find a solution. Something that could let me use a GPU which was not on my local computer. And that is when I remembered Google Colaboratory, a software that can allow you to run your notebooks online with a GPU or even a TPU. I had previously used it in another such research-like Time Series Machine Learning project.

## Flashback: 3 Months Ago
> There was once a little kid named Prannaya, who decided to be very dumb. He was over-committed and was dying of Bio and yet he decided to predict Covid-19 um.

Indeed, I decided to predict Covid-19 patterns to predict the trajectory. Using the `statsmodels` API ARIMA function `SARIMAX` , Facebook's Prophet API and Double Exponential Smoothing, I had to code.

Problem was that Jupyter Notebook wasn’t working on my laptop at the time, so I had to find another more usable platform. Hence came in Google Colab. I had been training the model for a whole week throughout the September Holidays, making them what was otherwise a project-work filled nightmare now an surprisingly terrible nightmarish hellscape. But I digress.

# I wish it was over.
I guess I managed to make the model train for a while and eventually it was giving substantial results. The data can be seen below:

![](https://miro.medium.com/max/534/1*hBkeNPmVeIuNq373Tk6ITA.png)

We continued to find better results, but by a certain point, the above was the best data we had. We went with it. And that was it. The project was over. My suffering was over. Or so I thought. You see, even as I stared at that plot in a Colab Notebook, with a sort of bliss in my heart, I was yet to find out that there was something waiting ahead… Something that would change the course of everything.
