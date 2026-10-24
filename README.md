# SweetMap Walkthrough

A shareable, single-page tour of [SweetMap](https://sweetmap.vercel.app/), the marketplace for home bakers and cake lovers.

Live: https://sweetmap-walkthrough.vercel.app/

## What's on the page

- **Film**: a 50-second animated story, coded in HTML/CSS/JS. It follows one order from the customer's first scroll to the five-star review. It autoplays when scrolled into view and has chapters, a progress bar and full screen.
- **Why SweetMap**: the problems it solves and the occasions it's made for, with photos.
- **Screens at a glance**: phone mockups of the main screens. Tap one to open it in the tour.
- **Try it yourself**: a clickable tour for cake lovers and bakers, plus a "How it works" view.
- **Get started**: setup steps for each side (open the link, add to home screen, sign up), with mockups and photo tips for bakers.
- **FAQ** and share buttons (WhatsApp, copy link).

Deep links: `#film`, `#why`, `#screens`, `#tour`, `#setup`, `#faq`, and `#customer`, `#baker`, `#platform` to open a specific tour.

## Editing

Everything lives in `index.html`; there's no build step. Push to `main` and Vercel redeploys.

- Photos are hot-linked from Unsplash. Swap an ID in the `PH` map to change a photo everywhere.
- The film's scenes are in the `FILM` array: each has a duration, a `build()` that returns the scene markup, and timed `cues`.
- The tour steps are in `FLOWS`.

Screens are recreated for the tour with example bakers and orders.
