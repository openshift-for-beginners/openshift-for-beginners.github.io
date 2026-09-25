---
layout: page
title: "Lecture 69: SCM for Beginners"
permalink: /09-conclusion-appendix/lecture-69-scm-overview/
---

# Lecture 69: Source Code Management (SCM) Overview

Before OpenShift can build your code, it needs to be stored in a **Source Code Management (SCM)** system.

### What is Git?
Git is the most popular version control system. It allows you to:
- Track changes to your code.
- Revert to previous versions.
- Collaborate with other developers.

### Common SCM Platforms
- **GitHub:** The most popular public hosting service.
- **GitLab:** Often used in enterprise environments for self-hosted Git.
- **Bitbucket:** Another popular enterprise alternative.

### OpenShift Integration
OpenShift uses **Webhooks** to listen for changes in these SCM platforms. When you "push" code to a repository, the SCM platform notifies OpenShift to start a new build automatically.

---

## Navigation
- [← Previous: Lecture 68]({{ site.baseurl }}/09-conclusion-appendix/lecture-68-conclusion/)
- [Next Topic: Lecture 70 - Demo GitLab Setup →]({{ site.baseurl }}/09-conclusion-appendix/lecture-70-demo-gitlab-setup/)