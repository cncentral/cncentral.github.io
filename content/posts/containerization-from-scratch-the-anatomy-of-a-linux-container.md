---
title:  "Containerization from scratch: The Anatomy of a Linux container"
description: Containers are isolated processes built using native Linux constructs such as namespaces, cgroups, and security policies. Knowing these constructs is important to understanding and effectively working with containerization technologies like Docker, Kubernetes, etc.
date:   2023-04-01
authors: [ravikanth]
image:  '/images/containerization.png'
tags:   [containers, learning, linux]
featured: false
draft: true
---

Containers are everywhere. One of the most popular application architectures is microservices-based and involves containerizing applications. Docker made containerization popular by introducing tooling that made it easy to package, distribute, and run applications as Linux containers. But how are containers created? Are they the same as virtual machines? In this article, you will learn about the anatomy of containers. Knowing what 

Before exploring the anatomy of containers, you must inspect what running applications require. 
