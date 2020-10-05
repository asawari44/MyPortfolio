---
title: "Internet protocol design"
date: 2019-03-20T12:14:34+06:00
image: "images/portfolio/item-4.png"
client: "Aalto University course work"
project_url : "https://github.com/asawari44/IP_final_assignment"
categories: ["Development"]
description: "It was an assignment designed by the Aalto University course called Internet protocols. The objective was to understand the designing process and working of different protocols."
draft: false
---

#### Project Requirements
In automated vehicular systems, if one vehicle needs to overtake the other, a video stream from other vehicles approching it in the same lane needs to be processed and the decision of overtaking or changing the lane has to be made on the basis of other vehicles on the vicinity. 

The objective was to set up a streaming protocol to view continuos video steam and simulate the scenario. Based on the processed data, we had to develop an algorithm that states when is the best time to cross the lane for a vehicle.
#### Project Details
We used docker containers for simluating vehicles and rabbitmq as the message handling queque/ broker. Each container would behave as a producer and send a video stream to the message broker. The broker stores metadata related to the frame of the video and sends it to all the subscribed vehicles. When a vehicle needs to cross the lane it would subscribe to the broker and start getting video streaming from the producer vehicles within the radius of 500m. Based on the received data, the algorithm calculates the current speed of the approaching vehicle and calculates the right time to cross the lane.

