---
layout: page
title: "Image Streams"
permalink: /05-concepts-builds-deployments/image-streams/
---

# Image Streams: Tracking Container Images

An **Image Stream** is a powerful abstraction that points to container images. It does not store the image itself, but it keeps track of tags and versions.

## Why use Image Streams?
1. **Abstraction:** Your Deployment points to the Image Stream, not a specific registry URL. If the image moves, you only update the Image Stream.
2. **Triggers:** OpenShift can "watch" an Image Stream. When a new image is pushed, OpenShift can automatically trigger a new deployment.
3. **Internal Registry:** OpenShift has a built-in registry that populates these streams automatically when you build code.

## Useful Commands
- **List streams:** `oc get is`
- **Import an image:** `oc import-image my-img --from=docker.io/library/nginx --confirm`

---

## Navigation
- [← Previous: Deployments]({{ site.baseurl }}/05-concepts-builds-deployments/deployments-overview/)
- [Next: Builds Overview →]({{ site.baseurl }}/05-concepts-builds-deployments/builds-overview/)