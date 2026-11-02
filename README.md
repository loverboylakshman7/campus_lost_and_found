# Campus Lost & Found

A responsive college Lost & Found web application demo.

## Features
- Browse sample lost and found listings
- Search by item name, description, or location
- Filter by item type and category
- Submit lost/found reports
- View reports created in the current browser
- Demo matching suggestions based on shared keywords and categories
- Claim request feedback
- Light/dark theme and responsive mobile navigation

## Run locally
No build tools are required.

1. Extract the ZIP.
2. Open `index.html` in a browser.

For a local development server, run:
```bash
python -m http.server 8000
```
Then visit `http://localhost:8000`.

## GitHub Pages
1. Create a GitHub repository.
2. Upload `index.html`, `styles.css`, `app.js`, `README.md`, and the `assets` folder.
3. Open repository **Settings → Pages**.
4. Select **Deploy from a branch**, choose `main` and `/ (root)`, then save.

## Important demo limitations
- Reports are stored in browser `localStorage`; they are not shared between devices.
- Sample listings are illustrative.
- Photo upload is shown in the form but files are not uploaded or persisted.
- Matching is a transparent keyword/category similarity demo, not a live Gemini AI model.
- Authentication, shared database, real notifications, and admin moderation require a backend such as Supabase.
- Never use this demo to publish private student information. Verify ownership before returning items.

## Suggested production upgrade
Connect Supabase Auth, PostgreSQL and Storage. Add server-side AI matching with credentials stored securely on the server, plus Row Level Security policies for user-owned reports and claims.
