---
title: "Recommendation System"
layout: post
sub_title: "Predictive Analysis"
excerpt: "Predictive Analysis"

image: 
  path: assets/images/projects/recommendation-3.png
  thumbnail: assets/images/projects/recommendation-3.png
actions:
  - label: "GitHub"
    icon: github
    url: "https://github.com/mehulg25/Recommendation-System"

---
I was listening to music when I came across a bunch of in-house curated playlists. I noticed how those playlists were curated not based on the genres but based on moods, actions, and what not. 
I was curious to know how users are actually consuming digital products in this age and so I decided to build my own recommendation system. But before building a recommendation system, I wanted to dig deeper into the data in order to find some trends in user listening habits. <br>
![plot](/assets/images/projects/spot-meme.jpg)
---
For this project, I decided to work on the Spotify dataset. The dataset included 1 million playlists with their respective songs. However, for the scope of this project, I decided to work only on the first 1,000 playlists.

I started off by making a correlation matrix to see if there is any relation between the track metadata, i.e., the song attributes like acousticness, valence, loudness, and popularity to name a few. 
![plot](/assets/images/projects/corr.png)
As we can see, there's only one strong correlation - Loudness Vs. Energy.
However, not a single attribute is highly correlated with popularity of the track. 

I was curious to know what exactly differentiates a popular song from other songs? Is there a recipe to make songs? <br>
To answer this question, I filtered out 5 most and least popular artists to compare the attirbutes of the songs by these artists using a radar chart. 
![plot](/assets/images/projects/radar.png)
Now we know the things that we should keep in mind before composing a song. Popular songs tend to have the following attributes:
- High Valence
  - Valence is nothing but a measure for happiness
- High Danceability
- Less Speechiness
- Less Acousticness

After observing these trends, I decided to analyze the growth of genres over the years and how billboard decides _Artist of the Decade_. You can check out the full report for a detailed analysis and visualizations.

For the recommendation system, I first filtered out the data based on the genre of the input song. Then, I used Cosine Similarity to find a similarity matrix between song attributes. Cosine Similarity is used to find similarity between two non-zero vectors. Here, the two non-zero vectors were the song attributes (input song and target song). The similarity was found by calculating the angle between these two vectors. I also decided to use Hamilton Similarity which is just like Cosine Similarity in order to further refine the recommendation. 

Honestly, I was pretty impressed by the results. My input song was Enter Sandman by Metallica, and you can see the results yourself.
![plot](/assets/images/projects/results.png)

To wrap it up, from audio cassettes to vinyl disks, from ipods to itunes, as media products shift from physical goods to bits, the way people explore and perceive new media has also changed through the years, making user personalization a very important aspect for any platform in this digital age. 

In future, I wish to explore more on recommending songs based purely on the playlists name. 

---

I would also like to thank Aarti Yelne, Danny Rivas, Nishit Chaudhari, and Saloni Shah for their help and insights.


---
