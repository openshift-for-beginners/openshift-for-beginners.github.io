---
layout: page
title: "Lecture 41: Demo - Storage"
permalink: /07-storage-templates-catalog/lecture-41-demo-storage/
---

# Lecture 41: Demo - Storage

### 1. View Persistent Volumes (Admin only)
```bash
oc get pv
```

### 2. Create and View a PVC
When you deploy a database via the UI, OpenShift often creates a PVC automatically. To see it:
```bash
oc get pvc
```

### 3. Check Binding Status
A PVC will show a status of **Bound** once it has successfully found a piece of storage to use. If it stays **Pending**, it means no suitable volume was found.

---

## Navigation
- [← Previous: Lecture 40]({{ site.baseurl }}/07-storage-templates-catalog/lecture-40-storage-overview/)
- [Next Topic: Lecture 42 - Static vs Dynamic →]({{ site.baseurl }}/07-storage-templates-catalog/lecture-42-static-vs-dynamic-provisioning/)