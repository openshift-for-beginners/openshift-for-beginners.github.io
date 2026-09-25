---
layout: page
title: "Lecture 64: SCC Overview"
permalink: /08-openshift-security/lecture-64-scc-overview/
---

# Lecture 64: Security Context Constraints (SCC)

**SCCs** control what actions a Pod can perform and what it has access to on the host Node.

### Key Controls
- Can the pod run as **root**?
- Can it access the host's network or file system?
- What User ID (UID) is the container allowed to run as?

### Default SCC: `restricted`
By default, OpenShift is much more secure than standard Kubernetes. It applies the `restricted` SCC to most pods, which prevents them from running as root or accessing host resources. This is why some Docker images fail on OpenShift if they weren't designed with security in mind.

---

## Navigation
- [← Previous: Lecture 63]({{ site.baseurl }}/08-openshift-security/lecture-63-demo-network-policies/)
- [Next Topic: Lecture 65 - Demo SCC →]({{ site.baseurl }}/08-openshift-security/lecture-65-demo-scc-overview/)