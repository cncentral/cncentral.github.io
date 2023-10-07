---
title:  "Containerization using Containerd - The Basics"
description: containerd is the foundation for running containers across different platforms. Being the fundamental building block, Containerd can be used to implement the basic containerization use cases. This article explores what Containerd is and how to use it.
date:   2023-08-19
authors: [ravikanth]
image:  '/images/containerd.png'
tags:   [containers, learning, containerd]
featured: true
draft: true
---

[containerd](https://containerd.io/) is an industry-standard container runtime widely used across different types of container environments. containerd was initially released by Docker in the year 2015 and contributed to CNCF in 2017. It is one of the first [CNCF graduated projects](https://www.cncf.io/projects/containerd/) and the most active open-source [projects on GitHub](https://github.com/containerd/containerd). containerd is available on both Linux and Windows platforms to manage the complete lifecycle of containers, from image transfers to container execution to container storage and network management. containerd is used across different container orchestration engines and platforms. This includes Docker, Kubernetes, managed Kubernetes offerings such as Azure Kubernetes Service (AKS), Google Kubernetes Engine (GKE), and Amazon's Elastic Kubernetes Service (EKS) support configuring containerd as the runtime. These container engines and orchestration platforms offer more sophisticated capabilities beyond executing containers. However, suppose your use case does not involve complete container orchestration and monitoring, or it includes creating custom container solutions or integrating with other orchestration and automation tools. In that case, you may consider using containerd as a standalone container runtime. containerd is most suitable for creating a minimalist and specialized runtime environment for your applications.

In this article, you will learn about the architecture of containerd and how to install and use containerd for your application containers or development on the Linux operating system.

# Architecture



# Install containerd

Installing containerd on a Linux system is a multi-step process. 

