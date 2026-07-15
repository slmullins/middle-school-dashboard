# Middle School Options Dashboard (2027–2028)

An interactive, single-file dashboard comparing Houston middle school options for 6th grade:
comparison table, school profiles, master timeline, application checklist (saved in your browser),
and shared tests/forms. All data is sourced from each school's official website.

**The whole app is one file: `index.html`.** No build step, no dependencies — it runs offline in any browser.

---

## Put it on GitHub Pages

You only need the file named **`index.html`** in the repo. (The `README.md` is optional.)

### Option A — GitHub website, no command line (easiest, ~2 min)

1. Go to <https://github.com/new> and create a new repository.
   - Name it anything, e.g. `middle-school-dashboard`.
   - Set it to **Public** (required for free GitHub Pages).
   - Leave "Add a README" unchecked. Click **Create repository**.
2. On the new repo page, click **uploading an existing file** (or **Add file → Upload files**).
3. Drag in **`index.html`** (and `README.md` if you like). Click **Commit changes**.
4. Go to **Settings → Pages** (left sidebar).
5. Under **Build and deployment → Source**, choose **Deploy from a branch**.
6. Set **Branch** to `main` and folder to `/ (root)`. Click **Save**.
7. Wait ~1 minute, then refresh. Your live site appears at:
   `https://<your-username>.github.io/middle-school-dashboard/`

### Option B — Command line (if you use git locally)

```bash
# in the folder that contains index.html
git init
git add index.html README.md
git commit -m "Add middle school dashboard"
git branch -M main

# create the repo first at https://github.com/new, then:
git remote add origin https://github.com/<your-username>/middle-school-dashboard.git
git push -u origin main
```

Then enable Pages: **Settings → Pages → Source: Deploy from a branch → main / root → Save.**

---

## Updating it later

Replace `index.html` with a new version (re-upload on the website, or `git add/commit/push`).
GitHub Pages redeploys automatically within a minute or two.

## Notes

- The checklist saves your check-offs in **your browser's** local storage — they stay on whatever
  device/browser you use, and aren't uploaded anywhere.
- HISD School Choice dates for 2027–28 were not yet published when this was built; those entries are
  marked "not yet posted" and show expected timing based on the prior two cycles. Re-verify before applying.
