---
layout: page
title: "Lecture 29: Custom Build"
permalink: /05-concepts-builds-deployments/lecture-29-custom-build/
---

# Lecture 29: Custom Build Strategy

The **Custom Build** strategy allows you to define a specific builder image that handles the build logic itself.

### When to use Custom Builds?
- When the S2I or Docker strategies are not enough for your specific requirements.
- When you have highly complex build requirements that involve multiple steps or specialized tools not found in standard builder images.
- When you want to use a completely different build engine within OpenShift.

### How it Works
You provide a Docker image that contains the build logic. OpenShift runs this image as a Pod, and that Pod is responsible for producing the final application image and pushing it to the registry.

---

## Navigation
- [← Previous: Lecture 28]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-28-s2i/)
- [Next Topic: Lecture 30 - Build Triggers →]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-30-build-triggers-webhooks/)