# MX Starlight Handyman Services - Complete Deployment Package

## Project Overview
Professional landing page for MX Starlight Handyman Services in Worcester, MA featuring:
- 6 services including transportation services
- Contact: (281) 475-0292, mxstarlight1@gmail.com
- Calendly integration: calendly.com/mxstarlight1
- Mobile-responsive design with custom branding
- No pricing displayed (as requested)

## Technology Stack
- **Frontend**: React 18 + TypeScript + Vite
- **Backend**: Express.js + Node.js
- **Styling**: Tailwind CSS + shadcn/ui components
- **Deployment**: Full-stack application with static file serving

## Hosting Options

### 1. Vercel (Recommended - Free Tier)
```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel --prod
```

### 2. Netlify (Free Tier)
```bash
# Build for static deployment
npm run build

# Upload dist/public folder to Netlify
# Set build command: npm run build
# Set publish directory: dist/public
```

### 3. Railway (Free Tier)
```bash
# Connect GitHub repo to Railway
# Set build command: npm run build
# Set start command: npm start
```

### 4. Render (Free Tier)
```bash
# Connect GitHub repo to Render
# Set build command: npm run build
# Set start command: npm start
```

## Environment Setup
No environment variables required - all configuration is built-in.

## Build Commands
```json
{
  "build": "vite build && esbuild server/index.ts --platform=node --packages=external --bundle --format=esm --outdir=dist",
  "start": "NODE_ENV=production node dist/index.js"
}
```

## Port Configuration
App automatically uses:
- `process.env.PORT` (for hosting platforms)
- Falls back to `5000` for local development
- Binds to `0.0.0.0` for accessibility

## File Structure
```
├── client/           # React frontend
├── server/          # Express backend
├── shared/          # Shared schemas
├── attached_assets/ # Logo and images
├── dist/           # Built files (generated)
└── package.json    # Dependencies
```

## Key Files Included
- Complete source code
- Logo: attached_assets/BBA73064-0996-421A-808E-6900B12A163D_1755613209721.jpeg
- All dependencies in package.json (including fixed nanoid)
- Build configuration
- Production-ready server setup

## Quick Deploy Instructions
1. Download/clone all files
2. Run `npm install`
3. Run `npm run build`
4. Deploy to any hosting platform above
5. Your site will be live with custom domain support

## Custom Domain
All hosting platforms above support custom domain connection for professional branding.