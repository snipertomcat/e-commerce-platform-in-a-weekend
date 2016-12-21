## Pre-Requisites

There are some requirements (prerequisites) that this book assumes you, the reader, already are familiar with:

* You know how to code basic php
* You know the standard request/response model for web applications
* You want to learn strong foundations that make e-commerce platforms work

That is really it... We will be creating a test server in the beginning so we have a place to write code and run what we have written in a web browser to see the results. I will be going over the request/response model briefly so if you are not too familiar with that concept, but a basic knowledge of php code is mandatory--otherwise, you'r going to find it difficult to keep up the pace of the content. I assume you know how to write a basic php program and run it in the browser and via command line. I also expect you to know:

* PHP superglobals ($_POST, $_GET, etc)
* How html and php pass data around (with forms)
* How to write html, css and javascript at an intermediate level

## Goals of this book

The goals of this book are to:

* Familiarize you with basic web applications components
* Introduce you to the standard business entities involved in an e-commerce system
* Utilize 3rd party software and libraries to avoid "re-inventing the wheel"
* Design and build a basic but functional e-commerce web application

## Setting up the application's core functionality

Part I of this book will be dedicated to configuring our development environment and local test server, as well as building out the most common functionality present in any modern day web application. This code will either be our own (handwritten), vendor packages made available via composer, or glue code that will tie in vendor software into our application so that we may use it. It will serve as the core platform for which all other components in our application will utilize or expand.

Basically the idea is to show you what a web application consists of by breaking down the concept into its various components. Throughout the book, we will be discussing how these individual components all fit together to form a functional application and how things like routing, user authentication, security, and other facets can be put into place by pre-existing open source code. We will use this knowledge to select various pre-built components so that we don't have to re-do the standard functionality found in most modern day web applications (a process called "re-inventing the wheel"). To name a few, we will be installing and using:

* Symfony's Routing component
* TWIG template engine 
* Facades and Interfaces from the Laravel framework
* various other packages

We will manage all our 3rd party code with a package manager called Composer. Although composer has an easy going learning curve, it is widely used in the web development world and is the de-facto in package management. 

During the time you are learning these basic pieces of an application you will be writing real code. That's right! We are going to start coding right off the bat and this is why this book in particular is different... Most of the time, there is a large learning overhead that must be taught before any actual coding happens. Quite the contrary, this book teaches you what you need to know _while_ teaching you how to code. The concepts that I portray in this book all are made real through code and all the work you do _while_ learning these concepts are all going to be part of the resulting application at the end.

## Develop an intricate understanding of e-commerce systems

To understand how to build an e-commerce software system, you have to not only know e-commerce but also understand it intimately and identify the different entities in a basic online store as well as their relationships to each other. In Part II we will introduce e-commerce systems and how the concepts of real world commerce must all be taken into account in order to design a proper software architecture (that would be the "e" in e-commerce). The basic concepts of a brick and mortar store are essential to know and understand before any data model can be created in code that represents a store. Among these are:

* Products
* Categories
* Orders
* Carts
* Customers
* Shipping/Delivery information
* Payments

We will be translating each of these entities from how we know them to be in real life to models used in the application. This is done by creating a database schema that corresponds to what we know a real live _store_ to be. Each data model in the domain will correspond to an entity in an e-commerce system. It is here that we will build out our models and, by the end of the section, have created and deployed a live mysql database to hold everything!
 
## Tie everything together and build out our application

Now that we have gone over all crucial concepts and details of our software, we can finally start writing the application's core processes. By this point we will already have a firm understanding of what an e-commerce system is, what it does, and the different pieces that fit together to form a complete e-commerce solution. Also, we will have built the "ground layers" of the app--what I mean by this is the lower level components that make the web application function... Everything we've built up to this point will be used as the foundation to build the most important aspects of the system and the main features and making functional Twig templates for displaying pages to the user.