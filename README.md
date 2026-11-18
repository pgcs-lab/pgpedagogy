# Our Apprenticeship Pedagogy

An interactive 3D version of the Primary Goal apprenticeship pedagogy, told as a rainforest rather than a farm.

The pedagogy grows like a single giant tree. Read it from the ground up: what we believe sits in the roots, how we design sits on the forest floor and in the understorey, the learner's experience lives in the canopy, and the result breaks through at the top.

**Live site:** https://pgcs-lab.github.io/pgpedagogy/

## The five layers

| # | Layer | What it shows | Group |
|---|-------|---------------|-------|
| 1 | Roots | What we believe about learning through apprenticeships (eight beliefs) | Curriculum design |
| 2 | Forest floor | Design backwards from the change (a trail you plan from the target end first) | Curriculum design |
| 3 | Understorey | Put each KSB where it is learned best | Curriculum design |
| 4 | Canopy | How learning develops (a five-stage cycle on a looping vine) | Learner experience |
| 5 | Emergent | The result: Knowledge, Skills, Behaviours, Identity, Impact | Outcome |

Our guiding commitment: evidence-informed, inclusive and continuously innovative practice.

## Using it

- **Drag** to look around, **scroll** or pinch to zoom.
- **Click anything that glows** to open that item.
- Use the **dots on the right** to jump between layers, or the arrow keys. `Esc` returns to the whole tree.
- Click the **macaw**. You'll see.

### Auto tour

Click **Play the tour** on the intro screen, or the play button in the bottom-right corner. The camera climbs through every layer and item on a loop. Any click, drag, scroll or key press pauses it.

### Links straight to a layer

Add one of these to the end of the URL:

| Link ending | Opens |
|-------------|-------|
| `#roots` | Layer 1 |
| `#forest-floor` | Layer 2 |
| `#understorey` | Layer 3 |
| `#canopy` | Layer 4 |
| `#emergent` | Layer 5 |
| `#tour` | Kiosk mode (see below) |

### Kiosk mode for events

Open the site with `#tour` on the end, for example `https://pgcs-lab.github.io/pgpedagogy/#tour`. It skips the intro and starts the auto tour. If someone stops to have a play, it picks the tour back up after 45 seconds of nobody touching it. Put the browser in full screen (`F11` on Windows) and leave it running.

## How it's built

It's one file: `index.html`. No build step, no dependencies to install, no framework.

- 3D: [Three.js](https://threejs.org/) 0.160, loaded from jsDelivr
- Font: Plus Jakarta Sans, from Google Fonts
- Everything else (the tree, the forest, the macaw, the fireflies) is generated in code when the page loads

It needs a browser with WebGL, which means any recent Chrome, Edge, Safari or Firefox, desktop or mobile. It also needs an internet connection the first time it loads, to fetch Three.js and the font.

## Editing the words

All of the text lives in one place near the top of the script in `index.html`: the `LEVELS` array. Each layer has a `title`, an `intro`, an optional `callout`, and a list of `items`, each with a title (`t`), an optional subheading (`q`) and a description (`d`).

Change the text, commit, and GitHub Pages will republish within a minute or two. Keep the number of items in each layer the same unless you also want to move things around in the 3D scene.

## Hosting

This repo is published with GitHub Pages from the `main` branch root. On a free GitHub account, Pages only works while the repo is **public**, so leave it that way. There's nothing sensitive in here, just the one HTML file.

To set it up on a fresh repo: **Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)`**.

## Credits

Pedagogy: Primary Goal. 3D version built with Claude.
