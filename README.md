# CI + Branch Protection Workflow

# Overview
This repository uses a Pull Request–based workflow to keep the main branch stable and protected.

# What Is Implemented
- The main branch is protected
- Direct pushes to main are blocked
- All changes must be done in a feature branch
- Changes reach main only via Pull Requests
- Every Pull Request must pass GitHub Actions CI (backend + frontend checks)
- At least one approval is required before merging

# How to Work on This Repository
1. Create a new branch from main
2. Push code changes to the feature branch
3. Open a Pull Request targeting main
4. CI runs automatically
5. After CI success and approval, the Pull Request can be merged

# Why This Setup Exists
- Prevents broken code from reaching main
- Enforces code review and CI validation
- Matches real-world DevOps best practices

# One-Line Summary
The main branch only accepts reviewed and CI-validated code through Pull Requests.



# PR + CI + Branch Protection

This is the real, enterprise-grade “hook” behavior.

How it works (correct flow):
Developer pushes → feature branch
↓
Pull Request created
↓
CI automatically runs (build/test)
↓
GitHub BLOCKS merge
↓
Waits for:
  - CI success
  - Required reviews (Dev / Lead / DevOps)
↓
Merge allowed