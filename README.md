# Clean Content

Clean Content is a personal web app for watching the YouTube videos you chose,
without the recommendations feed. It plays each video inside the app, saves
where you stopped, and lets you take timestamped notes.

Live address after setup: `https://yousefipcm-debug.github.io/clean-content/`

## Features

- Plays videos in a built-in player with no recommendations sidebar or
  comments.
- Covers YouTube's suggestion grid when you pause or finish a video.
- Saves your position automatically and resumes from it.
- Fills in the title, channel, length, and thumbnail from the link.
- Supports playback speeds from 1× to 2× and timestamped notes.
- Installs like an app on macOS, iPhone, and Android.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The app. |
| `manifest.webmanifest` | Lets browsers install the app with its name and icon. |
| `sw.js` | Service worker that keeps the app available offline. |
| `icons/` | App icon in several sizes, plus the editable `logo.svg`. |

## Publish on GitHub Pages

1.  Sign in to [GitHub](https://github.com) as `yousefipcm-debug`.
1.  Click **New repository**.
1.  In the **Repository name** field, enter `clean-content`.
1.  Select **Public**, and then click **Create repository**.
1.  On the new repository page, click **uploading an existing file**.
1.  Drag every file and the `icons` folder from this package into the page.
    Keep the folder structure: `index.html` must be at the top level.
1.  Click **Commit changes**.
1.  Click **Settings** > **Pages**.
1.  Under **Branch**, select `main` and `/ (root)`, and then click **Save**.
1.  Wait one to two minutes, and then open
    `https://yousefipcm-debug.github.io/clean-content/`.

Note: The app doesn't play videos when you open `index.html` directly from
your computer. YouTube requires the page to come from a web address, and
shows **Error 153** otherwise.

## Install the app

- **Mac (Safari):** Open the address, and then click **File** >
  **Add to Dock**.
- **Mac or Windows (Chrome or Edge):** Click the install icon at the right
  of the address bar.
- **iPhone (Safari):** Tap **Share** > **Add to Home Screen**.
- **Android (Chrome):** Tap the menu > **Install app**.

## Your data

Your video list is saved in the browser where you use the app. Each device
keeps its own list.

To move your list to another device, do the following:

1.  On the first device, click **Back up…** in the sidebar.
1.  Send the backup file to the other device.
1.  On the other device, click **Restore…** and select the file.

The repository is public, so anyone can read the app's code. Your video list
stays private because it never leaves your browser.

## Update the app

Upload the new `index.html` to the repository the same way, and commit it.
The app picks up the new version the next time you open it.
