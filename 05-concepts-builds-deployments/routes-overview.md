---
layout: page
title: "Routes"
permalink: /05-concepts-builds-deployments/routes-overview/
---

# Routes: Exposing Applications

In Kubernetes, you use **Ingress** to expose services. In OpenShift, you use **Routes**.

## Key Features
- **Easy Setup:** A Route is created with one command: `oc expose svc/myapp`.
- **Automatic Hostnames:** OpenShift automatically generates a URL (e.g., `myapp-myproject.apps.cluster-name.com`).
- **TLS/SSL:** Routes support Edge, Passthrough, and Re-encryption termination types for secure traffic.

## Workflow
1. **Pod** runs the app.
2. **Service** provides internal load balancing to the Pods.
3. **Route** provides an external URL that points to the Service.

---

## Navigation
- [← Previous: Triggers and Webhooks]({{ site.baseurl }}/05-concepts-builds-deployments/triggers-and-webhooks/)
- [Next: Role Play 2 →]({{ site.baseurl }}/05-concepts-builds-deployments/role-play-02/)