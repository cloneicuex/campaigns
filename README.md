# LIC 2026 campaign scheduler

This repository contains the protected GitHub Actions schedule for the Leadership & Impact Conference 2026 daily prayer emails.

- Production runs: 6:30 AM America/Chicago, September 20–October 22, 2026
- Authentication: short-lived GitHub OIDC identity token; no campaign credential is stored in this repository
- Delivery safeguards: the conference application selects only opted-in registrants and prevents duplicate sends for the same campaign day
- Manual runs: use **Actions → Send LIC daily countdown → Run workflow** and choose **dry-run** unless an authorized recovery send is intended

The workflow exits without contacting the campaign outside the 2026 campaign window.
