---
layout: page
title: "Lecture 17: OpenShift vs. K8s Components"
permalink: /05-concepts-builds-deployments/lecture-17-openshift-vs-k8s-components/
---

# Lecture 17: OpenShift vs. Kubernetes Components

OpenShift is built on top of Kubernetes. While it uses all the standard Kubernetes objects (Pods, Services, ConfigMaps), it introduces several "wrapper" or "extension" components to improve the developer experience and automate security.

### Core Comparison Table

| Feature | Standard Kubernetes | OpenShift Extension |
| :--- | :--- | :--- |
| **Namespace** | Namespace | **Project** (Namespace + Metadata + Security) |
| **External Access** | Ingress | **Route** (Easier DNS and TLS management) |
| **Deployments** | Deployment | **DeploymentConfig** (Adds triggers and hooks) |
| **Image Management** | Direct Registry URL | **Image Stream** (Abstraction layer for images) |
| **CI/CD** | External Tools | **BuildConfig** (Integrated Build system) |

### Key Takeaway
OpenShift components are often "opinionated" versions of Kubernetes components. They are designed to work together to automate the path from source code to a running, secure URL.

---

## Navigation
- [← Back to Section Index]({{ site.baseurl }}/05-concepts-builds-deployments/)
- [Next Topic: Lecture 18 - Deployment vs. DeploymentConfig →]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-18-deploymentconfig-vs-deployment/)