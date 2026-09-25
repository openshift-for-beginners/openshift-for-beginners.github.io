layout: page
title: "Lecture 15: Demo - Projects and Users"
permalink: /04-openshift-concepts-projects-users/lecture-15-demo-projects-and-users/
---

# Lecture 15: Demo - Projects and Users

### Step 1: Verify Identity
```bash
oc whoami
```

### Step 2: Create a Project
```bash
oc new-project my-first-project
```

### Step 3: Switch Projects
```bash
oc project <target-project-name>
```

### Step 4: List Resources
```bash
oc get all
```

---

## Navigation
- [← Previous: Lecture 14]({{ site.baseurl }}/04-openshift-concepts-projects-users/lecture-14-projects-and-users/)
- [Next Topic: Lecture 16 - Quiz →]({{ site.baseurl }}/04-openshift-concepts-projects-users/lecture-16-quiz-projects-and-users/)