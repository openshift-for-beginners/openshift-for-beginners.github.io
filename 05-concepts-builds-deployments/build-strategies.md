---
layout: page
title: "Build Strategies"
permalink: /05-concepts-builds-deployments/build-strategies/
---

# Build Strategies

OpenShift supports three main ways to build images:

## 1. Source-to-Image (S2I)
- **Concept:** You provide source code; OpenShift provides a "Builder Image" (e.g., Python, Java, Node.js).
- **Benefit:** Developers don't need to learn Docker or write Dockerfiles.
- **Process:** OpenShift injects your code into the builder image and produces a final application image.

## 2. Docker Build
- **Concept:** OpenShift looks for a `Dockerfile` in your repository.
- **Benefit:** Full control over the build process.

## 3. Custom Build
- **Concept:** You provide your own builder image to perform highly specific build tasks.
- **Benefit:** For complex scenarios not covered by S2I or Docker strategies.

---

## Navigation
- [← Previous: Builds Overview]({{ site.baseurl }}/05-concepts-builds-deployments/builds-overview/)
- [Next: Triggers and Webhooks →]({{ site.baseurl }}/05-concepts-builds-deployments/triggers-and-webhooks/)