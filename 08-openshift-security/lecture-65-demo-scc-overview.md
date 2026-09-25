---
layout: page
title: "Lecture 65: Demo - SCC Overview"
permalink: /08-openshift-security/lecture-65-demo-scc-overview/
---

# Lecture 65: Demo - SCC Overview

### 1. List all SCCs (Admin only)
```bash
oc get scc
```

### 2. Check which SCC a Pod is using
```bash
oc get pod <pod-name> -o yaml | grep scc
```

### 3. Granting SCC permissions
If you have a specialized pod that **must** run as root (e.g., a logging agent), you grant the ServiceAccount the `anyuid` or `privileged` SCC:
```bash
oc adm policy add-scc-to-user anyuid -z my-service-account
```

---

## Navigation
- [← Previous: Lecture 64]({{ site.baseurl }}/08-openshift-security/)
- [Next Topic: Lecture 66 - Operators →]({{ site.baseurl }}/08-openshift-security/lecture-66-introduction-to-operators/)