---
layout: page
title: "Knowledge Check"
permalink: /05-concepts-builds-deployments/quiz/
---

# Knowledge Check: Builds and Deployments

**1. Which resource defines *how* an image should be built from source code?**
- [ ] DeploymentConfig
- [x] BuildConfig
- [ ] Route

**2. What is the main benefit of using an Image Stream instead of a direct Docker Registry URL?**
- [ ] It stores the actual image data.
- [x] It allows for automatic triggers when an image is updated.
- [ ] It makes the containers run faster.

**3. Which build strategy allows you to build an application without writing a Dockerfile?**
- [ ] Docker Build
- [x] Source-to-Image (S2I)
- [ ] Custom Build

**4. To expose a service to the external internet with an automatic URL, you create a:**
- [ ] ServiceStream
- [ ] IngressConfig
- [x] Route

---

## Navigation
- [← Back to Section Index]({{ site.baseurl }}/05-concepts-builds-deployments/)
- [Next Section: Networking and Scaling →]({{ site.baseurl }}/06-networks-services-routes-scaling/)