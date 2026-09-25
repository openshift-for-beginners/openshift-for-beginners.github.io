---
layout: page
title: "Lecture 60: Secrets Overview"
permalink: /08-openshift-security/lecture-60-secrets-overview/
---

# Lecture 60: Secrets Overview

**Secrets** are used to store sensitive information, such as passwords, OAuth tokens, and ssh keys.

### Secrets vs. ConfigMaps
- **ConfigMaps** are for plain-text, non-sensitive configuration.
- **Secrets** are for sensitive data. In OpenShift, they are stored as **Base64 encoded** strings.

### Important Note
Base64 is **not encryption**; it is just a way to hide data from plain sight. To truly secure secrets, OpenShift clusters can be configured to encrypt them at rest in Etcd.

---

## Navigation
- [← Previous: Lecture 59]({{ site.baseurl }}/08-openshift-security/lecture-59-demo-config-maps/)
- [Next Topic: Lecture 61 - Demo Secrets →]({{ site.baseurl }}/08-openshift-security/lecture-61-demo-secrets/)