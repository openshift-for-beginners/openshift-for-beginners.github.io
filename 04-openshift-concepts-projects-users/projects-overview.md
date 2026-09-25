---
layout: page
title: "Understanding Projects"
permalink: /04-openshift-concepts-projects-users/projects-overview/
---

# Understanding Projects

In Kubernetes, resources are grouped into **Namespaces**. OpenShift extends this concept by using **Projects**.

## What is a Project?
A Project is a Kubernetes Namespace with additional metadata. It is the primary unit of multi-tenancy in OpenShift.

## Key Characteristics
- **Isolation:** Resources in Project A are isolated from Project B.
- **Self-Service:** Users can be allowed to create their own projects.
- **Quotas:** Administrators can limit the amount of CPU, RAM, and Storage a single project can consume.

## Useful CLI Commands
- **Create a project:** `oc new-project my-app-demo`
- **Switch between projects:** `oc project <name>`
- **List projects:** `oc get projects`
- **Delete a project:** `oc delete project <name>` (Note: This deletes all resources inside!)

---

## Navigation
- [← Previous: Deploying Applications]({{ site.baseurl }}/04-openshift-concepts-projects-users/deploying-applications/)
- [Next: Users and Identity →]({{ site.baseurl }}/04-openshift-concepts-projects-users/users-overview/)