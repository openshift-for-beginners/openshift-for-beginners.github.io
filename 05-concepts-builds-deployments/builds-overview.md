---
layout: page
title: "Builds and BuildConfigs"
permalink: /05-concepts-builds-deployments/builds-overview/
---

# Builds and BuildConfigs

OpenShift can build container images directly within the cluster.

## 1. BuildConfig (`bc`)
A `BuildConfig` is the **definition** of how to create an image. It specifies:
- Where the source code is (e.g., GitHub).
- Which strategy to use (e.g., S2I or Docker).
- Where to push the resulting image (usually an Image Stream).

## 2. Build
A `Build` is the **running instance** of a BuildConfig. You can see build logs and history for every time a build is triggered.

## CLI Commands
- **Start a build:** `oc start-build <bc-name>`
- **View logs:** `oc logs -f build/<build-name>`
- **List builds:** `oc get builds`

---

## Navigation
- [← Previous: Image Streams]({{ site.baseurl }}/05-concepts-builds-deployments/image-streams/)
- [Next: Build Strategies →]({{ site.baseurl }}/05-concepts-builds-deployments/build-strategies/)