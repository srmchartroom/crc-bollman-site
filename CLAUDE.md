# CLAUDE.md — CRC-Bollman-Site

## Project Overview
Bollman Landscape premium website — vanilla HTML/CSS/JS, deployed via Vercel (Git integration).
Pushing to `master` on GitHub triggers Vercel production deployment automatically.

## Deployment Rule
**CRITICAL: After every completed change, you MUST commit and push to GitHub.**
Vercel deploys from the `master` branch on push. Uncommitted or unpushed work means the live site is stale.

Workflow after each change:
1. Check `git status` — look for changes in `assets/`, project root files, and all subdirectories
2. `git add` ALL changed/new files (not just the files you directly edited)
3. `git commit` with a concise message
4. `git push origin master`

Never end a conversation with uncommitted changes sitting in the working tree.

## Git Commit Rules
- **Always check `assets/` and the project root** for new or modified files before committing. These directories often have changes that aren't obvious (new images, config files, etc.).
- Always include the `assets/` folder when committing changes that touch images or other assets.
- Broken images on Vercel deployments are unacceptable — never leave assets uncommitted.
- When in doubt, run `git status` and commit everything that belongs in the repo.
