---
title: "Restaurant Reviews"
layout: post
sub_title: "Database Management and Sentiment Analysis"
excerpt: "Database Management and Sentiment Analysis"

image: 
  path: assets/images/projects/database-2.jpg
  thumbnail: assets/images/projects/database-2.jpg
actions:
  - label: "GitHub"
    icon: github
    url: "https://github.com/mehulg25/Restaurant-Reviews"
  - label: "Download Presentation"
    icon: pdf
    url: "/pdf-asset/DBMS_Presentation.pptx"
---
To cope with all the sleepless nights in pursuit of finishing my gazillion submissions, I rely on caffeine. NO, it doesn't help one bit. I think its all in my head. But atleast all my trips to Starbucks gave me the idea to pursue this project. The aim for this project is to analyze the reviews and tips given by customers to evaluate Starbucks Coffeehouses in and around College Park area.

![starbucks-image](/assets/images/projects/starbucks.jpg)

---

For this project, I started off by scrapping the data from the following websites:
- Yelp!
- Google Reviews
- FourSquare

The data consisted of datapoints like customer name, review, feedback, check-in time, business name, business address, etc. 

After getting the data in place, I made an ER diagram using [Lucidchart](https://www.lucidchart.com/pages/). This ER diagram further helped me to interrelate things of my interest. I also defined certain business rules, made relational model, and implemented normalization.

![ER-Diagram](/assets/images/projects/ERD.png)

The next task for me was to create tables and insert respective data. I saved these SQL queries in a DDL file.
After inserting data into the tables, I made a DML file to create materialized views using complex SQL queries in order to answer the following questions of interest:
- Which is the highest rated Starbucks branch in College Park area
- What sets the highest rated branch apart from the rest
- How can we improve the lowest rated branch
- How can we improve staff allocation strategy

After getting answers to the above mentioned questions, I decided to do a Sentiment Analysis of customer reviews to better understand customer opinions. Moreover, I made a tableau dashboard in order to visualize the results and compare the branches easily. 

![ER-Diagram](/assets/images/projects/dashboard.png)

I believe that this project can be used by any business in order to better understand their customers and improve their sales.

***

To test this project, feel free to fork my repo on [github](https://github.com/mehulg25/Restaurant-Reviews). You can also [download](/pdf-asset/DBMS_Presentation.pptx) the presentation for a better understanding.
