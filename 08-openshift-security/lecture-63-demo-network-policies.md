---
layout: page
title: "Lecture 63: Demo - Network Policies"
permalink: /08-openshift-security/lecture-63-demo-network-policies/
---

# Lecture 63: Demo - Network Policies

### 1. View Policies
```bash
oc get networkpolicy
```

### 2. Example: Deny All Traffic
A common security best practice is to deny all traffic by default and then explicitly allow what is needed.
```yaml
kind: NetworkPolicy
apiVersion: networking.k8s.io/v1
metadata:
  name: deny-by-default
spec:
  podSelector: {}
  ingress: []
```

---

## Navigation
- [← Previous: Lecture 62]({{ site.baseurl }}/08-openshift-security/lecture-62-network-policies-overview/)
- [Next Topic: Lecture 64 - SCC Overview →]({{ site.baseurl }}/08-openshift-security/lecture-64-scc-overview/)