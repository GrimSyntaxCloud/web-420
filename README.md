# WEB 420 RESTful APIs

Historical Node.js / Express / MongoDB coursework covering composers, people, customer purchases, user sessions and sports teams. The current entry point enables the team routes and Swagger documentation at `/api-docs`; other exercise routes remain in the source.

## Maintenance status

This repository stays available for possible recovery of its REST API examples. It is not the backend for the current portfolio demos. Its original dependencies and Node version are outdated and still have known advisories; modernize and test them before deployment.

## Database configuration

The application reads `MONGODB_URI` from the server environment and stops if it is missing. `.env.example` contains only a local, disposable database URL. The current historical startup script does not load `.env` automatically: set the environment variable through your development environment before using `npm start`. Never put a real database password in tracked source, a README, or a client-side bundle.

A hardcoded connection string was removed from the current source. Its credential must be revoked in the owning MongoDB Atlas account because previous commits still contain it. This source change does not revoke the credential or rewrite Git history. No connection to that database was attempted.

## Contributors

- Richard Krasso
- Andres Macias
