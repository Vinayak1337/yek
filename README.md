# YEK

A dark, single-page streetwear site for YEK. Mochi, a grumpy white cat holding a coffee mug, sits in a 3D hero and follows your cursor. Press **Shop the drop** and he grabs a dark wrapper curtain, drags it across the screen and reveals the collection in a physics-based carousel.

Everything lives in `index.html`: HTML, CSS and JavaScript in one file.

## Run it

Open `index.html` in a browser, or serve the folder:

```bash
node serve.mjs
```

Then visit http://127.0.0.1:5180.

The page loads Three.js, GSAP and Google Fonts from CDNs, so it needs a network connection. Without WebGL, the shop still opens with a plain slide-in.

## What's inside

- **Hero:** a pitch-black stage with an amber glow, the fluffy 3D cat (shell-rendered fur) whose head and eyes track the cursor, a two-line headline, a flat Shop the drop button, and three cards for the next drops with live countdowns.
- **Transition:** the cat raises a paw, grabs the curtain's edge, hops left dragging the cloth, and flings it across. The curtain stays as the shop's backdrop.
- **Shop:** eight garments drawn in SVG, in a carousel you can drag, flick, scroll or page with the arrow keys. It has momentum, spring snapping and rubber-band edges. Swatches recolour each piece and Add updates the bag.
- **Drops:** a calendar with the live drop and three upcoming ones, each with a ticking countdown and a Remind me toggle shared with the hero cards.
- **Lookbook:** six outfits built from the shop's pieces, in the same physics carousel. Add the look puts every piece in the bag.
- **Nap Club:** member perks, two meet-ups you can save a spot at, and a join form with email validation and a size picker. Mochi falls asleep on this page.

Every page lives behind the curtain at its own hash route (`#/shop`, `#/drops`, `#/lookbook`, `#/nap-club`), so links, back and forward and deep links all work. Moving between pages keeps the curtain up: its edge flaps and Mochi hops over to the new header. The YEK logo, Back to Mochi and Escape all return to the hero.

Product names, prices, drop dates, perks and meet-ups are placeholder content. The join form and reminders don't send anything; the form only remembers you in this browser.
