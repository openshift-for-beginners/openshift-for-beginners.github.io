---
layout: page
title: "Lecture 58: Config Map Overview"
permalink: /08-openshift-security/lecture-58-config-map-overview/
---

# Lecture 58: Config Map Overview

**ConfigMaps** allow you to decouple configuration artifacts from image content.

### Why use ConfigMaps?
Instead of hardcoding a database URL or a feature flag inside your code, you store it in a ConfigMap. This allows you to use the same container image in Development, Testing, and Production just by changing the ConfigMap.

### How are they used?
- As **Environment Variables** inside the Pod.
- As **Files** mounted in a volume.

---

## Navigation
- [← Previous: Lecture 57]({{ site.baseurl }}/08-openshift-security/lecture-57-demo-user-contexts/)
- [Next Topic: Lecture 59 - Demo Config Maps →]({{ site.baseurl }}/08-openshift-security/lecture-59-demo-config-maps/)