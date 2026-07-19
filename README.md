# Fincta

A full-stack finance dashboard for tracking financial data, visualizing it through interactive charts, and exporting reports as PDFs.

## Overview

Fincta is a React + Node.js application built around a personal/business finance dashboard. Users sign in via JWT or Google OAuth, view their data through interactive charts filtered by date range, and generate downloadable PDF reports — backed by a REST API and MongoDB.

## Features

- **Authentication** — JWT-based sessions with Google OAuth sign-in (Passport)
- **Dashboard & analytics** — interactive financial charts and visualizations (Recharts)
- **Date-range reporting** — filter and review data across custom date ranges
- **PDF export** — generate and download reports directly from the dashboard (jsPDF + html2canvas)
- **Email notifications** — automated emails via Nodemailer
- **REST API backend** — Express + MongoDB/Mongoose data layer

## Tech Stack

**Frontend** — React 17, Ant Design, React Router, Recharts, React Hook Form, Axios, styled-components
**Backend** — Node.js, Express, MongoDB, Mongoose, Passport (Google OAuth), JWT, bcrypt, Nodemailer

## Project Structure

```
Fincta/
├── fincta_backend/    # Express REST API, MongoDB models, auth, email
└── fincta_frontend/   # React (CRA) client — dashboard, charts, PDF export
```

## Getting Started

### Backend

```bash
cd fincta_backend
npm install
npm start
```

### Frontend

```bash
cd fincta_frontend
npm install
npm start
```

### Environment Variables

Create a `.env` file in `fincta_backend/` with:

```
MONGODB_URI=
JWT_SECRET=
GOOGLE_CLIENT_ID=
GOOGLE_CLIENT_SECRET=
SMTP_HOST=
SMTP_USER=
SMTP_PASS=
```

## License

MIT
