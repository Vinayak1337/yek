# YEK

A dark, single-page streetwear site for YEK. Mochi, a grumpy white cat holding a coffee mug, sits in a 3D hero and follows your cursor. Press **Shop now** and he grabs a dark wrapper curtain, drags it across the screen and reveals the collection in a physics-based carousel.

Everything lives in `index.html`: HTML, CSS and JavaScript in one file.

## Run it

Open `index.html` in a browser, or serve the folder:

```bash
node serve.mjs
```

Then visit http://127.0.0.1:5180.

The page loads Three.js, GSAP and Google Fonts from CDNs, so it needs a network connection. Without WebGL, the shop still opens with a plain slide-in.

## What's inside

- **Hero:** a pitch-black stage with an amber glow, the fluffy 3D cat (shell-rendered fur) whose head and eyes track the cursor, stacked type, a glowing Shop now button, and three glass cards teasing upcoming drops with live countdowns.
- **Transition:** the cat raises a paw, grabs the curtain's edge, hops left dragging the cloth, and flings it across. The curtain stays as the shop's backdrop.
- **Shop:** eight garments drawn in SVG, in a carousel you can drag, flick, scroll or page with the arrow keys. It has momentum, spring snapping and rubber-band edges. Swatches recolour each piece and Add updates the bag.

Product names, prices and drop dates are placeholder content.
