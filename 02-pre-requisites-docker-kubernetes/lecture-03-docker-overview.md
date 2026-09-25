---
layout: page
title: "Section 2: Pre-Requisites - Docker and Kubernetes"
permalink: /02-pre-requisites-docker-kubernetes/
---

# Section 2: Pre-Requisites - Docker and Kubernetes

Before working with OpenShift, it is important to understand the two core foundations behind it:

- **Docker / container basics** for packaging applications
- **Kubernetes basics** for orchestrating containers

This section provides a simple conceptual grounding for both topics so later OpenShift concepts make more sense.

---

## Topics in this section

1. [Lecture 3: Docker Overview]({{ site.baseurl }}/02-pre-requisites-docker-kubernetes/lecture-03-docker-overview/)
2. [Lecture 4: Kubernetes Overview]({{ site.baseurl }}/02-pre-requisites-docker-kubernetes/lecture-04-kubernetes-overview/)

---

## Learning Goals

By the end of this section, I should be able to:

- explain what a container is
- describe the purpose of Docker
- understand the difference between images and containers
- explain why container orchestration is needed
- describe what Kubernetes does
- connect Docker and Kubernetes concepts to OpenShift

---

## Why this section matters

OpenShift is built on top of Kubernetes and works with containerized applications.  
That means I need to understand:

- how applications are packaged
- how containers run
- how multiple containers are managed
- how applications are scheduled, scaled, and exposed

Without these basics, many OpenShift objects such as Pods, Deployments, Image Streams, Routes, and Builds can feel confusing.

---

## Section Summary

- Docker helps package and run applications in containers.
- Kubernetes helps manage containers at scale.
- OpenShift builds on Kubernetes and adds platform capabilities for developers and administrators.

---

## Navigation

- [← Previous Section: Introduction]({{ site.baseurl }}/01-introduction/)
- [Lecture 3: Docker Overview →]({{ site.baseurl }}/02-pre-requisites-docker-kubernetes/lecture-03-docker-overview/)
```

---

## `02-pre-requisites-docker-kubernetes/lecture-03-docker-overview.md`

```markdown
---
layout: page
title: "Lecture 3: Docker Overview"
permalink: /02-pre-requisites-docker-kubernetes/lecture-03-docker-overview/
---

# Lecture 3: Docker Overview

## Overview

Docker is one of the most important foundational technologies in the container ecosystem.  
It helps package an application along with its dependencies into a portable unit called a **container**.

Understanding Docker makes it easier to understand how applications are built, shipped, and run in OpenShift.

---

## Learning Objectives

After this topic, I should be able to:

- explain what Docker is
- describe what a container is
- differentiate between an image and a container
- understand why containers are useful
- connect Docker concepts to OpenShift workflows

---

## What is Docker?

Docker is a platform and toolset used to:

- build container images
- run containers
- package applications consistently
- move workloads across environments

It became popular because it made containers easier for developers to use in everyday workflows.

In simple terms:

- **Docker image** = packaged application template
- **Docker container** = running instance of that image

---

## What is a Container?

A container is a lightweight, isolated runtime environment that includes:

- the application code
- required libraries
- dependencies
- runtime components
- configuration needed to start the app

A container allows an application to run consistently across different environments.

### Key idea
Instead of saying:
> "It works on my machine"

containers help teams say:
> "It works the same everywhere"

---

## Why Containers Became Popular

Traditional deployment often had problems such as:

- applications behaving differently across environments
- dependency conflicts
- long setup times
- difficulty scaling consistently

Containers solve many of these problems by standardizing application packaging.

### Benefits of containers

- portability
- consistency
- faster deployment
- isolation
- easier scaling
- better resource usage than full virtual machines

---

## Containers vs Virtual Machines

Containers and virtual machines both provide isolation, but they work differently.

### Virtual Machines
Virtual machines include:

- application
- dependencies
- full guest operating system

They are heavier and consume more resources.

### Containers
Containers include:

- application
- dependencies
- shared host OS kernel

They are lighter, faster to start, and more efficient.

### Simplified comparison

| Aspect | Virtual Machine | Container |
|---|---|---|
| Includes full OS | Yes | No |
| Startup speed | Slower | Faster |
| Resource usage | Higher | Lower |
| Isolation level | Strong | Lightweight |
| Portability | Good | Very good |

---

## Docker Image vs Docker Container

This distinction is essential.

### Docker Image
A Docker image is:

- a packaged blueprint
- read-only
- used to create containers

It contains everything needed to run the application.

### Docker Container
A Docker container is:

- a running instance of an image
- active and executable
- created from an image

### Example
If an image is like a **class template**, then a container is like the **running object created from it**.

---

## Common Docker Concepts

### 1. Dockerfile
A `Dockerfile` is a text file that defines how to build a Docker image.

It may specify:

- base image
- files to copy
- commands to run
- application startup command

### 2. Image
Built from a Dockerfile and stored locally or in a registry.

### 3. Container
A running instance of the image.

### 4. Registry
A place where container images are stored and shared.

Examples include:

- Docker Hub
- private registries
- enterprise registries
- OpenShift internal image registry

---

## Basic Docker Workflow

A typical Docker workflow looks like this:

1. Write application code
2. Create a `Dockerfile`
3. Build an image
4. Store or push the image to a registry
5. Run the image as a container

---

## Common Docker Commands

### Build an image
```bash
docker build -t myapp:1.0 .
```

### Run a container
```bash
docker run -d -p 8080:80 myapp:1.0
```

### List running containers
```bash
docker ps
```

### List images
```bash
docker images
```

### Stop a container
```bash
docker stop <container-id>
```

---

## Why Docker Matters for OpenShift

OpenShift runs containerized applications.  
That means Docker-related concepts are directly relevant to:

- application packaging
- image creation
- build strategies
- registries
- deployments

Even when OpenShift uses Kubernetes-native container runtimes under the hood, the **Docker mental model** is still very useful for learning.

### OpenShift-related connections

- Docker images are deployed onto OpenShift
- OpenShift can build images from source
- OpenShift image streams help track container images
- OpenShift deployments run application containers in pods

---

## Important Mental Model

Think of the stack like this:

- **Docker / containers** → package and run applications
- **Kubernetes** → orchestrates containers
- **OpenShift** → provides a richer platform on top of Kubernetes

---

## Key Takeaways

- Docker helps package applications into containers
- Containers are lightweight and portable
- Images are templates; containers are running instances
- Registries store images
- Docker concepts are foundational for OpenShift

---

## My Notes

### What seems important
- image vs container distinction
- Dockerfile as image definition
- registry as image storage
- portability and consistency as key benefits

### Topics to revisit later
- how OpenShift builds images
- how image streams differ from raw Docker image handling
- how S2I compares to Dockerfile-based builds

---

## Quick Summary

Docker introduced a practical way to package applications into containers.  
These containers are lightweight, portable, and consistent across environments.  
This forms the application packaging foundation that OpenShift later builds on.

---

## Navigation

- [← Back to Section 2]({{ site.baseurl }}/02-pre-requisites-docker-kubernetes/)
- [Next Topic: Kubernetes Overview →]({{ site.baseurl }}/02-pre-requisites-docker-kubernetes/lecture-04-kubernetes-overview/)

