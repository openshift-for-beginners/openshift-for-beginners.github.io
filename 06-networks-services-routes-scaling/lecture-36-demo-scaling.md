---
layout: page
title: "Lecture 36: Demo - Scaling"
permalink: /06-networks-services-routes-scaling/lecture-36-demo-scaling/
---

# Lecture 36: Demo - Scaling

### 1. Scale via CLI
To scale a deployment named `myapp` to 3 replicas:
```bash
oc scale deployment/myapp --replicas=3
```

### 2. Verify Scaling
Watch the pods being created in real-time:
```bash
oc get pods -w
```

### 3. Scale via Web Console
- Go to **Developer Perspective** → **Topology**.
- Click on the application.
- Use the **up/down arrows** on the Pod ring to change the replica count instantly.

---

## Navigation
- [← Previous: Lecture 35]({{ site.baseurl }}/06-networks-services-routes-scaling/lecture-35-scaling/)
- [Next Topic: Lecture 37 - HPA Overview →]({{ site.baseurl }}/06-networks-services-routes-scaling/lecture-37-hpa-overview/)