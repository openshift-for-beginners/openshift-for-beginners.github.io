---
layout: page
title: "Lecture 70: Demo - GitLab Setup"
permalink: /09-conclusion-appendix/lecture-70-demo-gitlab-setup/
---

# Lecture 70: Demo - GitLab Setup

This demo covers how to set up a Git repository to use with OpenShift.

### 1. Create a Repository
Log into GitLab (or GitHub) and create a new project. Initialize it with a simple README or a "Hello World" application.

### 2. Generate a Personal Access Token
If your repository is private, OpenShift needs a token to "read" your code.
- Go to User Settings → Access Tokens.
- Create a token with `read_repository` permissions.

### 3. Create a Secret in OpenShift
In OpenShift, save these credentials so the build can access the repo:
```bash
oc create secret generic git-repo-creds \
    --from-literal=username=<user> \
    --from-literal=password=<token> \
    --type=kubernetes.io/basic-auth
```

### 4. Link the Secret to a Build
When creating your app, you point it to this secret so that the `BuildConfig` can successfully clone the code.

---

## Navigation
- [← Previous: Lecture 69]({{ site.baseurl }}/09-conclusion-appendix/lecture-69-scm-overview/)
- [Next Topic: Lecture 71 - CI/CD Overview →]({{ site.baseurl }}/09-conclusion-appendix/lecture-71-cicd-overview/)