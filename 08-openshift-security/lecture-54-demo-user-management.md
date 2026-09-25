---
layout: page
title: "Lecture 54: Demo - User Management"
permalink: /08-openshift-security/lecture-54-demo-user-management/
---

# Lecture 54: Demo - User Management

### 1. View Users
```bash
oc get users
```

### 2. View Service Accounts
Every project has a `default` service account. To see all of them in your project:
```bash
oc get sa
```

### 3. Create a Group
```bash
oc adm groups new developers
oc adm groups add-users developers user1 user2
```

---

## Navigation
- [← Previous: Lecture 53]({{ site.baseurl }}/08-openshift-security/lecture-53-user-management-overview/)
- [Next Topic: Lecture 55 - RBAC →]({{ site.baseurl }}/08-openshift-security/lecture-55-rbac-roles-bindings/)