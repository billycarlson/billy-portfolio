# Deploying to Vercel

## Option 1: Deploy via Vercel Dashboard (Easiest)

1. **Go to Vercel Dashboard**: https://vercel.com/dashboard
2. **Click "Add New" → "Project"**
3. **Import Git Repository** (if you want to track it):
   - Create a new repo for this static site
   - Push the `static-site` folder contents
   - Import it in Vercel
   
   OR
   
   **Deploy without Git**:
   - Click "Deploy" → "Browse"
   - Select the `static-site` folder
   - Vercel will deploy it

4. **Add your domain**:
   - Go to Project Settings → Domains
   - Add `wmcarlson.com` and `www.wmcarlson.com`
   - Update DNS records in Porkbun as Vercel instructs

## Option 2: Deploy via Vercel CLI

```bash
cd static-site
npm i -g vercel
vercel
```

Follow the prompts. When asked about the project, say it's a static site.

## Option 3: Replace Current Portfolio Project

If you want to replace your current portfolio project on wmcarlson.com:

1. In your current Vercel project settings
2. Go to Settings → General
3. Change the build command to: `echo "Static site"`
4. Change the output directory to: `static-site` (or wherever you put index.html)
5. Or just replace the entire project with the static-site folder

## File Structure for Vercel

```
static-site/
  ├── index.html      (your main page)
  ├── vercel.json    (routing config)
  └── package.json   (project config)
```

The `vercel.json` ensures all routes serve `index.html` (useful if you add more pages later).

## After Deployment

- Your site will be live at the Vercel URL (e.g., `your-project.vercel.app`)
- Add `wmcarlson.com` in Project Settings → Domains
- Update DNS in Porkbun to point to Vercel (they'll give you the records)

