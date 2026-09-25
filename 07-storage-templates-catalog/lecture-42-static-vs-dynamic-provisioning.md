---
layout: page
title: "Lecture 42: Static vs. Dynamic Provisioning"
permalink: /07-storage-templates-catalog/lecture-42-static-vs-dynamic-provisioning/
---

# Lecture 42: Static vs. Dynamic Provisioning

### Static Provisioning
- **Manual:** An administrator creates PVs manually in advance.
- **Limitation:** If a developer requests 5GB but the only available PV is 100GB, the remaining 95GB is wasted.

### Dynamic Provisioning
- **Automatic:** When a user creates a PVC, OpenShift automatically creates a PV on-the-fly.
- **StorageClass:** This is powered by **StorageClasses**. The PVC specifies which StorageClass to use, and the cluster's storage provider (AWS, Azure, OCS) creates the volume instantly.
- **Benefit:** No manual intervention and no wasted space.

---

## Navigation
- [← Previous: Lecture 41]({{ site.baseurl }}/07-storage-templates-catalog/lecture-41-demo-storage/)
- [Next Topic: Lecture 43 - Demo Dynamic Provisioning →]({{ site.baseurl }}/07-storage-templates-catalog/lecture-43-demo-dynamic-provisioning/)