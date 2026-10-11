# CJS '96 Reunion 2.0 Awards Night

Static landing page ready for GitHub Pages.

## What changed
This version is more **cinematic / movie-trailer style**:
- full-screen moving background images with slow zoom and crossfades
- dramatic headline treatment
- trailer-style light effects and overlays
- no sound button (can be added when music is supplied)
- countdown to voting and awards night

## Publish
1. Create a GitHub repository (for example `cjs96-awards`).
2. Upload the contents of this folder to the repository root. This build is self-contained for previewing: the HTML already embeds the photos, so it should open correctly even when viewed directly.
3. Go to **Settings → Pages → Build and deployment → Deploy from a branch**, select `main` and `/(root)`, and save.
4. Your site will appear at `https://YOUR-USERNAME.github.io/cjs96-awards/`.

## Customize images
- Replace the current `images.unsplash.com/...` URLs in `index.html` with your real reunion photos.
- Better option: create an `images/` folder in your repo and use your own photos, for example:
  - `images/dance.jpg`
  - `images/pool.jpg`
  - `images/karaoke.jpg`
  - `images/friends.jpg`

## Add background sound
Browsers typically block autoplay audio with sound. This build currently has no sound button.

To add sound:
1. Create a folder named `audio/`
2. Add your soundtrack as `audio/trailer-theme.mp3`
3. Keep it short, instrumental, and royalty-safe if you plan to share publicly.

## Voting link
- Set `const VOTING_URL = '';` in `index.html` to your Google Form or voting site URL.
- Until that is added, the button does not collect votes.

## Timing
- The current countdown assumes midnight **India Standard Time** on October 12 and October 17, 2026.
- Change `votingStart` and `awardsStart` in `index.html` if needed.

## Important note
GitHub Pages is static hosting. Public votes should go to an external form/service or a separate backend. The page itself does not store votes.

## Included reunion photos
The `images/` folder now includes nine real reunion photos from the chat, used in the cinematic background and moving montage. No stock photo URLs remain. Audio is optional: add `audio/trailer-theme.mp3` to enable the Play Trailer Sound button.


## Members-only welcome screen (casual deterrent)
- The current shared password is in `const REUNION_PASSWORD` inside `index.html`. Keep it in your own password manager; do not publish it in the README. This is a casual deterrent only.
- A visitor enters the password once per browser tab session.
- Right-click and drag on images are discouraged. Screenshots, saving through developer tools, and direct file access remain possible.
- **Important:** This is NOT secure access control: the password and embedded reunion photos remain visible in the public page source. GitHub Pages is public. For true privacy, use authenticated hosting.
