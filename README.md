# AI Meeting Notes Summarizer

This project summarizes meeting transcripts using Gemini AI securely.

## Features
- Upload or paste meeting transcripts
- Add custom instructions
- Secure backend proxy for Gemini API
- Share summaries via email or Gmail

## Setup
1. Install dependencies:
   ```powershell
   cd server
   npm install express node-fetch cors dotenv
   ```
2. Add your Gemini API key to `server/.env` (already set up).
3. Start the backend server:
   ```powershell
   node index.js
   ```
4. Update the frontend to use `/api/summarize` endpoint.

## Security
- The API key is stored in `.env` and never exposed to the frontend.
- `.env` is ignored by git.

## Deployment
- Upload all files except `.env` to GitHub.
- Never share your API key publicly.
