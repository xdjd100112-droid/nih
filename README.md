# nih

## Flappy Bird

A Flappy Bird replica that runs in the browser and can be installed as an app. Single HTML file, no dependencies.

**Play in the browser:** open `index.html` directly, or serve the folder with any static file server.

**Controls:** Space to jump on desktop, tap the screen on phones and tablets. Press Space or tap again after "Game Over" to restart.

Your best score is saved in the browser via localStorage.

### Install as an app

The game is a Progressive Web App. When it is served over HTTPS (for example GitHub Pages), it can be installed like a native app and works offline:

- **Android / Chrome / Edge:** press the **Download app** button at the bottom of the screen, or use the browser's "Install app" menu item.
- **iPhone / iPad:** open the page in Safari, tap **Share**, then **Add to Home Screen**.
- **Desktop Chrome / Edge:** press **Download app**, or click the install icon in the address bar.

To host it on GitHub Pages: repository **Settings → Pages**, source "Deploy from a branch", branch `main`, folder `/ (root)`. The game is then available at `https://<user>.github.io/nih/` and installable from there.

Note: the install button and offline support only work over `https://` or `localhost`, not when the file is opened directly from disk.

### Files

- `index.html` – the whole game
- `manifest.webmanifest` – app name, icons and display settings for installation
- `sw.js` – service worker that caches the game for offline play
- `icons/` – app icons
