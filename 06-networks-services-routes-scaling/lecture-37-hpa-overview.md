---
layout: page
title: "Lecture 37: Autoscaling (HPA) Overview"
permalink: /06-networks-services-routes-scaling/lecture-37-hpa-overview/
---

# Lecture 37: Horizontal Pod Autoscaler (HPA) Overview

The **Horizontal Pod Autoscaler (HPA)** automatically scales the number of pods in a deployment based on observed CPU or Memory utilization.

### How it Works
1. You define a **Minimum** and **Maximum** number of pods.
2. You define a **Target Utilization** (e.g., 50% CPU).
3. The HPA controller queries the **Metrics Server** every 15 seconds.
4. If the average CPU usage across all pods is higher than the target, HPA increases the replica count.

### Prerequisite
For HPA to work, your Pods **must** have resource requests defined (e.g., you must tell OpenShift that the pod expects to use at least 100m of CPU).

---

## Navigation
- [← Previous: Lecture 36]({{ site.baseurl }}/06-networks-services-routes-scaling/lecture-36-demo-scaling/)
- [Next Topic: Lecture 38 - Demo HPA →]({{ site.baseurl }}/06-networks-services-routes-scaling/lecture-38-demo-hpa/)