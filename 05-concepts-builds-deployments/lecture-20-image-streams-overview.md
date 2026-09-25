---
layout: page
title: "Lecture 20: Image Streams Overview"
permalink: /05-concepts-builds-deployments/lecture-20-image-streams-overview/
---

# Lecture 20: Image Streams Overview

An **Image Stream** (`is`) is an abstraction layer that points to container images. It does not store the actual image file; instead, it stores metadata about where the image lives and how it is tagged.

### Why use Image Streams?
1. **Abstraction:** Your Deployment/Pod points to the Image Stream name, not a long registry URL like `quay.io/my-registry/my-app:v1.2`.
2. **Automated Rollouts:** When an Image Stream is updated with a new image version, OpenShift can automatically trigger a new deployment of the app.
3. **Internal Tracking:** It makes it easier to manage "latest" tags while keeping track of previous versions.

### Key Concept: ImageChangeTrigger
This is the connection between Image Streams and DeploymentConfigs. If an Image Stream is updated, the DeploymentConfig "notices" and restarts the pods with the new image immediately.

---

## Navigation
- [← Previous: Lecture 19]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-19-demo-deploymentconfig-deployment/)
- [Next Topic: Lecture 21 - Demo →]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-21-demo-image-streams/)