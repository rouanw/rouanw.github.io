---
layout: post
title: A very particular set of skills
tags: engineering_practices
---

In the movie *Taken*, Liam Neeson's character talks about the very [particular set of skills](http://www.youtube.com/watch?v=B0hZ1KKpV54) that he posesses. Although his skills are a bit more sinister than I hope most developrs have, I believe that the good software developer also posesses a particular set of skills that place them a cut above their ordinary counterparts. A good developer has a solid understanding of some fundamental engineering practices. This post is an attempt at articulating my take on what these are.

##Automated testing

The two aspects that most often go wrong on software projects are maintainability and extensibility. This is often due to bad design, which we'll talk about in a moment. Irrespective of how your software is designed, though, if it is not tested, you're going to struggle. Automated tests are a living specification of an application's behaviour. When we want to modify the application, it is the tests that guide us and help us to understand how the changes we are making impact the application's behaviour. Automated tests stop bugs before they hit production, as they are coded, so that we have fewer maintenance issues in production. Automated tests help us to ensure that we're not breaking existing functionality when we add new features.

A developer who understands the importance of testing and knows how to write good tests will be an invaluable asset to your team. They should know how to write functional tests (so that they can protect your features), how to write unit and integration tests (to ensure that the internal structure of your application is sound) and how to practise Test Driven Development (so that your application is fully tested and well designed).

Automated tests give us confidence that our software does what it's meant to. The developer you hire should understand this and ensure that testing is a first class consideration in your development process. Developers who are passionate about testing tend to be intolerant of those who are not. Given your support, expect your new hire to quickly get the rest of the team writing tests.

##Design

Many of my colleagues prefer to call TDD Test Driven *Design*. I like this because it highlights that writing your tests before your code is more a design activity than a development activity. When you write your tests first, you grow each component of your application from the perspective of a consumer, which means that a focus on its design is baked in from the start. A good  programmer understands this. They don't neglect the refactoring step that forms an often ignored part of TDD, in order to make sure your application takes on a sensible shape. 

It is this constant refactoring that we refer to as emergent design and is all about making sure that the design of the program we are writing evolves in a way that is easily maintainable and extensible. When I talk about design, I'm not thinking of UML diagrams or planning out the details of the application in advance. I am talking about an awareness of what good code looks like and ensuring that the team is constantly making the small changes required to ensure that the code stays good.

The programmer you want to hire will understand emergent design, understand object oriented programming and  know how to refactor code to be easier to work with.

##Deployment

Your software is useless unless it is in production. No matter how innovative the features are that you've developed, no matter how confident you are that it does what it's meant to and no matter how well designed it is, if a user cannot use it, it is useless.

A good developer will know how to deploy applications. They should understand how to configure the applications so that they work in the right way. Very importantly, they should know how to automate the configuration and deployment of your application. Without automated deployments, you will always struggle to put your organisation's new ideas (and the hard work of your development team) in front of your users. Without automated deployments, your application's infrastructure will become mysterious and unpredictable.

When you hire a developer who knows how to help you automate the deployment and configuration of your applications, you gain the potential to move quickly on new ideas and gain the confidence that your application can recover from disasters.