---
layout: page
title: "Lecture 18: Deployment Config vs. Kubernetes Deployment"
permalink: /05-concepts-builds-deployments/lecture-18-deploymentconfig-vs-deployment/
---

# Lecture 18: Deployment Config vs. Kubernetes Deployment

In OpenShift, you have two choices for managing application replicas and updates.

### 1. Kubernetes Deployment (`Deployment`)
- **Standard:** The industry-wide Kubernetes object.
- **Controller:** Managed by the Kubernetes deployment controller.
- **Recommendation:** Generally preferred for most modern cloud-native applications.

### 2. OpenShift DeploymentConfig (`DC`)
- **OpenShift Native:** Created specifically for OpenShift.
- **Triggers:** Can automatically redeploy when an **Image Stream** tag changes (Image Change Trigger).
- **Hooks:** Supports complex lifecycle hooks (Pre, Post, Mid deployment scripts).
- **Strategy:** Often used in classic OpenShift S2I (Source-to-Image) workflows.

### Which should I use?
While `DeploymentConfig` provides some automated triggers that standard Kubernetes `Deployment` lacks, the standard Kubernetes `Deployment` is now the recommended default for most use cases to ensure portability.

---

## Navigation
- [← Previous: Lecture 17]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-17-openshift-vs-k8s-components/)
- [Next Topic: Lecture 19 - Demo →]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-19-demo-deploymentconfig-deployment/)