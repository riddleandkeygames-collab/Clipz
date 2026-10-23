# Clips

A magic app that looks like an ordinary video viewer. A video plays of a whiteboard being uncovered, and the spectator's choice is already written on it. You pick which of up to 99 outs appears by where you tap while pausing and playing the video.

It's a web app: one copy works on both iPhone and Android, installs to the home screen like a normal app, and runs offline once it has been opened with a signal.

## Put it online (once)

The app has to be served over HTTPS for phones to install it. GitHub Pages does this for free:

1. On GitHub, open this repository and go to **Settings → Pages**.
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**, the branch to **main** and the folder to **/ (root)**, then **Save**.
3. After a minute or two the page shows the address, which will be `https://riddleandkeygames-collab.github.io/Clipz/`.

## Install on iPhone

1. Open the address in **Safari** (it must be Safari, not Chrome or another browser).
2. Tap **Share**, then **Add to Home Screen**, then **Add**.
3. Open it from the home screen once while you have signal, so it saves itself for offline use.

## Install on Android

1. Open the address in **Chrome**.
2. Tap **Install app** when it's offered, or the **⋮** menu then **Install app** (on some phones, **Add to Home screen**).
3. Open it once while you have signal.

## Using it

- Hold anywhere on the video for 1.5 seconds to open the magician settings. Everything is explained there.
- The secret keypad is the whole screen in four rows: 1 2 3 / 4 5 6 / 7 8 9 / 0.
- Play, pause, play: tap to play, tap to pause (where you tap is the first digit), tap to play again (where you tap is the second digit).
- Effects, outs, pictures and your own videos are saved on each phone separately.
- A blank playing card in your own video can become the chosen card: add the video, open Placement, tick **Whole card face**, go to a frame where the card is clear and tap **Find the card**. Film it with the phone on a stand and nothing in front of the card at the end.

## Files

- `index.html`: the whole app
- `sw.js`, `manifest.webmanifest`, `icon-*.png`: installing and working offline
- `cloth.mp4`, `towel.mp4`, `board.mp4`, `station.mp4`, `cardm.mp4`, `cardf.mp4`, `shelf.mp4` and their `.jpg` stills: the built-in videos (`*-track.json` holds the tracked corners for the moving ones)
- `card-7h.png`, `sym/`, `doodle/`: the built-in pictures, symbols and doodles
- `faces/01.jpg` to `faces/53.jpg`: the card faces for the card-in-hand videos (Clubs, Hearts, Spades, Diamonds, Ace to King, then the Joker). They are Adrian Kennard's playing card designs (www.me.uk/cards), released into the public domain (CC0), taken from the @letele/playing-cards package.
