# Deploying to Vercel 🚀

This portfolio is configured and optimized for instant deployment on [Vercel](https://vercel.com).

---

## Method 1: Deploy with GitHub (Recommended)

This is the easiest and best method because Vercel will automatically redeploy whenever you push changes to your repository.

1. **Push this folder to a GitHub repository**:
   - Go to [github.com/new](https://github.com/new) and create a repository (e.g. `portfolio`).
   - Push your code to the repository:
     ```bash
     git init
     git add .
     git commit -m "feat: complete portfolio with 3D card flips and vercel configuration"
     git branch -M main
     git remote add origin https://github.com/ANMOLRAWAT990/portfolio.git
     git push -u origin main
     ```

2. **Connect to Vercel**:
   - Go to [vercel.com](https://vercel.com) and log in with your GitHub account.
   - Click **"Add New..."** → **"Project"**.
   - Under **"Import Git Repository"**, choose your `portfolio` repository.
   - Framework Preset: **Other** (Static HTML).
   - Root Directory: `./` (leave default).
   - Click **"Deploy"**.

3. **Live in 30 Seconds**:
   - Your portfolio will be live at `https://your-portfolio-name.vercel.app` with instant global edge caching and free SSL!

---

## Method 2: Deploy with Vercel CLI

If you have Node.js installed, you can deploy directly from your terminal:

1. Open PowerShell or Command Prompt in this folder (`c:\Users\hp\Desktop\portfolio\portfolio`).
2. Run:
   ```bash
   npx vercel
   ```
3. Follow the quick terminal prompts:
   - Log in to your Vercel account.
   - Confirm project settings (hit Enter for defaults).
4. For production deployment:
   ```bash
   npx vercel --prod
   ```

---

## Custom Domain Setup

Once deployed on Vercel:
1. Go to your Project Dashboard on [vercel.com](https://vercel.com).
2. Go to **Settings** → **Domains**.
3. Type your custom domain (e.g. `anmolrawat.dev`).
4. Follow the DNS instructions (add the CNAME / A record in your DNS provider like Namecheap or Cloudflare).
5. Vercel will automatically provision a free SSL certificate.
