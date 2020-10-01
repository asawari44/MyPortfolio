---
title: "Summer Intern Assignment(open source)"
date: 2019-05-12T12:14:34+06:00
image: "images/portfolio/item-3.png"
client: "Eficode"
project_url : "https://github.com/asawari44/EficodeAssignment"
categories: ["Development"]
description: "Eficode had announced an assignment for their summer internship program, the hiring process stopped due to Covid-19, but I got an opportunity to work on the assignment and publish it on my GitHub."
draft: false
---

#### Project Requirements

The assignment was provided by Eficode, Helsinki for a summer job, which involved creating a webpage / website that can show employees bus/ metro/ trams timings in order to reach a certain destination in time. The required technology stack involved, GraphQL as a query language, HSL open data interface, Website designing and building, deploying the website on any platform of choice and unit testing with robot framework. 

#### Project Details

I created a website using python flask webserver and used HSL open data interface to fetch bus timings and other related information such as location and bus hops, etc. I used GraphQL to query the returned response by the interface and used HTML/CSS/JS to set the response in a descent UI. 
I created docker image to containerize my website and I deployed it on an AWS EC2 instance. 
