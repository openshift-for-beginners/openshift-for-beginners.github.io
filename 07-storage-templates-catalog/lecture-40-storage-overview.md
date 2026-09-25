---
layout: page
title: "Lecture 40: Storage Overview"
permalink: /07-storage-templates-catalog/lecture-40-storage-overview/
---

# Lecture 40: Storage Overview

Containers are ephemeral, meaning data stored inside them is lost when the container restarts. To save data permanently, OpenShift uses a persistent storage system.

### Core Storage Objects
1. **Persistent Volume (PV):** A piece of storage in the cluster that has been provisioned by an administrator. It is a cluster-wide resource.
2. **Persistent Volume Claim (PVC):** A request for storage by a user. Think of it as a "voucher" that a Pod uses to claim a PV.
3. **StorageClass:** A way for administrators to describe the "classes" of storage they offer (e.g., "fast-ssd" vs "slow-hdd").

### The Workflow
- Admin creates a **Persistent Volume**.
- Developer creates a **Persistent Volume Claim**.
- OpenShift **binds** the PVC to a suitable PV.
- The **Pod** uses the PVC to mount the storage.

---

## Navigation
- [← Back to Section Index]({{ site.baseurl }}/07-storage-templates-catalog/)
- [Next Topic: Lecture 41 - Demo Storage →]({{ site.baseurl }}/07-storage-templates-catalog/lecture-41-demo-storage/)