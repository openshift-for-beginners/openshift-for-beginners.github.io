---
layout: page
title: "Lecture 53: User Management Overview"
permalink: /08-openshift-security/lecture-53-user-management-overview/
---

# Lecture 53: User Management Overview

OpenShift manages access by tracking three types of entities:

1. **Users:** Actual human beings interacting with the cluster.
2. **Groups:** A collection of users. Granting permissions to a group is easier than managing users individually.
3. **ServiceAccounts:** Special accounts used by **applications** or processes (like a CI/CD pipeline or a Pod) to interact with the OpenShift API.

### Identity vs. User
- An **Identity** comes from an external provider (like GitHub or LDAP).
- A **User** is the internal object in OpenShift that represents that identity.

---

## Navigation
- [← Back to Section Index]({{ site.baseurl }}/08-openshift-security/)
- [Next Topic: Lecture 54 - Demo User Management →]({{ site.baseurl }}/08-openshift-security/lecture-54-demo-user-management/)