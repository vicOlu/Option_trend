# Options Flow Analyzer - Vercel Deployment

## Quick Deploy

### Option 1: Vercel CLI (Recommended)

1. Install Vercel CLI:
   ```bash
   npm install -g vercel
   ```

2. Navigate to this folder and deploy:
   ```bash
   cd vercel-deploy
   vercel
   ```

3. Follow the prompts:
   - Log in to your Vercel account
   - Select your project scope
   - Deploy!

### Option 2: Vercel Dashboard (Drag & Drop)

1. Go to [vercel.com/new](https://vercel.com/new)
2. Click "Import" or drag the `vercel-deploy` folder
3. Click "Deploy"

### Option 3: GitHub Integration

1. Push this folder to a GitHub repository
2. Go to [vercel.com/new](https://vercel.com/new)
3. Import from GitHub
4. Vercel will auto-deploy on every push

## After Deployment

Your site will be live at:
- `https://your-project-name.vercel.app` - Public (read-only trends)
- `https://your-project-name.vercel.app/admin` - Admin (save to database)

**Share the main URL with colleagues. Keep /admin private for yourself.**

## Two Versions

| Page | URL | Features |
|------|-----|----------|
| **Public** | `/` | Upload CSV, view analysis, view trends (read-only) |
| **Admin** | `/admin` | All public features + Save to Database |

## Database (Supabase)

Already configured and connected:
- **Project URL**: https://bwqpikngknfmihgmaody.supabase.co
- **Tables**: flow_sessions, options_flow, daily_sentiment

Only you (via /admin) can write to the database. Colleagues can only read trends.

## Features

- Upload daily options flow CSV
- Full flow analysis (clustering, high conviction, etc.)
- View 7-day sentiment trends
- Track bullish/bearish streaks
- Detect sentiment flips
- Fetch live prices (Finnhub)
- **Admin only**: Save flows to shared database
