---
layout: post
title:  Why should I hire a polyglot programmer?
tags: languages engineering_practices
---

The term [polyglot](http://en.wiktionary.org/wiki/polyglot) refers to someone who is able to speak multiple languages. When I talk about a polyglot programmer, I'm talking about someone who is comfortable coding in multiple languages.

People are often sceptical of software developers with varied coding experience. They're used to seeing

	5 years C# experience
	
on the CV in front of them, so when they see the CV that says

	2 years Ruby experience
	1 year Python experience
	2 years Java experience

they're concerned that the person doesn't have the skills required for the job. I'm going to argue that this reaction, although natural, is misguided. I say that the person with the second CV might well be a better developer on a C# project, despite having little or no C# experience. As you read on you'll see that I'm not talking about any developer who happens to know a few languages, but a particular kind of polyglot programmer (with a very [particular set of skills](http://www.youtube.com/watch?v=B0hZ1KKpV54)).

Let me set the scene. Your organisation's technology stack is .NET. Your development team is a group of seasoned .NET developers. Their experience ranges from about 5-15 years. Let's say you hire the person with the second CV. She has a number of years of experience under her belt, but no .NET experience at all.

Despite the scepticism of the team, she is able to pick C# up really quickly. She is not only able to keep up with the team, but ends up teaching them many new things. Let's have a look at why.

## If languages don't matter, what does?

What I'm essentially saying is that it doesn't matter whether the programmer you're considering has deep knowledge of the language or framework your application uses. But if that's what I'm saying, how on earth are you meant to decide whether a coder is up to the task? How do you know they'll be able to pick up C# and add value to your project without slowing you down?

###A very particular set of skills

Software engineering is about a lot more than the language or framework you're using. In my experience, the better developer to have on your team is often the one that understands fundamental software engineering practices, rather than the one with deep framework or language knowledge. Here's my take on skills a good polyglot programmer should possess:

####Automated testing

The two aspects that most often go wrong on software projects are maintainability and extensibility. This is often due to bad design, which we'll talk about in a moment. Irrespective of how your software is designed, though, if it is not tested, you're going to struggle. Automated tests are a living specification of an application's behaviour. When we want to modify the application, it is the tests that guide us and help us to understand how the changes we are making impact the application's behaviour. Automated tests stop bugs before they hit production, as they are coded, so that we have fewer maintenance issues in production. Automated tests help us to ensure that we're not breaking existing functionality when we add new features.

A developer who understands the importance of testing and knows how to write good tests will be an invaluable asset to your team. They should know how to write functional tests (so that they can protect your features), how to write unit and integration tests (to ensure that the internal structure of your application is sound) and how to practise Test Driven Development (so that your application is fully tested and well designed).

Automated give us confidence that our software does what it's meant to. The developer you hire should understand this and ensure that testing is a first class consideration in your development process. Developers who are passionate about testing tend to be intolerant of those who are not. Given your support, expect your new hire to quickly get the rest of the team writing tests.

####Design

Many of my colleagues prefer to call TDD Test Driven *Design*. I like this because it highlights that writing your tests before your code is more a design activity than a development activity. When you write your tests first, you grow the components of your application from the perspective of a consumer, which means that a focus on its design is baked in from the start. A good polyglot programmer understands this. They don't neglect the refactoring step that forms an often ignored part of TDD, in order to make sure your application takes on a sensible shape. 

It is this constant refactoring that we refer to as emergent design and is all about making sure that the design of the program we are writing evolves in a way that is easily maintainable and extensible. When I talk about design, I'm not thinking of UML diagrams or planning out the details of the application in advance. I am talking about an awareness of what good code looks like and ensuring that the team is constantly making the small changes required to ensure that the code stays good.

The polyglot programmer you want to hire will understand emergent design, understand object oriented programming and  know how to refactor code to be easier to work with.

####Deployment

Your software is useless unless it is in production. No matter how innovative the features are that you've developed, no matter how confident you are that it does what it's meant to and no matter how well designed it is, if a user cannot use it, it is useless.

A good developer will know how to deploy applications. They should understand how to configure the applications so that they work in the right way. Very importantly, they should know how to automated the configuration and deployment of your application. Without automated deployments, you will always struggle to put your organisation's new ideas (and the hard work of your development team) in front of your users. Without automated deployments, your application's infrastructure will become mysterious and unpredictable.

When you hire a developer who knows how to help you automate the deployment and configuration of your applications, you gain the potential to move quickly on new ideas and gain the confidence that your application can recover from disasters.

###Varied experience

Your new hire notices that the assertions the team is writing in their tests are a bit clumsy. They don't read very nicely and the error messages don't provide much detail when they fail. In her days of coding in Java, she used a library called Hamcrest that made assertions a) read more like English and b) give better errors. She asks herself "Surely there is something like that for .NET". She does a quick Google and finds a library called FluentAssertions. It does everything she wants from an assertion library. To her delight, it even has cleaner syntax than the Java library she has used before, because of C#'s extension methods.

She observes that the team deploys their application manually. She has automated a number of deployments in her time and thinks to herself that, even though there are more sophisticated tools available, even just a bash script is a great improvement over manually deploying things. She's has a Unix background though, so she doesn't know which tool is applicable. Again, she's off to Google for something she can use to script deployments on Windows. She comes across PowerShell. She starts writing some code to help automate the deployment. She starts with just copying some files across to the environment she wants to deploy to. The syntax is a bit clumsier than Bash, but a lot of it is the same. She hacks away and does a web search when she gets stuck on the syntax or conventions. Soon she has a script up and running that copies the application DLLs and she gets cracking on getting the web server to serve the updated files. She asks herself whether there's a way to test Powershell, because she's written quite a bit of it now. She finds a testing framework called Pester and writes some tests. The team is taken aback. They've never even tried automating their deployment and some Windows newbie has just come and written scripts to do it in a Microsoft language. And she's written tests! Who knew you could test scripts?

The polyglot programmer brings with them an invaluable breadth of experience. They will open your team's eyes to the development practices and tools that are common in other languages.

###The right tool for the job

Knowing multiple languages allows the polyglot programmer to pick the right technology for the problem at hand. 

Not all applications are the same. The problems they seek to solve, or the opportunities they seek to leverage, are vastly different. Why should you care? Because different jobs require different tools. Software built on the wrong technology stack is ugly and painful. Why are you using Java to solve a clearly functional problem? Maybe you should be using Clojure instead. Why are you building a plain Rails app when your users are complaining that they need a more fluid interface? Maybe you should be using a single page Javscript framework.

No matter what the tech stack, modern applications often consist of a mix of languages. If you're writing a web application, it's very likely that you'll be writing some HTML, CSS and Javascript, whether you're building it using Rails or ASP.NET MVC. You might use a Python library like Fabric to deploy your Java application. You might have a fat Javascript front end that talks to a web server written in Ruby.

The polyglot programmer you hire should be able to use to breadth of their experience to help you make smart decisions about which technology to use.

##I'm sold! Where do I find one?

Finding good developers is not easy at the moment. Bad development practices are widespread (and often encouraged) in the industry. If you find a developer who matches the criteria I've described in this post, snap them up! Remember to look past their experience in your language or framework on their CV - otherwise you will miss out on a positive influence on your team.

My parting shot will be to say that, if you can't find a good polyglot programmer, you have the power to create one! Encourage your development team to broaden their skill set, give them the time to experiment with new languages, frameworks and tools. And, most importantly, make sure you're helping them build that very particular set of skills. Those skills that differentiate a great developer from a decent one, no matter which language they're coding in.
