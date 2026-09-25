---
layout: page
title: "Deploying Applications"
permalink: /04-openshift-concepts-projects-users/deploying-applications/
---

# Deploying Applications: Web Console vs. CLI

OpenShift provides multiple workflows to get code running in a cluster.

## 1. Deploying via Web Console
The **Developer Perspective** is the primary tool for this.
- **Topology View:** Provides a visual representation of the application stack.
- **+Add Flow:** Allows you to deploy from:
    - **Git Repository:** OpenShift detects the language and builds the image.
    - **Container Image:** Use an existing image from a registry (like Docker Hub).
    - **Samples:** Pre-configured demo apps.
    - **Dockerfile:** Build directly from a Dockerfile in a Git repo.

## 2. Deploying via CLI (`oc`)
The CLI is faster for experienced users and necessary for automation.
- **New App command:** `oc new-app <image-name> or <git-url>`
- **Check Progress:** `oc get pods -w`
- **Expose Service:** `oc expose svc/<service-name>` (to create a Route).

## Comparison
| Method | Best For | Key Feature |
| :--- | :--- | :--- |
| **Web Console** | Beginners / Visualizing | Drag-and-drop relationship mapping |
| **CLI** | Power Users / Scripting | Faster execution and repeatability |

---

## Navigation
- [← Back to Section Index]({{ site.baseurl }}/04-openshift-concepts-projects-users/)
- [Next: Understanding Projects →]({{ site.baseurl }}/04-openshift-concepts-projects-users/projects-overview/)