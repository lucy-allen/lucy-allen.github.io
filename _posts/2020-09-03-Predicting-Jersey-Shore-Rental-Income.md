---
layout: post
title: Predicting Jersey Shore Rental Income
---

![](images/stone_harbor_front.jpg)

### Motivation

One of my absolute favorite places to be is at the beach!  During the summer I spend most of my weekends there and some full weeks. My happy place is and always has been Stone Harbor, a beach town on the Jersey Shore.  There are always houses on the market in Stone Harbor as there are elsewhere, and I really enjoy window shopping for houses.  As a recent college graduate, I am no where near being able to afford a house, let alone a beach house, so this time spent window shopping should probably be referred to as day dreaming instead.  But hopefully someday this day dreaming can become a reality!  As a very mathematically minded person persuing Data Science, I thought "How can I use my data science skills to help myself afford a beach house?" And that is exactly the question I plan to answer in the rest of this blog.  

### Methodology

Stone Harbor is located in Cape May County New Jersey, so this is where I focused my research, however this methodology could be used in other areas as well, given there is sufficient data available.  There are many rental platforms that exist, so I wanted to focus on just one, and used VRBO rentals.  In order to gain the data from VRBO I used Beautiful Soup and Selenium, two python packages, to web scrape some data from the VRBO website.  I then used pandas and jupyter notebook to conduct some Exploratory Data Analysis and get a better understanding of the data that was available to me.  Since the goal of this project was to predict the rental income, I used sklearn as well to create a linear regression model for these predictions.  

### Exploratory Data Analysis

Exploratory Data Analysis (EDA) is a very important part of any Data Science project.  This allows you to really understand your data before digging into the deeper more complex models.  Some problems can even be solved using just EDA alone, however as this project involved predicting prices, supervised machine learning was required for the project as well.  While doing some EDA and plotting the target and some of the features I had, I noticed that the targer variable, the thing that I want to predict (price), was right skewed.  This is a problem for linear regressions, since a big assumption of linear regressions is linearity.  This means that the relationships between the dependent and independent variable must be linear.  This shouldn't be too surprising given the name "linear regression," however it can easily be violated, and a right skewed distribution of the target variable does just that.  While this might seem like a huge problem, luckily 

