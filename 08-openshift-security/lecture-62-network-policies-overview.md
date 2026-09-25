---
layout: page
title: "Lecture 62: Network Policies Overview"
permalink: /08-openshift-security/lecture-62-network-policies-overview/
---

# Lecture 62: Network Policies Overview

**Network Policies** act as a firewall for your Pods.

### Why use Network Policies?
By default, OpenShift allows all Pods in a cluster to talk to each other. Network Policies allow you to:
- Restrict traffic so only the **Frontend Pod** can talk to the **Database Pod**.
- Block all incoming traffic from outside the project except on specific ports.

### Logic
Policies use **Selectors** to identify which Pods the rule applies to and **Ingress/Egress** rules to define allowed traffic.

---

## Navigation
- [← Previous: Lecture 61]({{ site.baseurl }}/08-openshift-security/lecture-61-demo-secrets/)
- [Next Topic: Lecture 63 - Demo Network Policies →]({{ site.baseurl }}/08-openshift-security/lecture-63-demo-network-policies/)