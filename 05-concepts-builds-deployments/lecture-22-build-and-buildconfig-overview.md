---
layout: page
title: "Lecture 22: Build and Build Config Overview"
permalink: /05-concepts-builds-deployments/lecture-22-build-and-buildconfig-overview/
---

# Lecture 22: Build and Build Config Overview

One of OpenShift's most powerful features is its ability to build container images directly from source code. This is managed through two resources:

### 1. BuildConfig (`bc`)
The **BuildConfig** is the definition or the "recipe." It tells OpenShift:
- **Source:** Where is the code? (e.g., a Git URL).
- **Strategy:** How should it be built? (e.g., S2I or Dockerfile).
- **Output:** Where should the resulting image be sent? (usually an Image Stream).

### 2. Build
A **Build** is a single instance of that process running. 
- Every time you trigger a build, a new `Build` object is created.
- Builds are numbered (e.g., `myapp-1`, `myapp-2`).
- A Build runs inside a temporary Pod to perform the compilation and image creation.

---

## Navigation
- [← Previous: Lecture 21]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-21-demo-image-streams/)
- [Next Topic: Lecture 23 - Demo Build/BuildConfig →]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-23-demo-build-and-buildconfig/)