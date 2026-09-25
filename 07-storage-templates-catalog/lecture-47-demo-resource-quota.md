---
layout: page
title: "Lecture 47: Demo - Resource Quota"
permalink: /07-storage-templates-catalog/lecture-47-demo-resource-quota/
---

# Lecture 47: Demo - Resource Quota

### 1. View Quotas
```bash
oc get resourcequota
```

### 2. Describe a Quota
This shows you the "Used" vs "Hard" (Limit) values for the project:
```bash
oc describe quota <quota-name>
```

### 3. What happens when a Quota is exceeded?
If you try to create a new Pod that would put the project over its Memory Quota, the `oc create` or `oc apply` command will fail with a "Forbidden" error message.

---

## Navigation
- [← Previous: Lecture 46]({{ site.baseurl }}/07-storage-templates-catalog/lecture-46-resource-quota-overview/)
- [Next Topic: Lecture 48 - Voting App Intro →]({{ site.baseurl }}/07-storage-templates-catalog/lecture-48-voting-app-introduction/)