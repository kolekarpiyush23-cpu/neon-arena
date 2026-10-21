# Neon Arena — Real-time multiplayer browser game

A small, responsive arcade game where friends join the same room with a code, move around the arena, and compete to collect glowing orbs.

## Run locally
1. Install Node.js 18 or newer.
2. In this folder, run `npm install`.
3. Run `npm start`.
4. Open http://localhost:3000.
5. Enter a player name and a room code. Friends on the same computer/network can use the same room code.

## Make it accessible to friends online
Deploy this folder to a Node.js host that supports persistent WebSocket connections (for example Render, Railway, or another Node hosting provider). Use the included `package.json` start command. Once deployed, send friends the deployed URL and the same room code. The host's free-tier limits and sleep policies may vary.

## Gameplay
- WASD or arrow keys to move; on touch screens, drag/tap in the arena.
- All players in a room share the same target and scores.
- Click **Start 60-second round** to begin.
- The server checks collection distance and awards points.
- The **Copy invite link** button includes the room code in the URL.

## Project files
- `server.js` — Socket.IO multiplayer server and room state.
- `public/index.html` — game UI, canvas rendering, controls.
- `package.json` — dependencies and launch script.

## Before publishing
Test with at least two browsers/devices. Keep the server running on a WebSocket-capable host. This is a prototype suitable for a student project; it does not include accounts, persistent leaderboards, moderation, or production-grade anti-cheat.
