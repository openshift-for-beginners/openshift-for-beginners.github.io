---
layout: page
title: "Lecture 13: Deploying Applications - CLI"
permalink: /04-openshift-concepts-projects-users/lecture-13-deploying-applications-cli/
---

# Lecture 13: Deploying Applications - CLI

The OpenShift CLI (`oc`) is the tool of choice for automation and faster resource management.

### Creating an Application
The core command is `oc new-app`.
- **From Source:** `oc new-app https://github.com/myrepo/myapp`
- **From an Image:** `oc new-app nginx:latest`

### Monitoring Commands
- **Check Status:** `oc status`
- **View Pods:** `oc get pods`
- **Create a Route:** `oc expose svc/<service-name>` (Generates a public URL).

---

## Navigation
- [← Previous: Lecture 12]({{ site.baseurl }}/04-openshift-concepts-projects-users/lecture-12-deploying-applications-web-console/)
- [Next Topic: Lecture 14 - Projects and Users →]({{ site.baseurl }}/04-openshift-concepts-projects-users/lecture-14-projects-and-users/)