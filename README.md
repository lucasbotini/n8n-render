# Render-Ready n8n

This is a minimal n8n environment ready to deploy on [Render.com](https://render.com).

## Deploy Steps

1. Fork this repo to your GitHub.
2. Go to Render → New → Web Service.
3. Connect GitHub, select this repo.
4. Use the following settings:

- **Build Command:** `npm install`
- **Start Command:** `npm run start`

## Required Environment Variables

| Key                       | Value                      |
|--------------------------|----------------------------|
| N8N_BASIC_AUTH_ACTIVE    | `true`                     |
| N8N_BASIC_AUTH_USER      | `admin`                    |
| N8N_BASIC_AUTH_PASSWORD  | `yourpassword`             |
| N8N_PORT                 | `10000`                    |
| PORT                     | `10000`                    |
| N8N_HOST                 | `0.0.0.0`                  |
| WEBHOOK_URL (optional)   | `https://<your-url>.onrender.com` |