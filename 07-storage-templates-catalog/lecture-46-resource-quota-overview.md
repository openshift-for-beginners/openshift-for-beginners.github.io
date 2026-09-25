---
layout: page
title: "Lecture 46: Resource Quota Overview"
permalink: /07-storage-templates-catalog/lecture-46-resource-quota-overview/
---

# Lecture 46: Resource Quota Overview

While Requests/Limits apply to **Pods**, a **ResourceQuota** applies to the entire **Project**.

### Why use Quotas?
Administrators use Quotas to prevent one team from accidentally consuming all the resources in a cluster. 

### What can be limited?
- Total CPU and Memory across all pods in the project.
- Total number of Pods, Services, or PVCs.
- Total storage capacity (e.g., "This project can only use 20GB of total storage").

---

## Navigation
- [← Previous: Lecture 45]({{ site.baseurl }}/07-storage-templates-catalog/lecture-45-demo-resource-allocation/)
- [Next Topic: Lecture 47 - Demo Quota →]({{ site.baseurl }}/07-storage-templates-catalog/lecture-47-demo-resource-quota/)