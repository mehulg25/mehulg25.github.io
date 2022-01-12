---
title: "Restaurant Reviews"
layout: post
sub_title: "Database Management and Sentiment Analysis"
excerpt: "Database Management and Sentiment Analysis"

image: 
  path: assets/images/projects/database-banner.jpg
  thumbnail: assets/images/projects/database-thumbnail.jpg
actions:
  - label: "GitHub"
    icon: github
    url: "https://github.com/mehulg25/Restaurant-Reviews"
  - label: "Download Presentation"
    icon: pdf
    url: "/pdf-asset/DBMS_Presentation.pptx"
---
To cope with all the sleepless nights in pursuit of finishing my gazillion submissions, I rely on caffeine. 
NO, it doesn't help one bit! I think it's all in my head. But atleast all my Starbucks trips gave me the idea to take up this project. The aim of this project is to analyze the reviews and tips given by customers to evaluate __Starbucks Coffeehouses__ in and around College Park area.

![starbucks-image](/assets/images/projects/starbucks.jpg)

---

For this project, I started off by scrapping the data from the following websites:
- Yelp!
- Google Reviews
- FourSquare

The data consisted of datapoints such as customer name, review, feedback, check-in time, business name, business address, etc. 

After getting the data in place, I made an __ER diagram__ using [Lucidchart](https://www.lucidchart.com/pages/). This ER diagram further helped me to correlate things of my interest. I also defined certain __business rules__, made a __relational model__, and implemented __normalization__.

![ER-Diagram](/assets/images/projects/ERD.png)

The next task was to create tables and insert corresponding data. I saved these SQL queries in a __DDL__ file. After inserting data into the tables, I made a __DML__ file to create __materialized views__ using complex SQL queries in order to answer the following questions of interest:
- Which is the highest rated Starbucks branch in College Park area?
- What sets the highest rated branch apart from the rest?
- How can we improve the lowest rated branch?
- How can we improve staff allocation strategy?

After getting answers to the above mentioned questions, I decided to do a __Sentiment Analysis__ of customer reviews to better understand their opinions.

Moreover, I made a __Tableau__ dashboard in order to visualize the results and compare the branches easily. 

![ER-Diagram](/assets/images/projects/dashboard.png)

I believe that this project can be used by any business in order to refine their understanding of customers and translate into improved sales.

***

To test this project, feel free to fork my repo on [github](https://github.com/mehulg25/Restaurant-Reviews). You can also [download](/pdf-asset/DBMS_Presentation.pptx) the presentation for a better understanding.
