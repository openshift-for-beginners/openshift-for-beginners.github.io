---
layout: page
title: "Lecture 26: OpenShift Build Strategies"
permalink: /05-concepts-builds-deployments/lecture-26-openshift-build-strategies/
---

# Lecture 26: OpenShift Build Strategies

OpenShift is flexible in how it creates images. There are three primary strategies used in a `BuildConfig`.

### 1. Docker Build
- **Source:** A Git repo containing a `Dockerfile`.
- **How it works:** OpenShift runs a standard `docker build` command using your Dockerfile.
- **Best for:** Teams that already have Docker experience and want full control over the image layers.

### 2. Source-to-Image (S2I)
- **Source:** Just the application source code (e.g., Java, Python, Ruby).
- **How it works:** OpenShift combines your code with a "Builder Image" to produce a final image. No Dockerfile required.
- **Best for:** Developers who want to focus on code rather than infrastructure.

### 3. Custom Build
- **Source:** Any image you define as a builder.
- **How it works:** You provide a custom Docker image that performs the build logic.
- **Best for:** Highly specialized or proprietary build processes.

---

## Navigation
- [← Previous: Lecture 25]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-25-demo-route/)
- [Back to Section Index]({{ site.baseurl }}/05-concepts-builds-deployments/)
- [Next Topic: Lecture 27 - Docker Build →]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-27-docker-build/)