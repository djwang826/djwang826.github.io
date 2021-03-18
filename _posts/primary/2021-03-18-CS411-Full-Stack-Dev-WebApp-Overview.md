---
layout: post
title: CS411 Full Stack Web App Overview
---

An overview of a full stack web application built from scratch for my CS411 Software Engineering course.

[Github repository link](https://github.com/omeedth/411_Project)

**Requirments**

1. Database
2. Two APIs
3. Third-party authentication

**The Idea**

Before we could start the web app, we had to decide what to create. We proposed to the professor a travel aid app that would help find the cheapest transportation to your desired location along with helping you decide the best locations to visit depending on your preferences. The full proposal of our idea is attached below.

> Our application will essentially be a travel aid. We will use data from sites such as hotels.com, Airbnb, Hertz, Zipcar, and Google flight 
> search to provide information about the best deals on places to stay and modes of transportation in/to the user’s destination of choice. 
> We will also pull data from the user’s Facebook or Instagram account in order to generate a list of places they might be interested in 
> visiting within the city/region they are visiting. We will use TripAdvisor to pick the highest rated locations and to provide information 
> on entry fees, etc. Additionally, we will tell the user what form of transportation will be the least expensive and most convenient for 
> travelling to the attractions we’ve gathered for them (such as ride-sharing, rental bikes, or the metro/bus). We will use the user’s 
> Google login information as our third-party authenticator. Users will be required to create a profile within the application. 

**The Tech Stack**

The original stack was MERN (MongoDB, Express, REACT, and NodeJS), but the database was later changed to Cloud Firestore. Our full explanation of the tech stack is attached below.

> We are using Cloud Firestore, Express, REACT, and NodeJS (a slight modification of the MERN stack). We chose this technology 
> stack because we think it works best for web-based applications, especially since NodeJS and MongoDB mesh together very well. 
> REACT is being used for the  front end because we wanted to learn a new front end application. We originally wanted to use MongoDB
> but eventually decided to use Cloud Firestore instead. No one on our team had any experience with MongoDB so integrating it into our 
> app was going to be difficult. Firestore, a Google product, came with clear instructions and was very easy to work with. We also 
> considered using Python with Flask and MySQL for the database, but we figured those would be much messier to integrate. This is because
> MySQL is used for more enterprise related websites/databases. We also decided against Flask because when we thought about web applications
> JavaScript was the first thing to come to mind, and not Python/Flask.

**User stories and Sequence Diagrams**

After determining the idea and the tech stack, we wrote three user stories that described the possible actions a user would be able to do on the web app. The goal of this was to use the stories as a guide during development. You can read the stories in the documentation folder in the Github repo.

We then created the sequence diagram for the 'happy path', which is essentially the path where the user does exactly what should be done when navigating the app, and nothing breaks.

![SequenceDiagram](/images/SequenceDiagramforUserStory2.png)

**Implementation**

Setup and installation of the components was fairly simple, along with setting up the repository on Github. After browsing the available APIs, we decided on the Amadeus and Yelp Fusion APIs. We used the Amadeus API to find the cheap flights and the Yelp Fusion API to find tourist attractions. We also decided to use Facebook to fulfill the third party Oauth requirement - the users would log in using Facebook and their credentials stored in the database. We also divided up the tech stack so each member could focus on one specific part, although we kept each other updated on what we did so everyone would understand the whole tech stack. I was assigned the front end, and created the interface using REACT and material-ui, as shown below.

![FrontPage](/images/CS411pic1.png)

The full code for the page can be seen in the GitHub repo.

I was also in charge of the API's, and parsing the data returning from the requests. The data needed was buried pretty deep within the POST data sent back, but I was able to find it. But after displaying the data, the numbers refused to be properly formatted into a list or a table, so I ultimately had to leave it as shown above, as I had run out of time.

The API was tested beforehand with Postman to make sure we used the best requests to get the data we needed. For Amadeus, we used the 'lowfare' request to get the cheapest fare for the two locations. For Yelp, we used the 'business search' request and displayed the top rated businesses in the destination.

**Submission and Grade**

At the end of the semester, we submitted the web application with the above components finalized and received a grade of A.