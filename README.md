# Letternoxd

**Mark films "Not interested," add badges.** A free, open-source extension for Letterboxd, with a one-click watchlist button too.

Letterboxd lets you hide films you've watched or watchlisted, but there's no way to say "I've seen the trailer, I'm never watching this." Letternoxd adds that.

> Unofficial. Letternoxd is a fan-made browser extension and isn't affiliated with or endorsed by Letterboxd.

## What it does

- **Not interested (⃠)**: hover any poster and click ⃠ in the top-right corner. On a film's own page, use **Nah** next to Watch / Like / Watchlist.
- **Show / Fade / Hide not interested**: three new choices in Letterboxd's filter (eye) menu, next to its own filters. Faded films keep a white ⃠ so you can tell why.
- **One-click watchlist**: a watchlist button sits in each poster's hover bar, so you no longer need the "…" menu. The "…" button moves to the top-left corner.
- **Status badges**: a small badge in each poster's top-left corner: green eye for seen, orange heart for loved, blue clock for your watchlist (with a thin blue border). Turn them on or off with "Show status badges" in the eye menu.
- **Coloured fades**: with Letterboxd's own "Fade watched films" on, seen and loved posters fade toward dark green / dark orange instead of black, so you can still tell them apart.
- **Changed your mind?** Watching, loving or watchlisting a film takes it off "not interested" automatically, and its ⃠ stays greyed out until you undo those.
- **Seen it? Off the watchlist.** Marking a film watched (or loving it) takes it off your watchlist too.
- **Instant**: everything updates the moment you click, and films you've marked are hidden before the page finishes drawing.

## Where your data lives

Films you mark are saved to a **private list called "Not Interested"** on your own Letterboxd account (the extension creates it the first time you click ⃠). Nothing is lost if you reinstall or switch computers, and you can edit the list on Letterboxd like any other.

Letternoxd collects nothing. It only talks to letterboxd.com, as you, and keeps its settings in your browser.

## Install

**From the Chrome Web Store** (Chrome, Arc, Brave, Edge): *link coming soon*.

**From this repository:**

1. Download this repository (green **Code** button → **Download ZIP**) and unzip it somewhere permanent.
2. Go to `chrome://extensions` (Arc: `arc://extensions`, Brave: `brave://extensions`, Edge: `edge://extensions`).
3. Turn on **Developer mode** (top right), click **Load unpacked**, and choose the unzipped folder.
4. Reload any open Letterboxd tabs.

To update, replace the files, click ↻ on the extension's card, and reload Letterboxd.

## Good to know

- The filter works after each page loads, so a page may show a few fewer posters than usual. A note under the grid says how many were hidden.
- Page totals (e.g. "1,234 films") still count hidden films.
- Desktop browsers only; the Letterboxd apps aren't affected.
- It relies on how Letterboxd's website works today, so a redesign may need an update.

## Troubleshooting

Open the browser console on a Letterboxd page and run:

- `lbNotInterested.state()` to see what the extension knows (your list, saved films, settings).
- `lbNotInterested.resync()` to re-read your "Not Interested" list now. It otherwise refreshes every 6 hours, when you return to a tab after 10 minutes, and whenever you click ⃠.

## License

MIT
