---
layout: page
title: "Lecture 35: Scaling"
permalink: /06-networks-services-routes-scaling/lecture-35-scaling/
---

# Lecture 35: Scaling

Scaling is the process of increasing or decreasing the number of Pod instances to handle load.

### Types of Scaling
1. **Vertical Scaling:** Increasing the CPU or RAM of an existing Pod (Requires a restart).
2. **Horizontal Scaling:** Increasing the **number** of Pods (Replicas). This is the standard cloud-native approach.

### Manual Scaling
You can manually tell OpenShift exactly how many replicas you want for a Deployment or DeploymentConfig.

---

## Navigation
- [← Previous: Lecture 34]({{ site.baseurl }}/06-networks-services-routes-scaling/lecture-34-demo-services-and-routes/)
- [Next Topic: Lecture 36 - Demo Scaling →]({{ site.baseurl }}/06-networks-services-routes-scaling/lecture-36-demo-scaling/)