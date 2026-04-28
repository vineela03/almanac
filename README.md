# The Almanac — Setup Guide (Built using Claude)

A personal task app for your iPhone (and laptop). Hosted free on GitHub Pages.

---

## What you're about to do

1. Create a GitHub account (free, ~2 min)
2. Upload these 7 files to a new repository (~3 min)
3. Turn on GitHub Pages (~1 min)
4. Add it to your iPhone Home Screen (~1 min)

Total: about 10 minutes. After that, opening the app is one tap, like any native app.

---

## Step 1 — Create a GitHub account

Go to **github.com** and sign up. Pick any username — you'll see it in your app's URL later.

## Step 2 — Create a new repository

After signing in:

1. Click the **+** in the top-right corner → **New repository**
2. **Repository name**: `almanac` (or anything you like, lowercase, no spaces)
3. Set it to **Public** (required for free Pages hosting)
4. **Don't** check "Add a README" — you already have one
5. Click **Create repository**

## Step 3 — Upload the files

On the new empty repository page, click the **"uploading an existing file"** link (it's in the middle of the page, in the quick-setup section).

Drag all 7 files from the `almanac` folder into the upload area:

- `index.html`
- `manifest.json`
- `service-worker.js`
- `icon-180.png`
- `icon-192.png`
- `icon-512.png`
- `icon-512-maskable.png`

Scroll down, click **Commit changes**.

## Step 4 — Turn on GitHub Pages

1. Click the **Settings** tab (top of the repository page)
2. In the left sidebar, click **Pages**
3. Under **Source**, choose **Deploy from a branch**
4. Under **Branch**, select **main** and **/ (root)**, then click **Save**
5. Wait about 1–2 minutes. Refresh the Pages settings page until you see a green box at the top

That URL is your app. Bookmark it — it's permanent and free.

## Step 5 — Add to your iPhone Home Screen

This step is **required** for notifications to work on iPhone.

1. Open the URL in **Safari** on your iPhone (must be Safari, not Chrome)
2. Tap the **Share button** (square with up-arrow) at the bottom of the screen
3. Scroll down and tap **Add to Home Screen**
4. Tap **Add** in the top-right

You'll now have an Almanac icon on your Home Screen. Tap it — the app opens full-screen, no Safari bars, no address bar. Feels native.

The first time you open it from the Home Screen, it'll ask permission for notifications. Tap **Allow**.

---

## How reminders work on iPhone

iOS is strict about background activity, so here's the honest layout:

- **When the app is open**: Reminders fire as system notifications + a soft chime. Reliable.
- **When the app is closed**: iOS may suspend it before a reminder fires. To handle this, the app tracks when you last opened it. Anything that came due while you were away appears in a **"While you were away"** banner at the top the next time you open the app — so nothing is ever missed silently.
- **Best habit**: open the app once in the morning to clear yesterday's banner and see today's plan.

---

## Updating the app later

If you want changes (new features, different colors, bug fixes):

1. Click the file you want to replace (e.g. `index.html`)
2. Click the pencil icon → delete its contents → paste the new contents → **Commit changes**

GitHub Pages will redeploy automatically in 1–2 minutes. Your iPhone may need a hard refresh: close the app completely (swipe up from app switcher), then reopen.

---

## Troubleshooting

**"My site isn't live yet"** — Pages can take up to 5 minutes the first time. Refresh the Settings → Pages page; the green box appears when ready.

**"It loaded but looks unstyled"** — give it 10 seconds; Tailwind compiles in-browser on first load. If it persists, check that all 7 files uploaded successfully.

**"Notifications never appear"** — Make sure you opened the app from the Home Screen icon (not Safari), and that you tapped Allow when prompted. You can also check iPhone Settings → Notifications → Almanac.

**"My tasks disappeared"** — Tasks are stored in your phone's browser storage, scoped to the app. Clearing Safari data or reinstalling the home screen icon can wipe them. Your tasks are not synced between devices unless you export them.

---

Enjoy your almanac.
