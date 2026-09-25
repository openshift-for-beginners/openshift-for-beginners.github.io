---
layout: page
title: "Lecture 71: CI/CD for Beginners"
permalink: /09-conclusion-appendix/lecture-71-cicd-overview/
---

# Lecture 71: CI/CD for Beginners

**CI/CD** stands for Continuous Integration and Continuous Deployment.

### Continuous Integration (CI)
The practice of frequently merging code changes into a central repository, followed by automated builds and tests.
- **Goal:** Find bugs early.

### Continuous Deployment (CD)
The practice of automatically deploying every change that passes the CI stage to a production (or pre-production) environment.
- **Goal:** Release software faster and more reliably.

### CI/CD in OpenShift
OpenShift supports CI/CD through:
- **BuildConfigs & Triggers:** Simple, built-in automation.
- **OpenShift Pipelines:** Based on **Tekton**, this is a cloud-native CI/CD framework that runs entirely in the cluster.
- **OpenShift GitOps:** Based on **ArgoCD**, it ensures the cluster state matches the configuration stored in Git.

---

## Navigation
- [← Previous: Lecture 70]({{ site.baseurl }}/09-conclusion-appendix/lecture-70-demo-gitlab-setup/)
- [Next Topic: Lecture 72 - Bonus →]({{ site.baseurl }}/09-conclusion-appendix/lecture-72-bonus-summary/)