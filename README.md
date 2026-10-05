# Learn STEM with Silas — AI V3

This project contains the website and its Express AI backend.

## Deploy online

The simplest setup is to deploy this entire project to Vercel. Vercel can run the Express backend and serve the website from the same deployment.

1. Upload this project to GitHub.
2. Import the GitHub repository into Vercel.
3. In Vercel Project Settings → Environment Variables, add:
   - `OPENAI_API_KEY` = your OpenAI API key
   - `OPENAI_MODEL` = `gpt-6-luna`
4. Deploy.
5. Open the Vercel URL. The Solve, Hint, Teach Me and Practice buttons use the `/api/...` routes in `server.js`.

IMPORTANT: Never put `OPENAI_API_KEY` in `index.html`, browser JavaScript, or a public GitHub file.

The API uses OpenAI's Responses API through the official OpenAI Node package.
