---
title: Kubernetes - The Basics
description: Kubernetes is an open-source container orchestration and management platform. This article walks through the basics of Kubernetes and highlights its features.
date:   2021-10-20
authors: [ravikanth]
image:  '/images/k8s.png'
tags:   [kubernetes]
featured: true
draft: true
---

The rise of containers to package, distribute, and deploy applications changed how development and operations teams looked at applications and infrastructure. With application code and the necessary dependencies in the same package, containers allow a faster and more portable way to develop and distribute applications. Container engines such as Docker made developing, distributing, and deploying application services as containers easy. This led to complex microservice architectures that used containers to decompose larger applications into several small, single-purpose application services that can be developed and managed independently of other components in the application architecture. 

The Docker engine includes orchestration tools such as Compose and Swarm. Compose can orchestrate multiple container creation on a single node, while Swarm is a multi-host cluster that can orchestrate application containers across multiple hosts. Deploying and managing a microservices application requires more than just container orchestration. You need to be able to scale in or scale out the application services based on traffic patterns, resource utilization, and many other factors. You need to be able to monitor the availability of each container within the application architecture and take action when a service becomes unavailable. The need for better management capabilities also grows as the application complexity grows. Docker Compose and Swarm do not provide comprehensive management capabilities or the ecosystem for managing complex microservice architectures. This is where Kubernetes shines.

**Kubernetes**, often called K8s, is an [open-source platform](https://github.com/kubernetes/kubernetes) for automating containerized applications' deployment, scaling, and management. Building upon 15 years of experience running production workloads at Google, Kubernetes is one of the largest open-source projects. The name Kubernetes translates roughly to *the person at the helm who steers a ship*. At Google, three engineers- [Joe Beda](https://twitter.com/jbeda), [Brendan Burns](https://twitter.com/brendandburns), and [Craig McLuckie](https://twitter.com/cmcluck)- led the effort to build an open-source container orchestration and management system.

Kubernetes was first announced in 2014. Version 1.0 was released in 2015, and the same year, Google donated the Kubernetes project to the Cloud Native Computing Foundation. K8s became a CNCF-graduated project in 2018. Today, Kubernetes is the fastest-growing and most-used container orchestration and management system. With more than 3500 contributors, Kubernetes is one of the most active and largest open-source projects on GitHub.

## Architecture

At a high level, K8s contains a few components that are core to container orchestration and management.

![/images/kubernetes-container-runtime.png](/images/kubernetes-container-runtime.png)

The diagram shows that the Kubernetes infrastructure contains control plane and worker nodes. The Kubernetes control plane is the interface that defines, deploys, and manages the container's lifecycle.

The control plane is typically made of a few different components. This includes:

| Component                | Description                                                  |
| ------------------------ | ------------------------------------------------------------ |
| API Server               | This component is implemented as [kube-apiserver](https://kubernetes.io/docs/reference/command-line-tools-reference/kube-apiserver/) and is the front end for all Kubernetes cluster operations. |
| Controller Manager       | Kubernetes implements the                                    |
| etcd                     |                                                              |
| Scheduler                |                                                              |
| Cloud Controller Manager |                                                              |

