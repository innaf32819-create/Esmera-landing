# Esmera Landing — Pages Deployment

## Option A — Deploy from branch (simplest, no Actions)
1. Push these files to the **main** branch, root.
2. Go to **Settings → Pages**.
3. **Source:** *Deploy from branch*.  
   **Branch:** `main` — **/ (root)**.
4. Save — Pages will publish automatically.

## Option B — GitHub Actions (Actions tab shows the run)
1. Keep the provided workflow: `.github/workflows/pages.yml`.
2. In **Settings → Pages**, set **Source: GitHub Actions**.
3. Push a commit to `main` — check **Actions** tab for *Deploy static site to Pages*.
4. After it finishes, the link appears in **Settings → Pages** (and in the workflow summary).

### Notes
- `index.html` is at repo root.
- Added `.nojekyll` to avoid any Jekyll interference.
- Asset placeholders are included; replace when ready.
