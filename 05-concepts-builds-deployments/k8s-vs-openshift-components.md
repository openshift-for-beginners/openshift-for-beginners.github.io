---
layout: page
title: "K8s vs. OpenShift Components"
permalink: /05-concepts-builds-deployments/k8s-vs-openshift-components/
---

# OpenShift vs. Kubernetes Components

OpenShift is built on Kubernetes, so it uses all standard Kubernetes objects (Pods, Services, ConfigMaps). However, OpenShift introduces higher-level abstractions to simplify development.

| Standard Kubernetes | OpenShift Extension | Purpose |
| :--- | :--- | :--- |
| Namespace | **Project** | Multi-tenancy with extra security/metadata. |
| Ingress | **Route** | Easier external access with automatic DNS. |
| Deployment | **DeploymentConfig** | Adds triggers (e.g., deploy when image changes). |
| Container Image | **Image Stream** | Abstraction layer for tracking image versions. |
| (External CI/CD) | **BuildConfig** | Integrated tool to build images from source. |

---

## Navigation
- [← Back to Section Index]({{ site.baseurl }}/05-concepts-builds-deployments/)
- [Next: Deployments Overview →]({{ site.baseurl }}/05-concepts-builds-deployments/deployments-overview/)