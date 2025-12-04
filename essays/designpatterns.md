---
layout: essay
type: essay
title: "Experience with Common Design Patterns"
# All dates must be YYYY-MM-DD format!
date: 2025-12-03
published: true
labels:
  - Software Engineering
  - Design Patterns
  - ICS
  - Final Project
---

## My Introduction to Design Patterns
Before the module, I had never heard of design patterns before in the context of software engineering. Although just based on the name, I thought of it like the template or approach people use for their application so that it is something that anyone within the project can easily adapt to and recognize. The roof design on houses really deepened my understanding of how important design patterns are because one design pattern does not apply to every situation, and you have to be experienced enough to recognize which patterns are the most appropriate for the assignment you are tasked with. 

I definitely understand why design patterns are important for developers and designers because understanding each different design pattern really helps organize and simplify complex systems. Especially when collaborating with other people, signifying what design patterns you are using can definitely help people understand what kind of system you are working with, and they are able to understand the architecture of your program and know what is necessary for the project. I believe that the best way to explain what design patterns are is to think of them as strategies and concepts that have been used and tested for so long that they are generally very safe solutions based on problems that occur regularly within software development. 

## Design Patterns Implemented in WarriorHub Final Project
My group’s final project is called Warriorhub, which is designed to be an all-in-one application for UH Manoa students to view all campus events on a single application and be able to save events that they are interested in within a My Events page. I was interested to find out that even though I did not know what design patterns were before this current module, we have already implemented many of these well-used design patterns within our project. MVC may be one of the biggest design patterns that we are using because we are representing models that hold user data, event data, organizer data, interested event relationships, and event calendar. Viewers can see the landing page, login, event search, calendar view, and my events page, while admins/organizers have the functionality to create events, which ties into controllers where organizers and admins can change or add events, while users can add interested events into their my events page and update the views. 

The factory design pattern is also one that I found pretty straightforward since all events in our application are created on the same form and follow a specific process where organizers and admins add a name, location, time of event, description, image, and related categories to an event. This consistent structure is closely related to the factory design pattern, which I understand to be a standardized way to create objects. 

The singleton design pattern, to my basic understanding, is implemented within our project and everyone else’s because we are using only one database to coordinate all of our actions across the application. Lastly, the observer pattern is really important for any responsive application and our final project because the requirements we made for our project demonstrate that our application will populate all events into the calendar page whenever an event is created. Users may select events that they are interested in, and they will then populate into their My Events page for them to view, and newly created events will also immediately be added into the Search Events page. 

These design patterns are very fundamental to any application that is being implemented and developed, but I am also learning to avoid anti-patterns such as the Lava Flow anti-pattern because I can understand how easily it is to accidentally fall into these habits. While working on Warriorhub, there were a few instances where I wasn’t completely familiar with the logic other team members put into API files or DB actions. The code logic wasn’t old or unused, but I sometimes found myself afraid to touch these files when the program itself was working very smoothly because of my fear of breaking it. After a lot of time spent double-checking, rewriting code, and checking in with other members, I was able to complete whatever task was assigned to me. Although I can see how difficult it may be when you don’t have a team that is familiar with code logic that was implemented long before you arrived to work on a project. 

