# The Barber Shop

A nostalgic, single-page website designed for modern barber shops to display on screens — evoking the old days of weekend visits to the barber with old Hindi songs playing on a radio.

## Concept

The site is built around a central **old wooden radio** UI that plays curated YouTube playlists of classic Hindi film songs. It's meant to run as an ambient display in barber shops, bringing back the warmth of the golden era.

## Features

- **Animated Hair & Beard Silhouette Logo** — A faceless silhouette with windblown hair and beard strands, floating wind particles
- **Vintage Wooden Radio** — The centerpiece UI element with:
  - Speaker grille with ambient glow
  - Green LED marquee display scrolling current song info (right-to-left)
  - Tuning and volume dials (animated rotation)
  - Frequency bar with sweeping red needle
  - Waveform visualizer bars
  - AM/FM/SW mode buttons and mute toggle
  - Antenna with wobble animation
  - Subtle vibration animation simulating sound output with tempo variation
- **YouTube Playlist Integration** — Six curated playlists of old Hindi film songs (Kishore Kumar, Lata Mangeshkar, Mohammed Rafi, Mukesh, Asha Bhosle, Mixed)
- **Embedded Player** — Slide-up player bar with YouTube iframe embed
- **Atmospheric Design** — Sepia vignette background, film grain overlay, wallpaper pattern, floating scissors decorations

## Tech Stack

- Single HTML file (no build tools)
- Pure CSS animations (no JS animation libraries)
- Google Fonts: Playfair Display, Special Elite, IM Fell English
- YouTube IFrame embed API for playlist playback

## Usage

Open `barber-shop.html` in any modern browser. Click a playlist card to start playing music through the embedded YouTube player.

Ideal for:
- Barber shop display screens
- Waiting area ambience
- Nostalgic themed events

## Deployment

The site is deployed to GitHub Pages via a GitHub Actions workflow. Every push to `master` triggers automatic deployment.

**Live URL:** `https://aakashpahwa.github.io/thebarbershop/`

### Setup (one-time)

In your GitHub repo settings:
1. Go to **Settings → Pages**
2. Under **Source**, select **GitHub Actions**

That's it — pushes to `master` will auto-deploy.

## File Structure

```
index.html                     — Complete self-contained website
.github/workflows/deploy.yml   — GitHub Pages deployment pipeline
README.md                      — This file
```
