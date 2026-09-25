---
layout: page
title: "Lecture 38: Demo - HPA"
permalink: /06-networks-services-routes-scaling/lecture-38-demo-hpa/
---

# Lecture 38: Demo - HPA

### 1. Create an HPA via CLI
To scale `myapp` between 2 and 10 pods whenever CPU exceeds 50%:
```bash
oc autoscale deployment/myapp --min=2 --max=10 --cpu-percent=50
```

### 2. View HPA Status
```bash
oc get hpa
```
*Note: It may take a minute for "Targets" to show actual percentages while metrics are collected.*

### 3. Simulate Load
If you run a load-testing tool against your Route URL, you will eventually see the "Replicas" count increase in the `oc get hpa` output.

---

## Navigation
- [← Previous: Lecture 37]({{ site.baseurl }}/06-networks-services-routes-scaling/lecture-37-hpa-overview/)
- [Next Topic: Lecture 39 - Quiz →]({{ site.baseurl }}/06-networks-services-routes-scaling/lecture-39-quiz-networking-scaling/)