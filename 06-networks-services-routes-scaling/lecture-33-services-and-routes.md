---
layout: page
title: "Lecture 33: Services and Routes"
permalink: /06-networks-services-routes-scaling/lecture-33-services-and-routes/
---

# Lecture 33: Services and Routes

To make an application accessible, we use Services for internal traffic and Routes for external traffic.

### Services
- **Purpose:** Stable entry point for Pods.
- **Internal:** Services are usually only reachable from within the cluster.
- **Load Balancing:** If you have 3 replicas of a Pod, the Service distributes requests among them.

### Routes
- **Purpose:** Exposes a Service to the outside world (the internet).
- **DNS:** Automatically creates a human-readable URL.
- **TLS Termination:**
    - **Edge:** SSL ends at the Router.
    - **Passthrough:** SSL goes straight to the Pod.
    - **Re-encryption:** Router decrypts and then re-encrypts traffic to the Pod.

---

## Navigation
- [← Previous: Lecture 32]({{ site.baseurl }}/06-networks-services-routes-scaling/lecture-32-networking-overview/)
- [Next Topic: Lecture 34 - Demo →]({{ site.baseurl }}/06-networks-services-routes-scaling/lecture-34-demo-services-and-routes/)