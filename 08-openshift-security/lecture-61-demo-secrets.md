---
layout: page
title: "Lecture 61: Demo - Secrets"
permalink: /08-openshift-security/lecture-61-demo-secrets/
---

# Lecture 61: Demo - Secrets

### 1. Create a Secret
```bash
oc create secret generic db-pass --from-literal=password=redhat
```

### 2. View the Secret (Encoded)
```bash
oc get secret db-pass -o yaml
```

### 3. Decode a Secret
```bash
echo "cmVkaGF0" | base64 --decode
# Output: redhat
```

---

## Navigation
- [← Previous: Lecture 60]({{ site.baseurl }}/08-openshift-security/lecture-60-secrets-overview/)
- [Next Topic: Lecture 62 - Network Policies →]({{ site.baseurl }}/08-openshift-security/lecture-62-network-policies-overview/)