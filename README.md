# Best Boobies Showcase

A playful neon-club browser game with **illustrated GTA-style contestant portraits**. Watch each girl get a spotlight show-off with jiggle animation, then tap who has the **best boobies**. Offline-friendly, vanilla JS/CSS only, works on GitHub Pages.

**Tone:** cheeky adult club humor. Illustrated characters only — no real people, no celebs, no minors.

## How to play

1. Open `index.html` in a modern browser (or host the folder on GitHub Pages).
2. Tap **START SHOW**.
3. Each round, a fresh random subset of **4–6 of 19** contestants take a spotlight turn with jiggle (A/B flipbook when available, CSS soft-body spring otherwise).
4. When the lineup appears, **tap who has the best boobies**.
5. Hidden crowd favorite = highest appeal score that round (ties broken randomly).
   - **Correct** → big points + streak bonus  
   - **Wrong** → lose a heart + small consolation
6. Game ends after **10 rounds** or **3 misses**. High score saved in `localStorage`.

## Assets

```
assets/01a.png … assets/19a.png   contestant A frames (19 unique)
assets/01b.png, 06b.png, 07b.png  bounce B frames (flipbook jiggle)
assets/stage.png                  neon club stage backdrop
```

All paths are relative so GitHub Pages works out of the box.

## Controls

| Input | Action |
|--------|--------|
| Tap / click | Start, skip showcase, pick, next |
| 🔊 / 🔇 | Mute Web Audio |

Mobile-friendly with large tap targets.

## Tech

- Single `index.html` + `assets/*.png`
- Vanilla JS/CSS — no CDN, no build step
- Preloads images with a loading bar
- Flipbook A/B (~130–170ms) + CSS scaleY/translateY spring for jiggle
