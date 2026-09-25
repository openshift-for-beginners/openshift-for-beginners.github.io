---
layout: page
title: "Lecture 44: Resource Allocation - CPU and RAM"
permalink: /07-storage-templates-catalog/lecture-44-resource-allocation-cpu-ram/
---

# Lecture 44: Resource Allocation - CPU and RAM

To ensure cluster stability, we must define how much CPU and Memory a Pod can use.

### Requests vs. Limits
1. **Requests:** The *minimum* amount of resources guaranteed to the container. OpenShift uses this to decide which Node has enough room to run the Pod.
2. **Limits:** The *maximum* amount of resources the container is allowed to consume.
    - If a Pod hits its **Memory Limit**, it is killed (OOMKilled).
    - If a Pod hits its **CPU Limit**, it is throttled (slowed down).

---

## Navigation
- [← Previous: Lecture 43]({{ site.baseurl }}/07-storage-templates-catalog/lecture-43-demo-dynamic-provisioning/)
- [Next Topic: Lecture 45 - Demo Resource Allocation →]({{ site.baseurl }}/07-storage-templates-catalog/lecture-45-demo-resource-allocation/)