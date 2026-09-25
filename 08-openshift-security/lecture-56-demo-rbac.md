---
layout: page
title: "Lecture 56: Demo - RBAC"
permalink: /08-openshift-security/lecture-56-demo-rbac/
---

# Lecture 56: Demo - RBAC

### 1. Add a role to a user in a project
To give "user1" the ability to view everything in the current project:
```bash
oc policy add-role-to-user view user1
```

### 2. Add a role to a group
```bash
oc policy add-role-to-group edit developers
```

### 3. View Bindings
To see who has what permissions in the current project:
```bash
oc get rolebindings
```

---

## Navigation
- [← Previous: Lecture 55]({{ site.baseurl }}/08-openshift-security/lecture-55-rbac-roles-bindings/)
- [Next Topic: Lecture 57 - User Contexts →]({{ site.baseurl }}/08-openshift-security/lecture-57-demo-user-contexts/)