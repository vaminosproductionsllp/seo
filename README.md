# Vaminos Blog Strategist AI

A Vaminos Productions LLP web app that generates SEO-focused blog topic plans using the OpenAI Responses API.

## Features
- Generate 10, 20, 30, or 50 blog ideas
- Market, audience, goal and context controls
- Optional Responses API web search
- Recommendations, topical clusters and publishing order
- Server-side API key handling, access-code protection and rate limiting

## Deploy on Render
1. Create a Node web service from this repository.
2. Build command: `npm install`
3. Start command: `npm start`
4. Add environment variables `OPENAI_API_KEY`, `OPENAI_MODEL` (recommended default: `gpt-5.1`) and a strong `APP_ACCESS_CODE`.
5. Set `NODE_ENV=production`.

Do not commit API keys or access codes to GitHub. See `.env.example` for the local configuration template.
