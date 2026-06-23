# GovJobs Portal

A complete government job portal with:

- Public website (index.html) that loads jobs from a JSON API
- Admin panel (admin.html) to add/edit/delete jobs
- RSS feed (rss.xml)
- Auto‑expiry of old jobs
- Dark/light mode
- Auto‑refresh and real‑time sync between admin and public site via localStorage

## How to run

1. Place all files in the same folder.
2. Open `index.html` in a browser (for local testing).
3. Open `admin.html` to manage jobs – changes will instantly reflect in `index.html`.
4. To host publicly, upload the folder to any web server, Netlify, or GitHub Pages.

## Updating the live JSON API

- The `index.html` reads from `jobs.json` by default.
- For a production setup, replace `CONFIG.API_URL` in `index.html` with your hosted URL (e.g., `https://yourusername.github.io/govt-jobs-api/jobs.json`).
- The admin panel saves data to `localStorage`. You can export the JSON and replace the `jobs.json` file manually, or set up a GitHub Actions workflow to auto‑deploy.

## Features

- Search & filter by category
- Sort by latest, deadline, vacancies
- RSS subscription button
- Dark mode toggle
- Responsive design
