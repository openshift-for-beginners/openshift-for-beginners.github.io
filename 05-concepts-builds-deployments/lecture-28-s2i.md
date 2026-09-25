---
layout: page
title: "Lecture 28: S2I (Source-to-Image)"
permalink: /05-concepts-builds-deployments/lecture-28-s2i/
---

# Lecture 28: Source-to-Image (S2I)

**Source-to-Image (S2I)** is an OpenShift-native tool that produces ready-to-run images by injecting source code into a container image and letting that image prepare the code for execution.

### The S2I Process
1. **Builder Image:** OpenShift provides (or you provide) a builder image for a specific language (e.g., Python, Node.js, Java).
2. **Assemble Script:** The builder image contains an `assemble` script that knows how to build the code (e.g., running `npm install` or `mvn package`).
3. **Run Script:** The resulting image contains a `run` script that knows how to start the application.

### Why Developers Love S2I
- **No Dockerfile required:** You don't need to learn how to write or maintain Dockerfiles.
- **Security:** Red Hat provides officially supported, patched, and secure builder images.
- **Standardization:** All apps in a specific language follow the same build pattern across the organization.

---

## Navigation
- [← Previous: Lecture 27]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-27-docker-build/)
- [Next Topic: Lecture 29 - Custom Build →]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-29-custom-build/)