# Toolbox: put it on your iPhone (free)

Toolbox is a web app. You put it online for free, then add it to the iPhone Home Screen from Safari. It gets its own icon, opens full screen like a real app, and works without internet after the first time. No App Store and no fees.

## What's in this folder

| File | What it does |
|---|---|
| `index.html` | The whole app |
| `manifest.webmanifest` | The app's name, colors and icon |
| `sw.js` | Lets the app work offline |
| `icons/` | The Home Screen icon |

## Step 1: Put it online (about 5 minutes, free)

The easiest way is **Netlify Drop**:

1. On a computer, unzip this folder.
2. Go to **app.netlify.com/drop**.
3. Drag the whole **toolbox-app** folder onto the page.
4. Netlify gives you a web address like `https://something-random.netlify.app`.
5. Make a free Netlify account so the site stays up. In **Site settings** you can change the name, for example to `toolbox-shalin.netlify.app`.

(GitHub Pages also works and is free.)

## Step 2: Add it to the iPhone

1. Open **Safari** on the iPhone. It must be Safari.
2. Go to the web address from Step 1.
3. Tap the **Share** button (the square with an arrow pointing up).
4. Scroll down and tap **Add to Home Screen**, then tap **Add**.
5. The Toolbox icon appears on the Home Screen. Open it from there.

## Good to know

- **Data stays on the phone.** Appointments and documents are saved only on that iPhone. Nothing is sent anywhere.
- **Always open it from the Home Screen icon.** The Home Screen app and a Safari tab keep separate data, so things saved in one won't appear in the other.
- **Deleting the icon deletes the data.** Removing the app from the Home Screen erases everything saved in it.
- **Sharing:** send the web address to friends. Each person gets their own empty app.

## Updating the app later

1. Change `index.html`.
2. In `sw.js`, change `toolbox-v1` to `toolbox-v2` (and keep going up each time).
3. Drag the folder onto your Netlify site's **Deploys** page again.
4. Close and reopen the app on the iPhone. It updates the next time it has internet.
