---
layout: page
title: "Lecture 48: Voting Application Introduction"
permalink: /07-storage-templates-catalog/lecture-48-voting-app-introduction/
---

# Lecture 48: Voting Application Introduction

To see how all these components (Builds, Deployments, Services, and Routes) work together, we use a multi-tier "Example Voting Application."

### Architecture
1. **Voting App:** Front-end (Python) where users cast votes.
2. **Redis:** In-memory database to store votes temporarily.
3. **Worker:** A .NET app that pulls votes from Redis and pushes them to Postgres.
4. **Postgres:** Persistent SQL database.
5. **Result App:** Front-end (Node.js) to display the final vote counts.

---

## Navigation
- [← Previous: Lecture 47]({{ site.baseurl }}/07-storage-templates-catalog/lecture-47-demo-resource-quota/)
- [Next Topic: Lecture 49 - Demo Voting App →]({{ site.baseurl }}/07-storage-templates-catalog/lecture-49-demo-deploy-voting-app/)