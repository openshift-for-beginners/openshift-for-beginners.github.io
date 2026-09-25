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