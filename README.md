# EmotionLogic Insurance Backend

This folder is ready to be deployed as a standalone Render web service.

## Files to push

- `server.cjs`
- `package.json`
- `package-lock.json`
- `.gitignore`
- `.env.example`

## Render setup

- Root directory: this `Backend` folder
- Build command: `npm install`
- Start command: `npm start`

## Environment variables

- `SMTP_USER`
- `SMTP_PASS`
- `SMTP_FROM`
- `SMTP_HOST`
- `SMTP_PORT`
- `SMTP_SECURE`
- `TRACKING_BASE_URL`

## Notes

- `TRACKING_BASE_URL` must be the public URL of this same backend.
- Do not commit `.env`, `sent_history.csv`, or `open_events.csv`.
- The service exposes:
  - `GET /`
  - `GET /sent-history`
  - `POST /send-bulk`
  - `GET /track/open/:trackingId`
