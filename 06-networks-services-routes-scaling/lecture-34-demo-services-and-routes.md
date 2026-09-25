---
layout: page
title: "Lecture 34: Demo - Services and Routes"
permalink: /06-networks-services-routes-scaling/lecture-34-demo-services-and-routes/
---

# Lecture 34: Demo - Services and Routes

### 1. View Services
```bash
oc get svc
```

### 2. View Routes
```bash
oc get routes
```

### 3. Create a Route from the CLI
If you have a service named `frontend`, you can expose it easily:
```bash
oc expose svc/frontend
```

### 4. Testing Connectivity
Use `curl` or a web browser to hit the URL provided in the `HOST/PORT` column of the `oc get routes` output.

---

## Navigation
- [← Previous: Lecture 33]({{ site.baseurl }}/06-networks-services-routes-scaling/lecture-33-services-and-routes/)
- [Next Topic: Lecture 35 - Scaling →]({{ site.baseurl }}/06-networks-services-routes-scaling/lecture-35-scaling/)