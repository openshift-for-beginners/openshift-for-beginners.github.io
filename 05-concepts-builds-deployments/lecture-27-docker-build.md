---
layout: page
title: "Lecture 27: Docker Build"
permalink: /05-concepts-builds-deployments/lecture-27-docker-build/
---

# Lecture 27: Docker Build Strategy

The **Docker Build** strategy is the most familiar method for developers coming from a standard Kubernetes or Docker background.

### How it Works
- OpenShift looks for a `Dockerfile` in the root of your source code repository (or a specified context directory).
- It performs a `docker build` using the OpenShift build engine.
- The resulting image is then pushed to the designated Image Stream.

### Key Considerations
- **Control:** You have total control over the base image, environment variables, and how the application is installed.
- **Security:** By default, OpenShift runs containers as a random non-privileged User ID. If your Dockerfile assumes it is running as `root` (e.g., writing to `/root` or protected folders), the container might fail to start on OpenShift.
- **Optimization:** You are responsible for keeping the image layers small and secure.

---

## Navigation
- [← Previous: Lecture 26]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-26-openshift-build-strategies/)
- [Next Topic: Lecture 28 - S2I →]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-28-s2i/)