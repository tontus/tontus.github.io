---
layout: page
title: portfolio
permalink: /portfolio/
nav: true
nav_order: 7
---

# Table of Contents

- [Research Publication](#research-publication)
- [Presentation](#presentation)
- [Software Development](#software-development)
  - [Scale Restaurant](#1-scale-restaurant)
  - [Talking Planets](#2-talking-planets)
  - [Hunting Flashcards](#3-hunting-flashcards)
- [Other Projects](#other-projects)
  - [Cyber Adventures of Deep](#1-cyber-adventures-of-deep)

## Research Publication

**Title:** A cognitive behaviour data analysis on the use of social media in the global south context focusing on Bangladesh  
**Paper link:** [Read the Paper](https://www.nature.com/articles/s41598-023-30125-w) https://doi.org/10.1038/s41598-023-30125-w  
**Role:** Null hypothesis formulation, Survey design, data collection & analysis, writing manuscript

**Description:** This research is an extension of my undergrad thesis, “Why do we share fake news?”. In this research, my two teammates and I investigated the human factors that may influence someone to spread misinformation regarding COVID-19 vaccination on social media. After surveying literature from various disciplines, including Philosophy, Psychology, and Computer Science, we formulated several null hypotheses about the pattern of misinformation propagation. We were struggling to find a suitable way to capture the interactions of individuals with fake news. I started reading about other papers to find a way to collect this kind of data. I designed an experiment that can capture and quantify the participants' interactions with a piece of false news in a controlled environment. After collecting some demographic information about the participants, we supplied them with some fabricated news as stimuli about the problems related to COVID-19 vaccines displayed from usually acclaimed sources in Bangladesh. We asked a series of questions related to them. All the survey takers were supplied with the same fabricated news from the same sources to reduce bias. The questions we asked ranged from how it made them concerned about their friends and families to how desperate they were to share these as soon as they finished the survey. We used Likert scales with 7 points to collect data ranging from strongly negative (1) to strongly positive (7). Some examples of the supplied fabricated news are given in Fig. 1 & 2. Those were created by me using Photoshop. Later in the survey, we clarified to the participants that the news was crafted and not actual.

{% include figure.html path="assets/img/portfolio/fig1.png" class="img-fluid" caption="Fig 1: Fabricated news from a renowned english news outlet, The Daily Star in Bangladesh"%}


{% include figure.html path="assets/img/portfolio/fig2.png" class="img-fluid" caption="Fig 2: Fabricated news from another renowned english news outlet, The Dhaka Tribune in Bangladesh"%}


After collecting and cleaning those data by removing reponses that were invalid, we were left with 206 responses. Then, with the instructions of the project supervisor, I began analyzing the data. I used the Chi-square test and the Spearman Rank Correlation Coefficient to measure the correlation between features and applied Ordinal Logistic Regression to see how the features were related. I used pythons’ pandas, numpy, scipy, seaborn and matplotlib libraries to analyze and visualize these data.

We observed several interesting trends through our research. For example, individuals spending more than 5 hours per day on social media were more likely to spread the false information provided to them compared to users who spent around 2 hours. Additionally, individuals are more likely to share information without verification that originates from a source with whom they have a personal relationship.

Later, we published our research in Scientific Reports. I contributed to writing the manuscript of the paper.

## Presentation

**Title:** Gamification of ICT textbook material to provide an interactive learning experience  
**Venue:** [CHI 2023 Virtual Workshop hosted by HCI4SouthAsia (remote)](https://hci4south.asia/workshop-chi-2023/)  
**Role:** Idea generation and presentation

**Description:** I presented a half-baked idea of a project of gamification of Bangladesh ICT textbook content to provide an interactive learning experience to underprivileged students. This project aims to provide digital literacy to disadvantaged students who don’t have access to the internet and digital devices and prepare them for the upcoming digital world. To make this game effective and engaging, 3 learning principles will be followed. These are (1) **Interest-powered learning**, (2) **Peer-supported Learning**, and (3) **Relevance of learning content.**

- **Interest-powered learning:** To make the game more engaging for our targeted age group, we will create an interface that simulates a real-life scenario. The interface will be designed to resemble an email inbox and school portal. In this game, the students will act as assistants in a lab. Their job will be to read, reply, and follow the instructions provided in the email address. That instruction may include uploading data or files with their credentials on the school portal and having video calls with other lab members. Some emails may contain spam or phishing content, and students’ tasks will be to identify and avoid those malicious situations.

- **Peer-supported learning:** This game will be designed as a multiplayer game. Each student will have both individual and group tasks. For instance, a task may require one student to read an email and send the right data file to another lab member. After that, the second lab member will receive and upload the data to complete the group task. Inside the game, the students can communicate with each other over the internet to solve any challenges that may arise. This will help strengthen their online collaboration skills. 

- **Relevance of learning content:** The game’s content will be related to the student’s coursework to aid their understanding. Class 8-10 ICT curricula contain the above-mentioned topics. The content will be embedded within an enjoyable and exciting gameplay, acting as a Trojan horse.

More about the presentation can be found [here](https://drive.google.com/file/d/1fEBKUUiBCHnBLnFProgXMqacBcOyZCmV/view) and [here](https://docs.google.com/presentation/d/1ivirRIgMqAfxFcqjR5fTKt4HRihVuT2pvhOu5mDWPDg/edit?usp=sharing).

## Software Development

### 1. Scale Restaurant

**Title:** Scale Restaurant  
**Technology and tools used:** Django (Python) for the backend, Flutter (Dart) for mobile apps, PostgreSQL for the database, Docker for DevOps, React (JavaScript) for the website frontend, and RESTful API.  
**Links:** [Website](https://scale-kuwait.com/), [Mobile Apps - Android](https://play.google.com/store/apps/details?id=com.scaleKuwait.app), [Mobile Apps - iOS](https://apps.apple.com/us/app/scale-restaurant/id1583414026)  
**Role:** Software Architect and Developer, including Deployment.

**Description:** This project focuses on establishing a comprehensive system for a food delivery startup. I’ve designed the software architecture and developed the whole system. The project is divided into several parts.

* **Website backend:** Serving as the system's nucleus, the website follows a RESTful architecture pattern. Other subsystems communicate with the server via API endpoints. The server receives the API requests and returns the appropriate responses after executing the necessary computations. To mitigate potential security breaches, exclusive database access is granted solely to this backend. A simplified diagram of the system architecture is shown in Fig 3. Pythons’ Django and PostgreSQL are used for the backend.

<div style="text-align: center;">
{% include figure.html path="assets/img/portfolio/fig3.png" class="img-fluid" caption="Fig 3: System architecture of the project"%}
</div>

* **Mobile Apps:** The mobile apps are for the customer end. The apps allow customers to subscribe to a package and select their desired meal from a provided menu. Customer can pause their subscribed days using the app. Additionally, customers can monitor their nutritional intake, encompassing calories, carbs, fat, and proteins. These apps have been crafted for Android and iOS platforms using a cross-platform framework, Flutter.

{% include figure.html path="assets/img/portfolio/fig4.png" class="img-fluid" caption ="Fig 4: Screenshots of the mobile apps"%}
  
* **Admin Dashboard:** The admin dashboard is for internal usage. The management team can generate various company reports, such as sales and orders. They can also update the menu, manage use subscriptions, update dishes from this website, print info stickers, and manage delivery queue. The website's front end is made with React, which uses API to communicate with the central backend.

* **Testing Environment:** A meticulous testing environment to test new features before making it public. It is a replica of the live system, ensuring robust feature testing.

* **DevOps:** I used docker in the Ubuntu server for the deployment. To make deployment seamless, I’ve installed some automation.


### 2. Talking Planets

**Title:** Talking Planets

**Technology and tools used:** Flutter for mobile app and DialogFlow for chatting. 

**Links:** [Android app](https://play.google.com/store/apps/details?id=app.talking.planets&hl=en&gl=US)

**Role:** Software Development, UI/UX direction.

**Grants:** [We received a grant of 8000 Euro from the International Astronomical Union](https://www.astro4dev.org/category/astronomy-for-students-through-interactive-app-and-game/)

**Description:** Our team, Pothikrit, developed an interactive astronomy app to popularize astronomy and science education among the young generation in Bangladesh and worldwide. It aims to increase awareness of astronomy and reduce the knowledge gap between high-income and low-income communities. Students will also learn about pressing challenges, such as climate change, through the lens of astronomy.

We used Flutter to build the apps. Custom-trained DialogFlow was used for chatting with planets. This app supports Bengali and English, and we plan to include more languages. Custom-made graphics and animations made the app enjoyable to our target audiences. We received Astronomy for Development Grants funded by the Office of Astronomy for Development of the International Astronomical Union for this project.

<div style="text-align: center;">

{% include video.html path="assets/video/portfolio/figure5.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true max-height="250px" caption="Fig 5: Talking Planets app" %}

</div>


### 3. Hunting Flashcards

**Title:** Hunting Flashcards  
**Technology and Tools Used:** Flutter for mobile app  
**Link:** [iOS app](https://apps.apple.com/de/app/lernkarten-jagd/id1600091122)  
**Role:** Software Development  

**Description:** Hunting Flashcards is an iOS app that was made for a client using Flutter. The user of the app can learn different traits of various animals. Embedded latex was used to display equations inside the app.

<div style="text-align: center;">

{% include video.html path="assets/video/portfolio/fig6.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true max-height="250px" caption="Fig 6: Hunting Flashcards app" %}

</div>

## Other Projects

### 1. Cyber Adventures of Deep

**Title:** Cyber Adventures of Deep  
**Award:** [Champion in ‘Digital Khichuri Challenge-2019’](https://www.undp.org/bangladesh/press-releases/digital-khichuri-challenge-peaceful-and-inclusive-society-accelerating-progress-sdgs)  
**Role:** Idea generation, Presentation, Video editing  

**Description:** This was a national-level hackathon organized by the United Nations Development Programme (UNDP) and supported by Facebook and the ICT ministry in Bangladesh. The competition's goal was to find a way to promote harmony and peace in online social media. Our team won the first prize for creating an idea for an engaging game to teach teenagers to identify misinformation quickly. Also, making them aware of spreading fake news on social media has severe real-life consequences. The teaser of the game is given below. I used Adobe After Effects to animate and Procreate to draw graphics for this teaser. 


<div style="text-align: center;">

{% include video.html path="https://www.youtube.com/embed/IkbiYvM4Sao?si=-RioOuh2O5cRe4IN" class="img-fluid rounded z-depth-1" controls=true autoplay=true max-height="315px" caption="Fig 7: Cyber Aventure of Deep | Teaser" %}

</div>
