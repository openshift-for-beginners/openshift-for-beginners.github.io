---
layout: page
title: "Users and Identity Basics"
permalink: /04-openshift-concepts-projects-users/users-overview/
---

# Users and Identity Basics

OpenShift is designed for multi-user environments. It manages "who can do what" through Users and Groups.

## Types of Users
1. **Regular Users:** Humans interacting with the cluster via UI or CLI.
2. **System Users:** Created automatically by the cluster for internal tasks.
3. **Service Accounts:** Special users used by applications/pods to interact with the OpenShift API.

## Identity Providers (IDPs)
OpenShift doesn't store passwords internally. It connects to external Identity Providers like:
- **HTPasswd:** A simple file-based list of users (common for labs).
- **LDAP / Active Directory:** Enterprise standard.
- **GitHub / Google:** OAuth-based login.

## Commands to Check Identity
- **Who am I?** `oc whoami`
- **Context:** `oc config view` (shows current cluster and user connection details).

---

## Navigation
- [← Previous: Understanding Projects]({{ site.baseurl }}/04-openshift-concepts-projects-users/projects-overview/)
- [Next: Knowledge Check →]({{ site.baseurl }}/04-openshift-concepts-projects-users/quiz/)