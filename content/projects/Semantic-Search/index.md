---
title: "Semantic Search"
date: 2026-01-27
featured: "featured.png"
draft: false
description: "Project documentation for my MLOps Project"
tags: ["semantic", "search", "docker", "nlp", "linear algebra"]
showAuthor: true
---

## Purpose Of This Project
This project spawned from my professional experience in documentation, many times finding the most relevant information out of our documentation stores, and a lot of the time they don't even know what's in their own documentation either.

With my interest in Linear Algebra and Natural Language Processing as well as DevOps I figured that a solid project to work on would be to implement a full DevOps pipeline for a dockerized Semantic Search application.

## Tooling Utilized (Subject To Change As The Project Progresses)
- FastAPI - REST API
- Python - Primary Programming Language
- Docker - Containerization
- ChromaDB - Vector database
- VS Code - IDE Utilized
- HTML/CSS/JavaScript - Web Frontend
- GitHub - Version Control
- GitHub Actions - CI/CD
- GitHub Projects - Project Management
- pytest - Unit Testing Framework 
- Mermaid - Diagramming


## Weekly Progress

### 1/29/2026

#### Last Weeks Work

Last Week I spent my time thinking about what project I wanted to work on and making some neural connections between my work and the two other classes I'm taking right now with NLP and Linear Algebra. 

My NLP class went over NLTK and how to process Corpora and this got me thinking about how documentation systems are just large distributed Corpora.

I researched how NLP and Linear Algebra could be applied to documentation and stumbled on this great [Medium Article]() outlining what Semantic Search is and how these concepts might fit together, I also thought about how I'd like to incorporate a little bit of DevOps into this project so I looked into Docker and Github Actions a bit.

I cleaned up my Personal Portfolio Website it was a little neglected so I stood up a page for my project and changed some of the formatting and layout to be a bit more professional with the intent of showing off my portfolio of work.

I researched Vector Databases a bit to understand what I was getting myself into.

#### Work This Week

This week I plan to look a bit more into how to utilize existing Python libraries for handling .docx, .pdf, .txt, and .md files

Research a bit more about FastAPI

Look into the recommendation made to me by Professor Guinn Meta's FAISS library for similarity search and clustering of dense vectors 

Stand up my Github Repo for my project and start building

Pick my Vector Database

#### Impediments

I think the only impediment is that I'll be a traveling a little bit over this next week so making sure that I manage my time properly and find ways to offline some of the research I wanted to do (texts, documentation sites, books, etc.)
I'll be throwing this on my iPad and utilizing that for my offline workflow.


#### Reflections

I think my process can work better if I create an architectural diagram to help me with the big picture, and get this scoped into a project tracker so that I have something to reference broken down into smaller chunks and to keep me focused and on track. 


---

### 2/5/2026

#### Last Weeks Work

Last week I spent some time standing up my [GitHub Repo](https://github.com/Eonloop/semantix), and setting up the inital structure with the FastAPI Boilerplate, as well as the Dockerfile boilerplate and researching [ChromaDB](https://docs.trychroma.com/docs/overview/getting-started) vs. [Pinecone](https://www.pinecone.io/) vs. Meta's [FAISS](https://ai.meta.com/tools/faiss/) 

I decided to go with ChromaDB as my Vector Database, this decision was based on their simple integration with FastAPI and their "batteries included" style. Reading more into these tools was intriguing however, it seems like if I wanted a faster solution for simliarity search I would want to go with Meta's FAISS, but it seems a bit too low level for the scope I'm trying to maintain for this project, it seems like I'd need to build some supporting pieces to implement this properly for the task of text embedding comparisons.

Pinecone also presented an attractive solution, but with the cloud dependencies and more enterprise focus I figured I'd just go with ChromaDB for a purely local, fast and effective experience. That being said I'm now curious and will probably be poking at Pinecone and FAISS outside of this project as well.

I did some reading on [FastAPI](https://fastapi.tiangolo.com/tutorial/first-steps/) and it's accompanying web-server tools uvicorn which seems to be included if you `pip install fastapi[standard]` this getting started article was helpful. It reminded me of [Flask](https://flask.palletsprojects.com/en/stable/) a similar framework that I worked with in a previous class for assignments, as well as with an AI Technical interview application our team built. I got a boilerplate template stood up to familiarize myself with the tool so that I can eventually plug in my python scripting for text processing as well as the ChromaDB connection, and (hopefully) eventually a front-end user interface.

Finally I made sure to also take a look at Docker's documentation on containerizing this application so that I can make it portable, so that when someone wants to use or demo the tool they can do it from any machine they'd like. This [Writing a Dockerfile](https://docs.docker.com/get-started/docker-concepts/building-images/writing-a-dockerfile/) guide really helped me start a basic boilerplate to start the containerization process.

#### Next Weeks Work

Now that I'm back in the swing of things and have a little less travel time, this week will be more about the nuts and bolts. Some of my plans include:

- Standing up the scripts to ingest .pdf, .docx, and .md documentation, there are some python libraries that should help me out here.
- Create or pull some test documentation for ChromaDB to ingest, it seems to have an embedding pipeline already built in so that's cool and I'll see what I can do with that!
- Research more about Cosine Similarity Comparisons, this is already starting to pop-up in my NLP and Linear Algebra courses and it seems like it will be a better method than pure Euclidean distance (more to come on this)
- Stand up a diagram of what this flow will look like with Mermaid.js. Usually this is my first step, but I dove right into the research and boilerplates this time instead, I want to contextualize visually the flow I'm trying to achieve for this application, and the digramming stage is always one of the most helpful for me.

#### Impediments

- Context Switching: I think switching between work, the classes I'm taking, and everyday life can be tricky sometimes and it takes me a while to get into a solid flow. I think that scheduling some time for "Deep Work" this week may help me. I'm going to time block my calendar so that I carve out time appropriately.
- Fine tuning my strategy for how I'm approaching this project, making sure that I'm listing out the process via my diagram, and utilizing Github Projects more. I started with that a little bit this past week, but project management is it's own discipline that takes effort.

#### Reflections

Selecting a Vector Database and understanding the tooling that I'll be using and how I need to connect it has been a huge relief. I think trying to build the perfect architecture leads me into decision fatigue. That can be debilitating, I'm getting better about how I make my technical decisions. Which is helpful to actual moving forward on a project. It's all about iterations, getting the basic understanding and working prototype and building from there. I think I'm becoming a lot more realistic (while also maintaining a healthy level of curiosity) with how I handle projects. 


