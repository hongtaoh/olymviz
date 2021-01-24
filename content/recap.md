---
title: Recap
author: Chris Fang & Hongtao Hao
---
## Research Question Recap
This paper answered four major questions:

- How does female participation at the Olympics, both overall and in each continent, change over time?
- Is there a home-field advantage at the Olympics?
- What is the medal efficiency for each country and region?
- Which sports have the highest number of participating athletes at the Olympics?

## Major Findings
Our visualizations demonstrated that:
- Both the total number of participating athletes and the percentage of female athletes in the Olympics has been increasing. Female participation started from 0% in Athens 1896 to 45\% in Rio 2016. 

- However, this growth in the rate of participation of women varies across continents. The rate in Africa has always been lower than the global average except for during the 1930s. The rate in Asia and South America had also been always lower than the global average but caught up during the 1980s and 2000s, respectively. The rate in Europe, North America and Oceania has always been the same as or higher than the global mean.

- A country is more likely to have a higher degree of medal share when it hosts the Olympics. In other words, home-field advantage does seem to exist in the Olympics. 

- Among today’s countries and regions, the United States of America has the highest medal efficiency, 0.91. This means that on average, every American athlete almost earned a Bronze medal in the past Olympic Games. Medal efficiency for Russia, China, Pakistan, India, Germany, and Australia is also very high. We also found that medal efficiency had a high correlation with countries' economic development. 

- Athletics, gymnastics, swimming, shooting and football are among the sports with the highest number of participating athletes. This might be because these sports have greater shares of total medals. It might also because there are many sub-categories within them.

## Reflections & Future Work
First, when visualizing changes in female participation, we found that stacked bar charts are effective in showing the comparisons between male and females. Stacked area charts do not provide very accurate percentage change, but it is good if we also want to show how the total number of athletes has been increasing. The seaborn FacetGrid function is useful for visualizing female participation by continent. Reference information set in grey in the background and highlighting the global average helps us make comparisons between continents and with the global average much clearer. Our next step is to do this graph with Altair so as to enable interactivity when we post it online. 

In our study into the home-field advantage, we realized that even with jittering, scatter plot is not effective at showing a large number of data points. Beeswarm plot with box plot is good at displaying all the points without overlapping, but its representation of density distribution is not very intuitive and direct. KDE in a small multiple is a much better method for showing the distribution clearly. KDE in this case is especially useful for examining home-field advantage because it shows the level of probability that a country gets a certain share of medals. 

Our introduction of “medal efficiency” contributes to the assessment of a country’s efficiency at obtaining Olympic medals. The choropleth we used allows us to show all the countries and regions interactively. However, we acknowledged that it would have been better if it were a cartogram.  This might be our next step. 

Using word cloud is a very unique way to show the relative size of participation in various sports. The drawback is that some sports have two or more words in their names, and our processing of word clouds might not have been rendering their frequencies very accurately. That is why we see “water”, “art” and “competition” in the word cloud. We will fix this problem in our next step. 

We will publish it online as our portfolio later. 