---
layout: post
title:  "Dallas Crime Predictions"
date:   2021-10-22
excerpt: "My largest foray to-date into the world of Data Science and Machine Learning to answer real-world questions."

categories: 
tags: [Data Science, Python, Machine Learning]

repo_url: https://github.com/AustinCaudill/Dallas-Crime-Predictions
---
<h2>The Motivation and Objective</h2>
<p>Given my recent fascination with training machine learning models, I have begun looking for applications to use them everywhere in my personal life. This project idea came to life quickly after an unfortunate incident on the very street I live on. I quickly realized my local Police Department could certainly benefit from having more information - and more importantly - more easilcy accessed and understood information at their fingertips. Thus the motivation was born.

The objective was simple: To understand the types and scale of data made available by the City of Dallas and see if I could use any of it to understand the where and when of crime in the city. And as an added bonus, I was going to attempt to train a machine learning model on the data to see what may come of it.</p>
<h2>My Role</h2>
<p>In the interest of transparency, I must note that this project is of entirely my own motivations and volition. I have not partnered with any person or institution to gather, process, or interpret the data used in this prooject.</p>
<h2>The Data</h2>
<span class="image left"><img src="/media/datascience/data-source-preview.png"></span>
<p>The data for this project came directly from the Dallas Police Public Data site located <a href="https://www.dallasopendata.com/Public-Safety/Police-Incidents/qv6i-rri7" target="_new">here.</a> At time of writing, this data set consists of 861,000 rows and 86 columns at approximately 804mb in size. 
If you are interested in downloading this dataset for yourself, and do not require the most up-to-date data, I have archived a full copy of the data set here on my server to prevent excessive resource usage for the City of Dallas. <a href="datascience.thepetroguy.com/public/Police_Incidents.csv">Download this here in csv format.</a>
</p>
<p>With a dataset of this size, a substantial amount of cleaning had to be done. The largest amnount of cleaning occurred as a result of deleting duplicate rows for the same crime incident. The way data is entered into this spreadsheet, if multiple "units" or responding officers are assigned to an incident, another row is created with no further information other than the responding officer's badge number and patrol car. During Exploratory Data Analysis, EDA, it became clear that good records weren't kept until mid-2014, so I then dropped any rows prior to 2015. Luckily for me, Latitudinal and Longitudinal coordinates for the crimes were included in one columnn of the spreadsheet. I broke these out into separate columns for ease of use later on. 
</p>
<h2>Plotting & Graphing</h2>
<p>With the data cleaned, the next step was to understand more about what I was looking at. 
</p>