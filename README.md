# Hyvor Relay Test

Simple Node.js application for testing email sending through Hyvor Relay.

## Run

1. Install Node.js 18+ (20+ recommended).
2. Copy `.env.example` to `.env`.
3. Put your real Hyvor Relay API key in `.env`.
4. Run `npm install`.
5. Run `npm start`.
6. Open http://localhost:3000

## .env

HYVOR_RELAY_URL=https://mail.tontinehub.shopcoreone.com
HYVOR_RELAY_API_KEY=YOUR_REAL_API_KEY
HYVOR_RELAY_FROM=noreply@send.tontinehub.shopcoreone.com
PORT=3000

The Relay URL is `mail.tontinehub.shopcoreone.com`, while the current registered sending domain is `send.tontinehub.shopcoreone.com`.

Never expose the API key in frontend JavaScript.

If the API key has Allowed IPs enabled, the allowed IP must be the public IP of the machine running this Node.js backend.
