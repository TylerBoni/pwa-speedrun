# 8. Vercel Setup

## Connect Repository
- Add new project from GitHub
- Select repository
- Vercel auto-detects framework (Vite + React)

## Environment Variables
- Add any other required env vars from .env
- Copy and paste entire env file, update any that should be different for prod

## Domain Configuration
- Use Vercel-generated domain or add Cloudflare domain
- Configure DNS if using custom domain

## Build Settings
- Build command: `pnpm build` (or `npm run build`)
- Output directory: `dist`
- Install command: `pnpm install` (or `npm install`)

## Deployment
- Auto-deploys on push to prod branch
- Preview deployments for PRs
- Check deployment logs for errors
