---
layout: post
title:  "The Column Hackathon"
date:   2021-11-29
excerpt: "A short writeup describing my participation in a Hackathon with information about the exploratory data analysis and cleaning I performed, data visualization, and data interpretations. "

image: "/media/datascience/hackathon1/cover.png"

categories: 
tags: [Data Science, Python, Data Analytics]

repo_url: https://github.com/AustinCaudill/Hackathon-No-1
---
<h2>Introduction</h2>
<p>This project was completed as part of the <a href="https://www.datacareerjumpstart.com/" target="new">Data Career Jumpstart's</a> Hackathon with data from The Column, a chemical engineering email newsletter. The objective was to help The Column optimize email distribution and content to cater to its' readers.</p>

<h2>EDA and Data Cleaning</h2>
<p>The data provided consisted of multiple spreadsheets containing information about email open rates, links, and link click counts which had to be parsed and combined into one spreadsheet for analysis. Furthermore, there were many duplicate rows or rows with invalid data that had to be purged before EDA could begin. In total, <b>563 Links</b> were parsed and cleaned up for analysis.</p>
<p>I used a package named <a href="https://github.com/AutoViML/AutoViz" target="new">AutoViz</a> to automatically examine the data and provide suggested visualizations to help with the EDA. This is a great way to quickly understand what you are working with, but in my experience it also tends to churn out some pretty useless visualizations as well. </p>
<p><span class="image left"><img src="/media/datascience/hackathon1/fig1.JPG"></span>
From the graph on the left, we can see that readers are more responsive to the newsletter when it is sent on Monday, as the click rate to external links is much higher. The chart below shows that readers are more engaged with the newsletter around mid-morning.
<span class="image right"><img src="/media/datascience/hackathon1/fig2.JPG"></span>
</p>
<h2>Link Scraping and Results</h2>
<p>The links that were processed were then scraped to determine the most commonly interacted-with topics. Approximately <b>442k words</b> were analyzed. I created word frequency and pair frequency graphs to visualize the most commmonly occuring words and pairs from the links that reader's clicked on in the newsletter. This was assumed to be a measure of the content readers were most interested in. 
<span class="image"><img src="/media/datascience/hackathon1/fig3.JPG"></span>
<span class="image"><img src="/media/datascience/hackathon1/fig4.JPG"></span></p>
<p>The graphs above show that "chemical" and "company" are the 2 most common words in all of the links clicked, which makes sense given the audience of this newslettter. Interestly, "press release" is the most common pairing, indicating that readers are interested in reading the press releases belonging to the stories within the newsletter.</p>
<p>Finally, just to add a little more character to the project, I created the wordcloud below with text size indicative of word count.</p>
<center><span class="image"><img src="/media/datascience/hackathon1/fig5.png"></span></center>
<br />
<h2>The Certificate</h2>
<p>And of course, what would any good Hackathon contest be without a participation certificate?
<center><span class="image"><img src="/media/datascience/hackathon1/certificate.jpg"></span></p></center>