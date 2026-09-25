---
layout: page
title: "Lecture 59: Demo - Config Maps"
permalink: /08-openshift-security/lecture-59-demo-config-maps/
---

# Lecture 59: Demo - Config Maps

### 1. Create a ConfigMap from the CLI
```bash
oc create configmap my-config --from-literal=APP_COLOR=blue
```

### 2. View the ConfigMap
```bash
oc get configmap my-config -o yaml
```

### 3. Use in a Pod (YAML snippet)
```yaml
env:
  - name: COLOR
    valueFrom:
      configMapKeyRef:
        name: my-config
        key: APP_COLOR
```

---

## Navigation
- [← Previous: Lecture 58]({{ site.baseurl }}/08-openshift-security/lecture-58-config-map-overview/)
- [Next Topic: Lecture 60 - Secrets Overview →]({{ site.baseurl }}/08-openshift-security/lecture-60-secrets-overview/)