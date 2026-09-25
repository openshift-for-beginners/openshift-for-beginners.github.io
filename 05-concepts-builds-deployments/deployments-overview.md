---
layout: page
title: "Deployments vs. DeploymentConfigs"
permalink: /05-concepts-builds-deployments/deployments-overview/
---

# Deployments vs. DeploymentConfigs

OpenShift supports two ways to manage application replicas.

## 1. Kubernetes Deployment (`Deployment`)
- The industry standard.
- Recommended for most new projects.
- Managed by the Kubernetes controller.

## 2. OpenShift DeploymentConfig (`DC`)
- The legacy OpenShift-specific resource.
- **Unique Feature:** Can be triggered to redeploy automatically when a new image version is detected in an **Image Stream**.
- Provides specialized deployment hooks (pre/post).

### Which one to use?
While `DeploymentConfig` was essential in early OpenShift versions, Red Hat now recommends using standard **Deployments** unless you specifically need "Image Change Triggers" or specialized lifecycle hooks.

---

## Navigation
- [← Previous: Components]({{ site.baseurl }}/05-concepts-builds-deployments/k8s-vs-openshift-components/)
- [Next: Image Streams →]({{ site.baseurl }}/05-concepts-builds-deployments/image-streams/)