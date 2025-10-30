# Text-to-Animation AI Tool (API-based Starter)

This repository is a starter implementation for a Text → Animation pipeline:
- React frontend (Vite)
- Node/Express backend
- Worker (Bull + Redis) that orchestrates TTS (OpenAI), image generation (Replicate / Stable Diffusion), and composition (FFmpeg)

## Quick start (local, Docker)
1. Copy .env values (see server/.env.example) and set API keys.
2. Put royalty-free music into `server/media/music/mellow.mp3` and `server/media/music/upbeat.mp3`.
3. `docker compose up --build`
4. Open `http://localhost:3000` after building frontend into `frontend/dist` or run frontend dev separately.

## Notes
- Requires ffmpeg and ImageMagick for some helper commands if used.
- This is an MVP/starter. Harden for production before exposing publicly.
