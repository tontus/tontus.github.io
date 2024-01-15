---
layout: page
title: Portfolio
permalink: /portfolio/
nav: true
nav_order: 7
---


# Table of Contents
- [Research Publication](#research-publication)
- [Presentation](#presentation)
- [Software Development](#software-development)
  - [Scale Kuwait](#scale-kuwait)

## Research Publication

**Title:** A cognitive behaviour data analysis on the use of social media in the global south context focusing on Bangladesh  
**Paper link:** [Read the Paper](https://www.nature.com/articles/s41598-023-30125-w)  
**Role:** Null hypothesis formulation, Survey design, data collection & analysis, writing manuscript  
**Description:** This research is an extension of my undergrad thesis, “Why do we share fake news?”. In this research, my two teammates and I investigated the human factors that may influence someone to spread misinformation regarding COVID-19 vaccination on social media. After surveying literature from various disciplines, including Philosophy, Psychology, and Computer Science, we formulated several null hypotheses about the pattern of misinformation propagation. We were struggling to find a suitable way to capture the interactions of individuals with fake news. I started reading about other papers to find a way to collect this kind of data. I designed an experiment that can capture and quantify the participants' interactions with a piece of false news in a controlled environment. After collecting some demographic information about the participants, we supplied them with some fabricated news as stimuli about the problems related to COVID-19 vaccines displayed from usually acclaimed sources in Bangladesh. We asked a series of questions related to them. All the survey takers were supplied with the same fabricated news from the same sources to reduce bias. The questions we asked ranged from how it made them concerned about their friends and families to how desperate they were to share these as soon as they finished the survey. We used Likert scales with 7 points to collect data ranging from strongly negative (1) to strongly positive (7). Some examples of the supplied fabricated news are given in Fig. 1 & 2. Those were created by me using Photoshop. Later in the survey, we clarified to the participants that the news was crafted and not actual.

Fig 1: Fabricated news from a renowned english news outlet, The Daily Star in Bangladesh



Fig 2: Fabricated news from another renowned english news outlet, The Dhaka Tribune in Bangladesh

After collecting and cleaning those data by removing reponses that were invalid, we were left with 206 responses. Then, with the instructions of the project supervisor, I began analyzing the data. I used the Chi-square test and the Spearman Rank Correlation Coefficient to measure the correlation between features and applied Ordinal Logistic Regression to see how the features were related. I used pythons’ pandas, numpy, scipy, seaborn and matplotlib libraries to analyze and visualize these data. 

We observed several interesting trends through our research. For example, individuals spending more than 5 hours per day on social media were more likely to spread the false information provided to them compared to users who spent around 2 hours. Additionally, individuals are more likely to share information without verification that originates from a source with whom they have a personal relationship.

Later, we published our research in Scientific Reports. I contributed to writing the manuscript of the paper. 



## Presentation

**Title:** Gamification of ICT textbook material to provide an interactive learning experience  
**Venue:** CHI 2023 Virtual Workshop hosted by HCI4SouthAsia (remote)  
**Role:** Idea generation and presentation  
**Description:** I presented a half-baked idea of a project of gamification of Bangladesh ICT textbook content to provide an interactive learning experience to underprivileged students. This project aims to provide digital literacy to disadvantaged students who don’t have access to the internet and digital devices and prepare them for the upcoming digital world. To make this game effective and engaging, 3 learning principles will be followed. These are (1) **Interest-powered learning**, (2) **Peer-supported Learning**, and (3) **Relevance of learning content.** 

* **Interest-powered learning:** To make the game more engaging for our targeted age group, we will create an interface that simulates a real-life scenario. The interface will be designed to resemble an email inbox and school portal. In this game, the students will act as assistants in a lab. Their job will be to read, reply, and follow the instructions provided in the email address. That instruction may include uploading data or files with their credentials on the school portal and having video calls with other lab members. Some emails may contain spam or phishing content, and students’ tasks will be to identify and avoid those malicious situations.

* **Peer-supported learning:** This game will be designed as a multiplayer game. Each student will have both individual and group tasks. For instance, a task may require one student to read an email and send the right data file to another lab member. After that, the second lab member will receive and upload the data to complete the group task. Inside the game, the students can communicate with each other over the internet to solve any challenges that may arise. This will help strengthen their online collaboration skills. Relevance of learning content: The game’s content will be related to the student’s coursework to aid their understanding. Class 8-10 ICT curricula contain the above-mentioned topics. The content will be embedded within an enjoyable and exciting gameplay, acting as a Trojan horse.

More about the presentation can be found here and here. 


## Software Development

### Scale Kuwait

**Title:** Scale Kuwait  
**Technology and tools used:** Django (Python) for the backend, Flutter (Dart) for mobile apps, PostgreSQL for the database, Docker for DevOps, React (JavaScript) for the website frontend, and RESTful API.  
**Links:** [Website](website_link), [Mobile Apps - Android](android_app_link), [Mobile Apps - iOS](ios_app_link)  
**Role:** Software Architect and Developer, including Deployment 
**Description:** This project focuses on establishing a comprehensive system for a food delivery startup. I’ve designed the software architecture and developed the whole system. The project is divided into several parts. 

* **Website backend:** Serving as the system's nucleus, the website follows a RESTful architecture pattern. Other subsystems communicate with the server via API endpoints. The server receives the API requests and returns the appropriate responses after executing the necessary computations. To mitigate potential security breaches, exclusive database access is granted solely to this backend.  A simplified diagram of the system architecture is shown in Fig 3. Pythons’ Django and PostgreSQL are used for the backend.

* **Mobile Apps:** The mobile apps are for the customer end. The apps allow customers to subscribe to a package and select their desired meal from a provided menu. Customer can pause their subscribed days using the app. Additionally, customers can monitor their nutritional intake, encompassing calories, carbs, fat, and proteins. These apps have been crafted for Android and iOS platforms using a cross-platform framework, Flutter.*



