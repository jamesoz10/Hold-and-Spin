# Splash Screen Assets

Drop these three files into this folder (exact filenames required):

| Filename                  | What it is                          | Aspect | Notes                                |
| ------------------------- | ----------------------------------- | ------ | ------------------------------------ |
| `splash-bg.png`           | Hero background — casino exterior   | 9:16   | Full-bleed cover, ~1080×1920 ideal   |
| `splash-character.png`    | Showgirl, transparent background    | 2:3    | PNG with alpha channel               |
| `splash-frame.png`        | Ornate gold frame, transparent bg   | 1:1    | Wraps the CASINO JACKPOT teaser      |

## How to upload via GitHub

1. Open the repo → click `assets/`
2. Click **Add file → Upload files**
3. Drag the three images in (rename them to match the table above first)
4. Commit straight to the branch

The splash screen auto-detects missing files and falls back to a procedural
gradient, so partial uploads won't break the page.

## Optimisation tips

- Run the hero through [squoosh.app](https://squoosh.app) → WebP @ 80% quality
  for ~5× smaller file. Then rename `splash-bg.webp` and update the `<img src>`
  in `index.html`.
- The character PNG with transparency stays as PNG (WebP loses alpha quality).
