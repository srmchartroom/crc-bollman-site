# CLAUDE.md — CRC-Bollman-Site

## Project Overview
Bollman Landscape premium website — vanilla HTML/CSS/JS, deployed via Vercel (Git integration).
Pushing to `master` on GitHub triggers Vercel production deployment automatically.

## Deployment Rule
**CRITICAL: After every completed change, you MUST commit and push to GitHub.**
Vercel deploys from the `master` branch on push. Uncommitted or unpushed work means the live site is stale.

Workflow after each change:
1. `git add` the changed files (include `assets/` if any assets were added/modified)
2. `git commit` with a concise message
3. `git push origin master`

Never end a conversation with uncommitted changes sitting in the working tree.

## Git Commit Rules
- Always include the `assets/` folder when committing changes that touch images or other assets.
- Broken images on Vercel deployments are unacceptable — never leave assets uncommitted.
