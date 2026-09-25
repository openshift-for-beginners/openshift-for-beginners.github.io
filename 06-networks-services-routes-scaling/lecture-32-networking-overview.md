---
layout: page
title: "Lecture 32: Networking Overview"
permalink: /06-networks-services-routes-scaling/lecture-32-networking-overview/
---

# Lecture 32: Networking Overview

OpenShift uses a **Software Defined Network (SDN)** to provide connectivity between pods across the cluster.

### Key Networking Concepts
1. **Pod IP:** Every Pod gets its own unique IP address. However, Pods are ephemeral (they die and restart), so these IPs change.
2. **Service IP (ClusterIP):** A stable IP address that sits in front of a group of Pods. It provides internal load balancing.
3. **Flat Network:** By default, all Pods in the cluster can communicate with each other regardless of which Node they are running on.
4. **Project Isolation:** While the network is technically "flat," OpenShift uses Network Policies to isolate traffic between different Projects for security.

---

## Navigation
- [← Back to Section Index]({{ site.baseurl }}/06-networks-services-routes-scaling/)
- [Next Topic: Lecture 33 - Services and Routes →]({{ site.baseurl }}/06-networks-services-routes-scaling/lecture-33-services-and-routes/)