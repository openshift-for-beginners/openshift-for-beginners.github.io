---
layout: page
title: "Lecture 24: Route Overview"
permalink: /05-concepts-builds-deployments/lecture-24-route-overview/
---

# Lecture 24: Route Overview

In standard Kubernetes, you use an **Ingress** to expose an application to the internet. OpenShift uses **Routes**.

### What is a Route?
A Route is an OpenShift object that tells the built-in **HAProxy Router** to send external traffic to an internal **Service**.

### Key Advantages
- **Automatic DNS:** OpenShift automatically generates a unique URL for you.
- **Ease of Use:** You can create a route with a single command or a few clicks.
- **TLS Termination:** Routes handle SSL/TLS certificates easily (Edge, Passthrough, or Re-encryption).

### The Traffic Flow
`User Browser` → `OpenShift Router` → `Route` → `Service` → `Pod`

---

## Navigation
- [← Previous: Lecture 23]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-23-demo-build-and-buildconfig/)
- [Next Topic: Lecture 25 - Demo Route →]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-25-demo-route/)