# Vercel Web Analytics Setup

This portfolio project has been configured with **Vercel Web Analytics** to track visitor analytics and page views.

## Implementation Details

### What's Enabled

✅ **Vercel Web Analytics** - Tracks page views and visitor data
✅ **Route Detection** - Automatically captures page changes
✅ **Privacy Compliant** - Follows data privacy standards

### How It's Implemented

For this HTML-based portfolio, Vercel Web Analytics is implemented by adding two scripts to the `<head>` section of `index.html`:

```html
<script>
  window.va = window.va || function () { (window.vaq = window.vaq || []).push(arguments); };
</script>
<script defer src="/_vercel/insights/script.js"></script>
```

These scripts:
1. Define the `window.va` function to queue analytics calls
2. Load the Vercel analytics tracking script from `/_vercel/insights/script.js`

### Prerequisites Completed

- ✅ Vercel CLI can be installed via npm/pnpm/yarn/bun (see `package.json`)
- ✅ Web Analytics integration scripts added to `index.html`
- ✅ Ready to enable Web Analytics in Vercel Dashboard

### Next Steps to Enable

1. **Connect to Vercel:** Push your repository to GitHub/GitLab/Bitbucket
2. **Create a Vercel Project:** Go to [vercel.com/new](https://vercel.com/new) and import your repository
3. **Enable Web Analytics:** In your Vercel project dashboard, click the **Analytics** tab and click **Enable**
4. **Deploy:** The analytics will start tracking automatically after your next deployment
5. **View Data:** Return to the Analytics dashboard to see visitor data and page views

### Useful Commands

```bash
# Install Vercel CLI
npm install -g vercel
# or
pnpm add -g vercel

# Deploy to Vercel
vercel deploy

# Local development server
npm run dev
```

### Monitoring Analytics

Once deployed and enabled in the Vercel dashboard:
- Navigate to your project's **Analytics** tab
- View real-time visitor data and page views
- After a few days of visitors, you can:
  - Filter and explore your data
  - (Pro/Enterprise) Add custom events to track button clicks, form submissions, etc.

### Learn More

- [Vercel Web Analytics Documentation](https://vercel.com/docs/analytics)
- [Privacy & Data Compliance](https://vercel.com/docs/analytics/privacy-policy)
- [Custom Events](https://vercel.com/docs/analytics/custom-events)
- [Filtering Data](https://vercel.com/docs/analytics/filtering)
