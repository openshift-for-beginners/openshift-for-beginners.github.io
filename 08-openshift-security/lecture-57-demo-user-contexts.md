---
layout: page
title: "Lecture 57: Demo - Setting up User Contexts"
permalink: /08-openshift-security/lecture-57-demo-user-contexts/
---

# Lecture 57: Demo - Setting up User Contexts

A **Context** is a combination of a Cluster, a User, and a Project.

### 1. View your current config
```bash
oc config view
```

### 2. Switching Projects
Changing projects is technically changing your current context's namespace:
```bash
oc project my-other-project
```

### 3. Login as a different user
If you are testing RBAC, you can log in as another user to verify their limited permissions:
```bash
oc login -u developer -p developer
```

---

## Navigation
- [← Previous: Lecture 56]({{ site.baseurl }}/08-openshift-security/lecture-56-demo-rbac/)
- [Next Topic: Lecture 58 - Config Map Overview →]({{ site.baseurl }}/08-openshift-security/lecture-58-config-map-overview/)