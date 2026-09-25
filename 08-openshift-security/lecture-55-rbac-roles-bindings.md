---
layout: page
title: "Lecture 55: RBAC - Roles and Bindings"
permalink: /08-openshift-security/lecture-55-rbac-roles-bindings/
---

# Lecture 55: RBAC - Roles and Bindings

**RBAC (Role-Based Access Control)** determines "Who can do What, and Where."

### Core Components
1. **Roles:** Define a set of permissions (e.g., "can read pods").
    - **Role:** Specific to a Project.
    - **ClusterRole:** Cluster-wide permissions.
2. **Bindings:** Connect a User/Group/SA to a Role.
    - **RoleBinding:** Grants permissions within a specific Project.
    - **ClusterRoleBinding:** Grants permissions across the entire cluster.

### Common Default Roles
- **admin:** Full control within a project.
- **edit:** Can create/delete most objects in a project but cannot manage permissions.
- **view:** Read-only access to a project.

---

## Navigation
- [← Previous: Lecture 54]({{ site.baseurl }}/08-openshift-security/lecture-54-demo-user-management/)
- [Next Topic: Lecture 56 - Demo RBAC →]({{ site.baseurl }}/08-openshift-security/lecture-56-demo-rbac/)