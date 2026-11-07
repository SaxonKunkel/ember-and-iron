# Ember & Iron

An original real-time strategy game in the browser: raise a village, advance through the Village, Town and Castle ages, and lead one of eight historical civilizations against up to three AI rivals.

**Play it here: https://saxonkunkel.github.io/ember-and-iron/**

No account or download needed. It works on computers, tablets and phones.

## Play it like an app on iPhone

1. Open the link above in **Safari**.
2. Tap **Share**, then **Add to Home Screen**.
3. Start the game from the new icon and turn the phone sideways. It runs full screen and also works offline.

On Android, open the link in Chrome and choose **Install app** (or **Add to Home screen**) from the menu.

## What's in the game

- A 96×96 generated map with fog of war, and up to 3 AI rivals (Easy, Normal or Hard; free-for-all or allied against you).
- Four map types: Land, Lakes, Coastal (a central sea) and Islands (every town on its own island). Map visibility can be Hidden, Explored or All visible.
- Eight civilizations: Vikings, English, Germans, French, Mongols, Byzantines, Arabs and Spanish. Each has its own bonuses (one of them at sea) and a unique unit trained at the Keep; the Vikings also get the Longboat.
- Fishing and sea battles: Docks, Fishing Ships, deep-water fish, Fish Traps, War Galleys, Fire Ships, Demolition Ships and Transports. The AI rivals fish, fight for the sea and ship armies across the water.
- Villagers, spearmen, archers, scout riders, knights, monks, battering rams, mangonels and trebuchets. Spearmen beat cavalry, cavalry beat archers, and archers beat spearmen.
- Sheep you can herd (or steal), deer, fish, berries and farms; walls, gates and watchtowers; relics that monks carry to a Monastery.
- Touch controls for phones: tap to select, Box select, pinch to zoom, press and hold any button for its tooltip, and a Hide button that clears the panel off the map.
- Saves stay in the browser. **Export save file** in the Menu lets you move a game to another device.

## How it's built

The whole game is a single file, `index.html`. The art is drawn in code on a canvas, the sound is made with WebAudio, and there are no outside assets. The other files make it installable as an app:

| File | Purpose |
| --- | --- |
| `manifest.webmanifest` | App name, icon and full-screen landscape settings |
| `sw.js` | Service worker: works offline and loads the newest version first when online |
| `icons/` | Home-screen icons |

To publish an update, commit the change and push to `main`. GitHub Pages republishes the site in about a minute.
