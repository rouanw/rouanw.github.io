---
layout: post
title:  "Why should I hire a polyglot programmer?"
categories: code
---

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

What I'm essentially saying is that it doesn't matter whether the programmer you're considering has deep knowledge of the language or framework your system uses. But if that's what I'm saying, how on earth are you meant to decide whether a coder is up to the task? How do you know they'll be able to pick up C# and add value to your project without slowing you down?

###A very particular set of skills

Software engineering is about a lot more than the language or framework you're using. In my experience, the better developer to have on your team is often the one that understands fundamental software engineering practices, rather than the one with deep framework or language knowledge. Here's my take on skills a good polyglot programmer should possess:

####Automated testing
maintainability, extensibility

####Design
The D of TDD, OO, emergent design, refactoring

####Deployment
Configuration, automation

###Varied experience

Your new hire notices that the assertions the team is writing in their tesrs are a bit clumsy. They don't read very nicely and the error messages don't provide much detail when they fail. In her days of coding in Java, she used a library called Hamcrest that made assertions a) read more like English and b) give better errors. She asks herself "Surely there is something like that for .NET". She does a quick Google and finds a library called FluentAssertions. It does everything she wants from an assertion library. To her delight, it even has cleaner syntax than the Java library she has used before, because of C#'s extension methods.

She observes that the team deploys their application manually. She has automated a number of deployments in her time and thinks to herself that, even though there are more sophisticated tools available, even just a bash script is a great improvement over manually deploying things. She's has a Unix background though, so she doesn't know which tool is applicable. Again, she's off to Google for something she can use to script deployments on Windows. She comes across PowerShell. She starts writing some code to help automate the deployment. She starts with just copying some files across to the environment she wants to deploy to. The syntax is a bit clumsier than Bash, but a lot of it is the same. She hacks away and does a web search when she gets stuck on the syntax or conventions. Soon she has a script up and running that copies the application DLLs and she gets cracking on getting the web server to serve the updated files. She asks herslef whether there's a way to test Powershell, because she's written quite a bit of it now. She finds a testing framework called Pester and writes some tests. The team is taken aback. They've never even tried automating their deployment and some Windows newbie has just come and written scripts to do it in a Mircrosoft language. And she's written tests! Who knew you could test scripts?

### The right tool for the job

Knowing multiple languages allows the polyglot programmer to pick the right technology for the problem at hand. 

Part of the culture at [ThoughtWorks](http://www.thoughtworks.com) is to encourage developers to learn different languages. This is partially due to the fact that ThoughtWorkers tend to be quite geeky and like knowing lots of different languages, but is also due to the nature of the business. ThoughtWorks is a consulting company, which means that the languages we code in are most often influenced by the problems our clients are trying to solve. We use Java, Ruby, Python, Javascript, Clojure, C# and a host of other languages, depending on which language (or combination of languages) is best suited to the task at hand. We also often need to work within our clients' constraints. If they're a large organisation and all of their infrastructure runs Unix, it's unlikely that writing them a .NET application is going to be a good bet.

Most projects use multiple languages. No matter what the tech stack, modern applications often consist of a mix of languages. If you're writing a web application, it's very likely that you'll be writing some HTML, CSS and Javascript, whether you're building it using Rails or ASP.NET MVC. You might use a Python library like Fabric to deploy your Java application.

<div class="info-box">
	<h1>What is a polyglot programmer?</h1>
	The term <a href="http://en.wiktionary.org/wiki/polyglot">polyglot</a> refers to someone who is able to speak multiple languages. When I talk about a polyglot programmer, I'm talking about someone who is comfortable coding in multiple languages.
</div>
