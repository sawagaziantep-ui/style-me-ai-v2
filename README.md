# STYLE ME AI V2 — Vercel Zero Config

IMPORTANT: This version intentionally has NO vercel.json and NO build command.

Required structure:
- index.html
- api/generate.js

In Vercel Project Settings > Build and Deployment:
- Framework Preset: Other
- Build Command: leave empty
- Output Directory: leave empty
- Root Directory: ./

The /api folder at the project root is automatically deployed as a Vercel Function.

Environment variables:
- OPENAI_API_KEY
- REPLICATE_API_TOKEN

After deployment, test: /api/generate — it should return JSON with {"ok":true,...}.
