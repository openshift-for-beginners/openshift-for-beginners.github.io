---
layout: page
title: "Lecture 43: Demo - Dynamic Provisioning"
permalink: /07-storage-templates-catalog/lecture-43-demo-dynamic-provisioning/
---

# Lecture 43: Demo - Dynamic Provisioning

### 1. List Available Storage Classes
```bash
oc get sc
```

### 2. Request Storage via PVC
You can create a YAML file for a PVC that uses a specific storage class:
```yaml
apiVersion: v1
kind: PersistentVolumeClaim
metadata:
  name: my-dynamic-pvc
spec:
  accessModes:
    - ReadWriteOnce
  resources:
    requests:
      storage: 1Gi
  storageClassName: standard-csi # Example class
```

### 3. Verify
After applying the YAML, run `oc get pv,pvc`. You will see that a PV was created automatically to match your PVC.

---

## Navigation
- [← Previous: Lecture 42]({{ site.baseurl }}/07-storage-templates-catalog/lecture-42-static-vs-dynamic-provisioning/)
- [Next Topic: Lecture 44 - Resource Allocation →]({{ site.baseurl }}/07-storage-templates-catalog/lecture-44-resource-allocation-cpu-ram/)