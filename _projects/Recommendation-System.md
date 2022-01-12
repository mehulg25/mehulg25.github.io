---
title: "Recommendation System"
layout: post
sub_title: "Predictive Analysis"
excerpt: "Predictive Analysis"

image: 
  path: assets/images/projects/recommendation-banner.jpg
  thumbnail: assets/images/projects/recommendation-thumbnail.jpg
actions:
  - label: "GitHub"
    icon: github
    url: "https://github.com/mehulg25/Recommendation-System"
  - label: "Download Report"
    icon: pdf
    url: "/pdf-asset/FinalReport.html"
---
I was listening to music when I came across a bunch of in-house curated playlists. I noticed how those playlists were curated not based on the genres but based on moods, actions, and whatnot. I was curious to know how users consume digital products in this day and age, so I decided to build my own music recommendation system. But before building a recommendation system, I wanted to dig deeper into the data behind this in order to find some trends in user listening habits.

![plot](/assets/images/projects/spot-meme.jpg)

---

For this project, I decided to work on a dataset collected from [Spotify](https://www.spotify.com/us/). The dataset included 1 million playlists with their respective songs. However, for the scope of this project, I decided to work only on the first 1,000 playlists.

I started off by making a correlation matrix to see if there was any relation between the track metadata, i.e., the song attributes like acousticness, valence, loudness, and popularity, to name a few. 

![plot](/assets/images/projects/corr.png)

As observed, there was only one strong correlation - Loudness Vs. Energy. However, not a single attribute was highly correlated with popularity of the track. 

I was curious to know what exactly differentiates a popular song from other songs. I wanted to know - Is there a recipe that can be used to “make” songs?

To answer this question, I filtered out the 5 most and 5 least popular artists to compare the attributes of the songs using a radar chart. 

![plot](/assets/images/projects/radar.png)

I was able to identify what should be kept in mind before composing a song. It was observed that popular songs tend to have the following attributes:
- High Valence
  - Valence is nothing but a measure of happiness
- High Danceability
- Less Speechiness
- Less Acousticness

After observing these trends, I decided to analyze the growth of genres over the years, as well as how billboard decides on _Artist of the Decade_. Feel free to check out the [full report](/pdf-asset/FinalReport.html) for a more detailed analysis and related visualizations.

For the recommendation system, I started by filtering out the data based on the genre of the input song. Then, I used Cosine Similarity to find a similarity matrix between song attributes. Cosine Similarity is used to find similarity between two non-zero vectors. Here, the two non-zero vectors were the song attributes (input song and target song). The similarity was found by calculating the angle between these two vectors. I also decided to use Hamilton Similarity, which is similar to Cosine Similarity, in order to further refine the recommendation. 

Honestly, I was pretty impressed by the results. My input song was Enter Sandman by Metallica, the results for which can be seen below: 

![plot](/assets/images/projects/results.png)

From audio cassettes to vinyl disks, and iPods to iTunes, as media products shift from physical goods to bits, the way people explore and perceive new media has also changed through the years, making user personalization a very important aspect for any platform in this digital age. 

In the future, I would like to further this research and explore more about song recommendations based purely on the name of the playlists. 

---

To test this project, feel free to fork my repo on [github](https://github.com/mehulg25/Recommendation-System). You can also [download](/pdf-asset/FinalReport.html) the full HTML report for a detailed analysis.

I would like to thank Aarti Yelne, Danny Rivas, Nishit Chaudhari, and Saloni Shah for their help and insights.


