# AgentDesk Command Center

A multi-dashboard interface for AgentDesk with various views and analytics.

## Project Structure

```
├── index.html                 # Main landing page with navigation
├── src/
│   └── pages/
│       ├── dashboard.html     # Main dashboard view
│       ├── analytics.html     # Analytics dashboard
│       ├── agent-detail.html  # Agent detail view
│       ├── mobile.html        # Mobile-optimized view
│       ├── onboarding.html    # Onboarding flow
│       └── dashboard-refined.html # Enhanced dashboard
├── public/                    # Static assets (if needed)
├── package.json              # Node.js dependencies
├── vercel.json               # Vercel configuration
└── README.md                 # This file
```

## Available Pages

- **Main Dashboard** (`/dashboard`) - Primary mission control interface
- **Analytics** (`/analytics`) - Performance metrics and insights
- **Agent Detail** (`/agent-detail`) - Individual agent management
- **Mobile View** (`/mobile`) - Optimized mobile interface
- **Onboarding** (`/onboarding`) - New user setup experience
- **Refined Dashboard** (`/dashboard-refined`) - Enhanced dashboard experience

## Local Development

1. Install dependencies:
   ```bash
   npm install
   ```

2. Start the development server:
   ```bash
   npm run dev
   ```

3. Open `http://localhost:3000` in your browser.

## Deployment on Vercel

### Option 1: Connect Git Repository (Recommended)

1. Push your code to a Git repository (GitHub, GitLab, or Bitbucket)
2. Go to [Vercel Dashboard](https://vercel.com/dashboard)
3. Click "Add New..." → "Project"
4. Import your repository
5. Vercel will automatically detect the settings and deploy

### Option 2: Vercel CLI

1. Install Vercel CLI:
   ```bash
   npm i -g vercel
   ```

2. Login to Vercel:
   ```bash
   vercel login
   ```

3. Deploy from the project root:
   ```bash
   vercel
   ```

### Option 3: Drag and Drop

1. Zip the entire project folder
2. Go to [Vercel Dashboard](https://vercel.com/dashboard)
3. Drag and drop the zip file onto the deployment area

## Configuration

The `vercel.json` file handles:
- Static file serving
- Clean URLs
- Custom routing for each dashboard view
- Proper HTML content type handling

## Technologies Used

- **HTML5** - Semantic markup
- **Tailwind CSS** - Utility-first CSS framework (via CDN)
- **Google Fonts** - Typography (Inter & Material Symbols)
- **Vercel** - Hosting and deployment platform

## Features

- 📱 Responsive design
- 🌙 Dark mode support
- 🚀 Fast static hosting
- 🔄 Multiple dashboard views
- 📊 Analytics integration
- 🎨 Modern UI/UX design

## Environment Variables

No environment variables are required for this static site.

## Build Process

This is a static site with no build step required. All HTML files are served as-is with Tailwind CSS loaded from CDN.

## License

MIT License
