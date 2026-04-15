# StickyPlace Image Uploading Guide

Use this guide when replacing placeholder/local starter images for the site.

## Recommended Formats

- Primary: `.jpg` for photos
- Optional: `.webp` for better compression (if you want smaller files)
- Avoid: `.png` for large photo-heavy images unless transparency is required

## File Size Targets

- Hero image: `<= 450 KB`
- Gallery and Uses images: `<= 300 KB` each
- Absolute max per image: `<= 700 KB` (try to stay lower)

## Recommended Dimensions

- Hero (`hero-workbench.jpg`): `1600 x 1000` (or similar 16:10 / 16:9)
- In Action strip (`action-lab-1/2/3.jpg`): `1200 x 750`
- Gallery (`*_gallery` slots listed below): `1200 x 900` (4:3 works best)
- Uses cards (same source files reused): `1200 x 700` to `1200 x 800`
- Macro closeups (`macro-*.jpg`): at least `1000px` wide

## Naming Convention

- Keep lowercase, hyphenated names.
- Reuse these exact filenames so no page code changes are needed.

## Current Files To Replace

Place your updated photos in `assets/img/stickyplace/` with these names:

1. `hero-workbench.jpg`
2. `action-lab-1.jpg`
3. `action-lab-2.jpg`
4. `action-lab-3.jpg`
5. `macro-orientation.jpg`
6. `macro-components.jpg`

## Where Each Image Is Used

- `hero-workbench.jpg`
  - Home hero
  - Gallery item 1
  - Uses card: staging components
- `action-lab-1.jpg`
  - Home In Action strip (image 1)
  - Gallery item 3
  - Uses card: reducing hand fatigue
- `action-lab-2.jpg`
  - Home In Action strip (image 2)
  - Gallery item 2
  - Uses card: organizing resistors/capacitors
- `action-lab-3.jpg`
  - Home In Action strip (image 3)
  - Gallery item 4
  - Uses card: transporting parts
- `macro-orientation.jpg`
  - Gallery item 5
  - Uses card: checking orientation markings
- `macro-components.jpg`
  - Gallery item 6

## Quick Workflow

1. Export/crop your images to the recommended dimensions.
2. Compress with quality around `70-82` for JPG.
3. Save with the same filenames above into `assets/img/stickyplace/`.
4. Commit and push. GitHub Pages will automatically use the new files.
