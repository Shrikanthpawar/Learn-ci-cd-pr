🔐 CI + Branch Protection Workflow

This repository uses a Pull Request–based workflow to keep the main branch stable and protected.

✅ What is implemented

main branch is protected

Direct pushes to main are blocked

All changes must be done in a feature branch

Changes reach main only via Pull Requests

Every Pull Request must:

Pass GitHub Actions CI (backend + frontend checks)

Have at least one approval

🔁 How to work on this repo

Create a new branch from main

Push code changes to the feature branch

Open a Pull Request → main

CI runs automatically

After CI success and approval, merge is allowed

🎯 Why this setup

Prevents broken code from reaching main

Enforces review and CI validation

Matches real-world DevOps best practices

🧠 One-Line Summary

The main branch only accepts reviewed and CI-validated code through Pull Requests.