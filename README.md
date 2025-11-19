# Bentrell Promo Giveaway - App

**Giveaway:** Bentrell Promo Giveaway — ₦500,000 (1 winner)
**Entry period:** 21 Nov 2025 — 30 Jan 2026 (UTC)

## Quick local run (with Docker)
1. Copy `.env.example` -> `.env` and edit values.
2. Build and run:
   ```bash
   docker-compose up --build
   ```
3. Visit `http://localhost:3000` for public page.
4. Admin dashboard: `http://localhost:3000/admin.html` — browser will prompt for basic auth (ADMIN_USER/ADMIN_PASS).

## Local run without Docker
1. Install Node 18+, MongoDB running.
2. From project root:
   ```bash
   cd backend
   cp ../.env.example .env
   npm install
   npm run dev
   ```

## Opay integration
Implement `backend/utils/payout.js` to call Opay's payout/disbursement API and keep API keys server-side.

## Security & production checklist
- Replace Basic Auth with stronger auth.
- Use S3 or similar for screenshot storage in production.
- Use production MongoDB.
- Use HTTPS and secure the server.
