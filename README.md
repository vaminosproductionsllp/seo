# Vaminos Blog Strategist AI

A responsive AI-powered SEO blog topic generator for Vaminos Productions LLP. It uses the OpenAI Responses API and optional built-in web search.

## Features
- Generate 10, 20, 30, or 50 topic ideas
- Configure market, goal, audience, and additional context
- Optional current web research
- Blog titles, suggested keywords, search intent, content angle, relevant service, funnel stage, and priority
- Top 5 recommendations, clusters, and publishing order
- Copy and download generated Markdown
- Server-side API key handling, workspace access code, and rate limiting

## Deploy using Render Blueprint
1. Import this repository into Render as a Blueprint or create a Node web service.
2. Build command: `npm install`
3. Start command: `npm start`
4. Configure `OPENAI_API_KEY` with an OpenAI Platform API key.
5. Set `APP_ACCESS_CODE` to a long private passphrase. This is required for generation in production.
6. Keep `OPENAI_MODEL=gpt-5.1` unless you prefer another model available to your API project.
7. Set `NODE_ENV=production`. The included `render.yaml` configures the Singapore region and free plan.

The health check is `/api/health`. It reports whether configuration is present, but never exposes secrets.

## Local development
Requires Node.js 20 or newer.

```sh
npm install
cp .env.example .env
npm start
```

Add real values to your local `.env`. Never commit API keys, access codes, or the `.env` file.

## Notes
- OpenAI API usage is billed separately from hosting and depends on the model and web-search use.
- Render free services may sleep when idle and may have resource limits.
- Suggested keywords and priorities are qualitative unless verified using a dedicated SEO keyword-data source.
