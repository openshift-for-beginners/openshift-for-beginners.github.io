---
layout: page
title: "Local Setup: OpenShift Local (CRC)"
permalink: /03-getting-started-openshift/lecture-06-install-single-node-using-crc/
---

# OpenShift Local (CodeReady Containers)

**OpenShift Local** is the quickest way to get a full OpenShift 4.x cluster running on your local machine.

## Prerequisites
- **RAM:** Minimum 9GB (16GB recommended).
- **CPU:** 4 Virtual Cores.
- **Storage:** 35GB of free space.

## Basic Workflow
1. **Download:** Get the binary from the [Red Hat Console](https://console.redhat.com/openshift/create/local).
2. **Setup:** Run `crc setup` to prepare the virtualization layer.
3. **Start:** Run `crc start` to boot the cluster.
4. **Login:** Use the credentials provided in the terminal to access the UI or CLI.

## Pros & Cons
- ✅ Full control over the cluster (Admin access).
- ✅ No internet connection required after setup.
- ❌ Heavy on system resources.
- ❌ Takes 5–15 minutes to start.

---

## Navigation
- [← Previous: Installation Methods]({{ site.baseurl }}/03-getting-started-openshift/lecture-05-openshift-installation-methods/)
- [Next: Developer Sandbox →]({{ site.baseurl }}/03-getting-started-openshift/lecture-07-install-single-node-using-sandbox/)