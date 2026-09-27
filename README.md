# Shringaar Studio by Samapti

I built this responsive studio website as a React and TypeScript project. My goal was to make the studio's work the focus: real nail looks, a short reel, Instagram highlights, and clear ways for a visitor to get in touch. It is a working concept for studio review, not the studio's approved public website.

The site has four routes:

- **Discover (`/`)** - a photo-led introduction, recent work, a reel, highlights, studio information, and contact links.
- **The gallery (`/gallery`)** - a browsable set of looks with filters for all work, art, nails, and reels. The filtering happens in the browser.
- **Explore (`/explore`)** - links to the studio's Instagram highlights.
- **Our studio (`/studio`)** - a look inside the space, the visit details, and directions.

On smaller screens, gallery cards and highlights scroll horizontally. The WhatsApp and Call actions sit together so someone can choose how to ask about an appointment. The site links out to Instagram, phone, email, and the studio's Google Maps listing; it does not make a booking or collect customer details.

## Built with

React 19, TypeScript, Vite, and React Router. The page layout and responsive styles are in `src/style.css`; the components, content, routes, and link targets are in `src/App.tsx`. Studio imagery is stored locally in `src/photos/`, and the reel video served by the app is in `public/studio-nail-work.mp4`.

## Run it locally

Use Node.js 20.19+ or 22.12+.

```bash
npm ci
npm run dev
```

Vite prints the local URL. To check a production build:

```bash
npm run build
npm run preview
```

The build output goes to `dist/`. If you deploy it as a single-page app, configure the host to serve `index.html` for direct visits and refreshes on `/gallery`, `/explore`, and `/studio`. If you deploy under a subpath, set Vite's `base` and React Router's `basename` together.

## Project structure

```text
public/
  studio-nail-work.mp4     Reel video used by the app
src/
  App.tsx                  Components, routes, content, gallery filters, links
  main.tsx                 React entry point
  style.css                Layout and responsive styling
  photos/                  Studio images, reel poster, watercolor texture
  videos/                  Spare copy of the reel video; not used by the app
index.html                 HTML shell
package.json               Scripts and dependencies
vite.config.ts             Vite setup
tsconfig.json              TypeScript settings
```

The `.jpg`, `.webp`, and `.mp4` files are part of the project. A code-only text copy without them will not reproduce the complete site.

## Before this goes public

This is a portfolio and review build. The studio needs to approve the images, reel, founder details, branding, and copy before commercial use. Contact information, services, address, hours, and the Google rating should be checked with the studio and current listings before launch. Instagram posts and highlights may change or require sign-in. The rating shown here is a snapshot, not live data.

I used the studio's Instagram work as visual source material, the public profile of Samapti Sinha Mahapatra for the limited founder facts, and the studio's Google Maps listing for directions. The first-person studio copy is proposed website copy, not a quote or an approved statement from the studio. No secrets or API credentials belong in this repo.
