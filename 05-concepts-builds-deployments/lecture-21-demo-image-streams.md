---
layout: page
title: "Lecture 21: Demo - Image Streams"
permalink: /05-concepts-builds-deployments/lecture-21-demo-image-streams/
---

# Lecture 21: Demo - Image Streams

### 1. View Existing Image Streams
To see the image streams available in your current project:
```bash
oc get is
```

### 2. Import an Image into a Stream
You can import an image from an external registry (like Docker Hub) and track it as an Image Stream:
```bash
oc import-image my-nginx --from=docker.io/library/nginx:latest --confirm
```

### 3. Inspect a Stream
To see the different "tags" and the specific SHAs (unique identifiers) being tracked:
```bash
oc describe is my-nginx
```

This ensures that even if a registry tag is overwritten, OpenShift can track the specific version currently in use.

---

## Navigation
- [← Previous: Lecture 20]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-20-image-streams-overview/)
- [Back to Section Index]({{ site.baseurl }}/05-concepts-builds-deployments/)
- [Next Topic: Lecture 22 - Build and BuildConfig Overview →]({{ site.baseurl }}/05-concepts-builds-deployments/lecture-22-build-and-buildconfig-overview/)