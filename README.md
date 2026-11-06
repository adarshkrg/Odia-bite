# OdiaBite

A static food discovery and ordering demo for Odia cuisine.

## Run locally

Serve this folder over HTTP (required for browser password hashing), for example:

```bash
python -m http.server 8000
```

Open `http://localhost:8000/`. `index.html` is the Vercel entry point; `odiabite_taste_of_odisha.html` is the editable original page. The app loads `styles.css` and `app.js` from the same directory.

## Deploy to Vercel

Import this GitHub repository in Vercel and deploy it as a static site with the project root set to the repository root. No build command is required. Vercel serves `index.html` at the root URL.

## Demo account behavior

Customer and restaurant-owner accounts are stored in browser local storage. Passwords are salted and hashed with PBKDF2 in the browser. This is demo-only authentication: browser storage and client-side role checks are not secure for production. Production authentication requires a server API, persistent database, HTTPS, and server-validated sessions. One-click demo customer and admin logins are also provided.
