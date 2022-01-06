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
I was curious to know how users are actually consuming digital products in this age and so I decided to build my own recommendation system. But before building a recommendation system, I wanted to dig deeper into the data in order to find some trends in user listening habits. 

For this project, I decided to work on the Spotify dataset. The dataset included 1 million playlists with their respective songs. However, for the scope of this project, I decided to work only on the first 1,000 playlists.

I started off by making a correlation matrix to see if there is any relation between the track metadata, i.e., the song attributes like acousticness, valence, loudness, and popularity to name a few. 
![plot](/assets/images/projects/corr.png)
As we can see, there's only one strong correlation:
- Loudness VS. Energy
However, not a single attribute is highly correlated with popularity of the track. 

I asked myself, if not an attribute, then what exactly differentiates a popular song from other songs? Is there a recipe to make songs? 
To answer this question, I filtered out 5 most and least popular artists. I then compared the attirbutes of the songs by these artists using a radar chart. 
![plot](/assets/images/projects/radar.png)
Now we know the things that we should keep in mind before composing a song. Popular songs tend to have the following attributes:
- High Valence
  - Valence is nothing but a measure for happiness
- High Danceability
- Less Speechiness
- Less Acousticness


---
