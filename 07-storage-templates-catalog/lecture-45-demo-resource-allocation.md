---
layout: page
title: "Lecture 45: Demo - Resource Allocation"
permalink: /07-storage-templates-catalog/lecture-45-demo-resource-allocation/
---

# Lecture 45: Demo - Resource Allocation

### 1. Setting Resources in YAML
You define resources inside the `containers` section of a Deployment:
```yaml
resources:
  requests:
    memory: "64Mi"
    cpu: "250m"
  limits:
    memory: "128Mi"
    cpu: "500m"
```

### 2. Check Resource Usage
To see how much CPU/RAM your pods are actually using:
```bash
oc adm top pods
```
*(Note: Requires Metrics Server to be installed in the cluster).*

---

## Navigation
- [← Previous: Lecture 44]({{ site.baseurl }}/07-storage-templates-catalog/lecture-44-resource-allocation-cpu-ram/)
- [Next Topic: Lecture 46 - Resource Quota Overview →]({{ site.baseurl }}/07-storage-templates-catalog/lecture-46-resource-quota-overview/)