# Beauty by Earth

Full-stack website for a natural skincare brand: news, interviews, courses and influencer pages, search, user accounts and an admin dashboard.

## Features

- **Content** — news, interviews, courses, influencer and hashtag pages, plus search
- **Accounts** — register, login, confirmation, forgot and reset password, with Passport (local strategy) and sessions stored in MongoDB
- **Admin and user dashboards** — with Chart.js charts
- **Newsletter and email** — Mailchimp signups; transactional email with Nodemailer and Mailgun
- **Community** — Disqus comments and social sharing
- **Security** — Helmet, express-validator, mongo-sanitize and Google reCAPTCHA
- **SEO** — XML sitemap and RSS parsing

## Tech stack

Next.js · React · Express (custom server) · MongoDB with Mongoose · Passport · express-session · Chart.js · Mailchimp · Mailgun · Nodemailer

## Getting started

```bash
npm install
npm run devbackend   # Express + Next.js with auto-reload (nodemon)
```

Then open http://localhost:3000.

Create a `.env` file with your MongoDB connection string, session secret, and mail and Mailchimp credentials. Never commit it.

## Scripts

| Command | What it does |
| --- | --- |
| `npm run devbackend` | Run the server with nodemon |
| `npm run dev` | Run the server once |
| `npm run build` | Build the Next.js frontend |
| `npm start` | Run in production mode |

## Project structure

```
pages/        Next.js routes
components/ containers/ Layout/   UI
server/
  api/ controllers/ models/ middleware/ passport_config/ db/ helpers/
validation/   Form validation
lib/          Shared code
```
