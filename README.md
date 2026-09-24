# FpS — 3D Multiplayer FPS

One server: **test**. Deathmatch arena, PC + mobile auto controls, chat, bots for solo fun.

## Run locally
```
npm install
npm start
```
Open http://localhost:3000

## Put on Render (website)
1. Push this folder to GitHub.
2. Go to https://dashboard.render.com → New → Web Service → select repo.
3. Render reads `render.yaml` automatically:
   - Build: `npm install`
   - Start: `npm start`
4. Open your `https://fps-game.onrender.com` link — everyone joins server **test**.

## Controls
- PC: WASD move, mouse look (click to lock), click shoot, R reload, Shift sprint, Space jump, Tab scores, Enter chat.
- Mobile (auto-detected): left stick move, drag right side look, 🔥 shoot, ▲ jump, ⟳ reload.

## Features
- Main menu + server browser (only "test")
- Procedural 3D soldiers with walk / shoot / death animations + nametags
- Detailed FP gun viewmodel: bob, recoil, muzzle flash + light, reload dip animation, tracers, impacts, blood
- Arena map with crates, towers, glow pillar, health packs
- Multiplayer via Socket.IO: positions, authoritative HP/kills, killfeed, scoreboard, chat
- 3 practice bots so it's fun even alone
