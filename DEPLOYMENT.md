# Deployment

This site is deployed to Cloudflare Pages.

## Automatic Deploys (GitHub Actions)

This repo includes a GitHub Actions workflow that can deploy to the existing Cloudflare Pages project on every push to `main`.

### 1) Create a Cloudflare API token

In Cloudflare:

1. Go to **My Profile** -> **API Tokens** -> **Create Token**.
2. Create a **Custom token** with:
   - Permissions: **Account** -> **Cloudflare Pages** -> **Edit**
   - Resources: limit to your account (recommended)
3. Copy the token value.

### 2) Add GitHub repository secrets

In GitHub repo settings:

1. Go to **Settings** -> **Secrets and variables** -> **Actions**.
2. Add secrets:
   - `CLOUDFLARE_API_TOKEN`: the token you created above
   - `CLOUDFLARE_ACCOUNT_ID`: your Cloudflare account id (it appears in the dashboard URL as `dash.cloudflare.com/<account_id>/...`)

### 3) Deploy

Push to `main` and the workflow will deploy automatically.

