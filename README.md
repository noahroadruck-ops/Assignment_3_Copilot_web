# Simple Social Media Website

Simple Social Media Website is a small, desktop-first social media prototype built with plain HTML, CSS, and JavaScript. It includes a home feed, a separate profile page, sample posts, and lightweight client-side interactions. All content is local sample data; there is no account system, server, or database.

## Features

- Responsive home page with a fixed icon sidebar and a horizontally scrollable followed-people row.
- Sample post feed with portrait-style local CSS art, author details, timestamps, and icon controls.
- Like buttons that toggle state and update their counts.
- Comment forms that append comments locally without numbering them.
- A bottom-right Messages panel with sample conversations and open, close, and Escape-key controls.
- Separate profile page with profile details, statistics, profile actions, icon tabs, and 24 CSS-art gallery placeholders.

## Project Files

- `index.html` — Home page, post feed, messages panel, and client-side post interactions.
- `profile.html` — Profile details and the 24-tile post gallery.
- `README.md` — Project overview, setup, and usage instructions.

## Requirements

- A modern web browser.
- No packages, build tools, or external services are required.
- Python is optional if you prefer to run the site through a local web server.

## Installation and Setup

1. Download or clone the project, then open the project folder in VS Code.
2. No dependency installation is necessary. The site uses browser-native HTML, CSS, and JavaScript.
3. Open `index.html` in a web browser to use the site. The sidebar links open the Home and Profile pages.

To serve the folder locally instead, open a terminal in the project directory and run:

```powershell
py -m http.server 8000
```

Then visit `http://localhost:8000` in your browser. Stop the server with `Ctrl+C`.

## Usage

### Home

- Scroll the followed-people row horizontally to browse its sample profiles.
- Scroll the feed to view sample posts.
- Select the heart icon to like or unlike a post; its count updates immediately.
- Select the comment icon to open that post's comment form. Submit a comment to add it to the page.
- Select Messages at the bottom-right to view sample conversations. Close the panel with its close button.

### Profile

- Use the Profile icon in the sidebar to open `profile.html`.
- The page displays sample profile details, follower statistics, icon tabs, and 24 placeholder posts.
- Edit profile, View archive, and the gallery tabs are visual controls only; they are not connected to account data or alternate galleries.

## Replacing Placeholder Images

The sample post and profile gallery artwork is drawn with CSS, so the site works without image downloads. To use your own photos, place image files in an `images` folder beside `index.html`, then replace a placeholder element with an image using a relative path:

```html
<img class="post-photo" src="images/bookstore.jpg" alt="Bookshop window on a sunny day">
```

Provide useful `alt` text for each photo and style the image with `width: 100%`, `height: 100%`, and `object-fit: cover` to preserve the portrait layout.

## Scope and Data

Interactions run in the browser only. Likes and comments are not saved after reloading the page, messages are sample conversation previews, and the profile does not connect to a real account or service.