# Deployment Guide — The Barber Shop

This project deploys to **GitHub Pages** via a GitHub Actions workflow.

## Prerequisites

- Git configured with push access to `https://github.com/aakashpahwa/thebarbershop.git`
- GitHub Pages source set to **GitHub Actions** in repo settings

## How to Deploy

1. **Make your changes** to `index.html` (or any file).

2. **Commit and push to `master`:**
   ```bash
   git add -A
   git commit -m "Your commit message"
   git push origin master
   ```

3. **Deployment is automatic.** The GitHub Actions workflow (`.github/workflows/deploy.yml`) triggers on every push to `master` and deploys the site.

4. **Verify deployment** at: https://aakashpahwa.github.io/thebarbershop/

## Workflow Details

- **File:** `.github/workflows/deploy.yml`
- **Trigger:** Push to `master` branch, or manual `workflow_dispatch`
- **Steps:**
  1. Checks out the repo
  2. Configures GitHub Pages
  3. Uploads the entire repo root as a Pages artifact
  4. Deploys to GitHub Pages

## One-Time Setup (already done)

If Pages is not yet configured on a fresh repo:

1. Go to **GitHub repo → Settings → Pages**
2. Under **Build and deployment → Source**, select **GitHub Actions**
3. Push any commit to `master` to trigger the first deployment

## Manual Trigger

You can also trigger deployment without a code change:

```bash
# Empty commit to re-trigger
git commit --allow-empty -m "Trigger deployment"
git push origin master
```

Or via GitHub UI: **Actions → Deploy to GitHub Pages → Run workflow**

## Live URL

https://aakashpahwa.github.io/thebarbershop/
