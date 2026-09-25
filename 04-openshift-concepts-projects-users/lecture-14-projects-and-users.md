---
layout: page
title: "Lecture 14: Projects and Users"
permalink: /04-openshift-concepts-projects-users/lecture-14-projects-and-users/
---

# Lecture 14: Projects and Users

OpenShift is a multi-tenant platform designed for secure collaboration.

### What is a Project?
An OpenShift **Project** is a Kubernetes Namespace with extra features:
- **Isolation:** Resources are hidden from other users.
- **Self-Service:** Admins can let users create their own projects.

### Understanding Users
1. **Regular Users:** Humans logging in via CLI/UI.
2. **System Users:** Internal accounts for cluster tasks.
3. **Service Accounts:** Accounts used by **applications** (pods) to interact with the API.

---

## Navigation
- [← Previous: Lecture 13]({{ site.baseurl }}/04-openshift-concepts-projects-users/lecture-13-deploying-applications-cli/)
- [Next Topic: Lecture 15 - Demo →]({{ site.baseurl }}/04-openshift-concepts-projects-users/lecture-15-demo-projects-and-users/)