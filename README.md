# Between Us

**A softer corner of the internet for sharing what is on your mind and reminding others that they are not alone.**

🌐 **Live demo:** [between-us-public-site-1.vercel.app](https://between-us-public-site-1.vercel.app/)

## About

Between Us is a single-page web prototype for a gentle, anonymous-feeling community bulletin. Visitors can browse example notes, write a thought for the public board, or save a reflection in a private, browser-local vault. The design aims to feel calm, welcoming, and easy to use.

## Features

- **Community bulletin:** Displays 25 starter notes with topics and supportive responses.
- **Share or listen:** Switch between writing a note and reading or responding to notes.
- **Public board and private vault:** Choose whether a new note is added to the board or saved in the local private vault.
- **Topic suggestions:** Notes receive a topic label based on simple keyword matching.
- **Supportive replies:** Add a reply or use one of the suggested kind responses.
- **Browser persistence:** Notes and replies are saved with the browser's `localStorage`.
- **Accessibility support:** Includes a skip link, labeled controls, and screen-reader announcements for meaningful updates.
- **Responsive layout:** The page adapts to narrower screens.

## Tech stack

- HTML5
- CSS3, written in the page's `<style>` block
- Vanilla JavaScript, written in the page's `<script>` block
- Browser Web Storage API (`localStorage`)

There are no frameworks, package dependencies, build tools, or backend services in this prototype.

## Run locally

1. Download or clone this repository.
2. Open `index.html` in a modern web browser.

Alternatively, run a local static server from the project folder:

```bash
python -m http.server 8000
```

Then visit <http://localhost:8000>. No install or build step is required.

## How to use

1. Select **I want to share** to open the note composer.
2. Choose the **Public board** or **Private vault** option.
3. Write a note and save it.
4. Select **I want to listen** to browse the bulletin and leave a supportive response.

## Project structure

```text
.
├── index.html   # Complete website: markup, styles, and JavaScript
└── README.md    # Project overview and setup instructions
```

## Prototype limitations and privacy

This version is a front-end prototype. It has no server, user accounts, shared database, or moderation tools. The 25 starter notes are included in the page. New posts and replies are stored only in the browser that created them; they do not appear for other visitors. Private-vault notes are also stored in that browser's `localStorage`, not encrypted or protected by an account. Avoid saving sensitive information, especially on a shared device.

To make the public board genuinely shared and protect private notes across devices, the project would need a backend, database, authentication or another privacy design, and moderation controls.

## Deployment

The current prototype is deployed on Vercel at the live demo link above. It was uploaded as a static project. To have future GitHub commits deploy automatically, connect the GitHub repository to the Vercel project in its **Settings → Git** page.
