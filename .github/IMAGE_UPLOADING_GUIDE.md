# StickyPlace Image Uploading Guide

Use this guide when replacing placeholder/local starter images for the site.

## Quick Glossary (Beginner Friendly)

- **Hero image**: the large first image at the top of the Home page.
- **In Action strip**: the row of 3 side-by-side photos under the "In Action" section on Home.
- **Gallery images**: the 6 image tiles on the `/gallery/` page.
- **Uses cards**: image cards on the `/uses/` page for each use case.
- **Macro closeups**: tight zoom photos of tiny components (not wide lab shots). These help show detail like polarity marks, pin orientation, and part spacing.
- **Navbar logo mark**: top-left icon in the website header.
- **Favicon**: tiny icon shown in the browser tab.

## Recommended Formats

- Primary: `.jpg` for photos
- Optional: `.webp` for better compression (if you want smaller files)
- Avoid: `.png` for large photo-heavy images unless transparency is required
- Branding (logo/favicon): `.svg` preferred for crisp scaling

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
- Navbar logo mark (`logo-mark.svg`): design on `256 x 256` viewBox
- Favicon (`stickyplace-favicon.svg`): design on `64 x 64` viewBox

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

Branding assets:

7. `assets/img/stickyplace/logo-mark.svg` (top-left navbar icon)
8. `assets/img/favicon/stickyplace-favicon.svg` (browser tab icon)

## Where Each Image Is Used

- Home page (`/`):
  - Hero section uses `hero-workbench.jpg`
  - "In Action" 3-image strip uses `action-lab-1.jpg`, `action-lab-2.jpg`, `action-lab-3.jpg`
  - "Uses" is on a separate page (`/uses/`)
- Gallery page (`/gallery/`):
  - 6 gallery tiles use a mix of `hero-workbench.jpg`, `action-lab-*`, and `macro-*`
- Uses page (`/uses/`):
  - each card image uses one of `hero-workbench.jpg`, `action-lab-*`, or `macro-orientation.jpg`

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
  - This should be a close-up image (zoomed-in details, not wide scene)
  - Gallery item 5
  - Uses card: checking orientation markings
- `macro-components.jpg`
  - This should be a close-up image (tiny part detail emphasized)
  - Gallery item 6
- `logo-mark.svg`
  - Navbar top-left avatar (set in `_config.yml` via `avatar`)
- `stickyplace-favicon.svg`
  - Browser tab/favicon (set in `_config.yml` via `favicon`)
  - Loaded in `_includes/default/head.liquid`

## Logo / Favicon Design Notes

- Keep both icons visually related (same Pad + Chip motif).
- Use simple bold shapes; tiny details disappear at small sizes.
- Suggested brand colors:
  - Primary blue: `#2563eb`
  - Teal accent: `#14b8a6`
  - Dark ink: `#0f172a`
  - Light surface: `#eff6ff` / `#dbeafe`
- Keep safe padding around icon content:
  - Logo mark: ~10-14% inner margin
  - Favicon: ~8-12% inner margin
- Test favicon legibility at 16x16 and 32x32.

## Quick Workflow

1. Export/crop your images to the recommended dimensions.
2. Compress with quality around `70-82` for JPG.
3. Save using the same filenames listed above.
4. Run local preview and check these pages: `/`, `/gallery/`, `/uses/`.
5. Commit and push. GitHub Pages will automatically use the new files.

## How To Choose Better Photos

- Hero: choose a clean, wide shot with clear subject and workspace context.
- In Action strip: pick 3 photos that show a sequence (setup -> alignment -> transport/use).
- Macro closeups: use bright lighting and strong focus so markings are readable.
- Keep visual style consistent: similar color temperature and brightness across all photos.
