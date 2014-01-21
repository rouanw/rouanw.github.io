---
layout: post
title:  "Why should I hire a polyglot programmer?"
categories: code
---

People are often sceptical of software developers with varied coding experience. They're used to seeing

	5 years Java experience
	
on the CV in front of them, so when they see the CV that says

	3 years Ruby experience
	1 year Python experience
	1 year C# experience

they're concerned that the person doesn't have the skills required for the job. I'm going to argue that this reaction, although natural, is misguided. I contend that it's very possible that the person with the second CV will be a better developer on a Java project, despite having little or no Java experience.

# An example

I was on a project not too long ago, where the technology stack was .NET. The team from the client we were working with were seasoned .NET developers. Their experienced ranged from about 5-15 years. Enter one of our consultants, with a number of years of experience under his belt, but with no .NET experience at all. If I remember correctly, his background was mainly Ruby and Java.

Despite the scepticism of the team, he was able to pick C# up really quickly. And was able to not only keep up with the team, but teach them many new things. Let's have a look at why.

# If languages don't matter, what does?

What I'm essentially saying is that it doesn't matter whether the programmer you're considering has deep knowledge of the language or framework your system uses. But if that's what I'm saying, how on earth are you meant to decide whether a coder is up to the task? How do you know they'll be able to pick up Java and add value to my project without slowing us down?

##Core concepts

##Varied experience

Our consultant notices that the assertions the team is writing in their tesrs are a bit clumsy. They don't read very nicely and the error messages don't provide much detail when they fail. In his days of coding in Java, he used a library called Hamcrest that made assertions a) read more like English and b) give better errors. He asks himself "Surely there is something like that for .NET". He does a quick Google and finds a library called FluentAssertions. It does everything he wants from an assetion library. To his delight, it even has cleaner syntax than the Java library he has used before, because of C#'s extension methods.

Our consultant notices that the team deploys their application manually. He has automated a number of deployments in his time and thinks to himself that, even though there are more sophisticated tools available, even just a bash script is a great improvement over manually deploying things. He's a Unix guy though, so he doesn't know which tool is applicable. Again, he's off to Google for something he can use to script deployments on Windows. He comes across PowerShell. He starts writing some code to help automate the deployment. He starts with just copying some files across to the environment he wants to deploy to. The syntax is a bit clumsier than Bash, but a lot of it is the same. He hacks away and does a web search when he gets stuck on syntax or convention. Soon he has a script up and running that copies the application DLLs and he gets cracking on getting the web server to serve the updated files. He asks himself whether there's a way to test Powershell, because he's written quite a bit of it. He finds a testing framework and writes some tests. The team is taken aback. They've never even tried automating their deployment and some Unix guy has just come and written scripts to do it in a Mircrosoft language. And he's written tests! Who knew you could test scripts?

## The right tool for the job

Knowing multiple languages allows the polyglot programmer to pick the right technology for the problem at hand. 

Part of the culture at [ThoughtWorks](http://www.thoughtworks.com) is to encourage developers to learn different languages. This is partially due to the fact that ThoughtWorkers tend to be quite geeky and like knowing lots of different languages, but is also due to the nature of the business. ThoughtWorks is a consulting company, which means that the languages we code in are most often influenced by the problems our clients are trying to solve. We use Java, Ruby, Python, Javascript, Clojure, C# and a host of other languages, depending on which language (or combination of languages) is best suited to the task at hand. We also often need to work within our clients' constraints. If they're a large organisation and all of their infrastructure runs Unix, it's unlikely that writing them a .NET application is going to be a good bet.

Most projects use multiple languages. No matter what the tech stack, modern applications often consist of a mix of languages. If you're writing a web application, it's very likely that you'll be writing some HTML, CSS and Javascript, whether you're building it using Rails or ASP.NET MVC. You might use a Python library like Fabric to deploy your Java application.

#Notes

The term [polyglot](http://en.wiktionary.org/wiki/polyglot) refers to someone who is able to speak multiple languages. When I talk about a polyglot programmer, I'm talking about someone who is able to code in multiple languages. So, if Sue is a programmer who is comfortable coding in (say) Javascript, Ruby and Java, I'd feel okay about calling her a polyglot programmer.