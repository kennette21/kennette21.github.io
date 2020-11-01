---
layout: post
author: tom
tags: culture-blog soccer
---

# Lost in the coding sauce
## On a Saturday Morning

Reach a barrier, then overcome it. This is coding. Well, all progress through life, but I have learned this fact over and over again while working as a software developer in the last 3 years.

I am trying to gain a better understanding of full stack applications, cloud hosting/computing, and most of the concepts that tie modern web development together. I learn a fair amount at work, but so many of the systems are already built up that some of the complexity is hidden for me.

One strategy to learn more is to just work on personal projects. This portfolio is about publicising these projects. On the one had to have a place to showcase them, on the other hand to keep myself accountable with quality and progress. It is possible I have too many irons in the fire... However, I am optimistic that someday (hopefully soon) I will have a tenious grasp of each layer of the stack to the extent that I can throw together a PoC of almost any idea that comes to mind.

### current in-progress projects:
#### Culture Blog 
This is a really fun project. The concept is unique and it covers the idea I wanted to achieve with the explore portion of this portfolio. I would really like to get this out in production to iterate on it further.

What is needed for production deployment:
- figure out whether to use ORM (sequilize) or a Query Builder (knex) to properly model the DB
- connect the app to AWS RDS DB instance
- SETUP user creation using Passport and the ^^^ user model
- Dockerize the whole application
- Pull the docker app on an AWS instance.

#### Soccer Training Generation
This app is very simple. It just has a DB where you can store simple diagrams of traning drills. There are 4 categories of drills: warm-up, technical, mini-game (possession), finishing. 

All the app does is display one diagram from each category in a single page. This takes the planning out of sessions, and guarentees that sessiosn are simple and involve drills that are simple and effective.

I used this idea to learn a bit more about AWS EC2 creation and using Docker to develop on my machine then pull the image on the AWS instance. That learning was spectacular and very smooth. I had a very PoC application build and on AWS within an hour.

What is needed for production:
- atleast 2 diagrams for each category
- connect the app to AWS DB (i think DDB)
- React application added to current PoC


## Why Lost in the Sauce?
This morning there were many obsticals, and I did not have the conviction or focus to stay on one until it was overcome. I jumped from one obstical to another without sumiting any. The obsticals i was faced with today were:
- Sequelize or Knex for Culture Blog: how to setup, how to get it to work
- SSH tunneling to RDS instance in AWS: needed host, not sure if VPC was important
- Dockerizing Culture Blog/any BE/FE application with two package.jsons. Considered setting up React in soccer training Poc, but thats when i dropped the whole idea of coding today and started writing this post.

These are just theories:
1. I did not plan what to work on this morning. I did not have a clear goal. I kind of wanted to do some things in the culture blog, but that is kind of a mess. I kind of wanted to setup the RDS instance... 
##### takeaway:
have a clear goal that you can shoot for in a coding session.
2. Many irons in the fire detract from that clear goal.
##### takeaway:
One idea was to only focus on one project to completion.. Not a bad idea with this Soccer Training generator... Maybe try next week to compelte this generator.