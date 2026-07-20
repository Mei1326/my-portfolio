# Your Portfolio — Setup Notes

This is your "cinematic-portfolio" template, customized with your resume data
and your photo.

## What's already done
- `data/profile.json` and `data/content.json` — filled in with your name, bio,
  skills, education, hackathon projects (Academic DocumentValidator, Smart
  Fitness Platform, Shielded Inbox, CivicVoice Station), certificates, and
  achievements from your resume.
- Your photo has been placed into the Hero, About, and Footer image slots
  (`public/assets/hero1.png`, `jyoti-about.png`, `jyoti-footer.jpeg`,
  `mobile-footer.webp`) — resized to fit each slot.
- Page title, meta description, social preview (OG) image, and manifest all
  updated to your name.
- GitHub + LinkedIn links wired up from your resume.

## What you should still do
1. **Intro video missing**: The original template had two short video clips
   of its original owner (`about_me.mp4` for the opening hero video, and
   `footer-video.mp4` for the footer section). I removed those since they
   weren't of you. Record a short 5–15s clip of yourself and save it as:
   - `public/assets/about_me.mp4`
   - `public/assets/footer-video.mp4`
   Until you add these, those two sections will show a dark/empty background
   instead of a video.
2. **Project images**: I reused the template's two sample project images
   (`project-artgenio1.png`, `project-easyfolio1.png`) across your 4 projects
   since I didn't have screenshots of your actual projects. Swap in real
   screenshots when you have them (same file names, or update the `image`
   path in `data/profile.json`).
3. **Project/GitHub links**: All project links currently point to your GitHub
   profile (github.com/Mei1326). Update each project's `link` in
   `data/profile.json` to the specific repo once you have one.
4. **Deploy URL**: `lib/siteConfig.js` has a placeholder
   `https://meiyalaghan-portfolio.vercel.app`. Update it once you deploy.

## How to run it locally
```bash
npm install
npm run dev
```
Then open http://localhost:3000

## How to deploy (free, easiest)
1. Push this folder to a new GitHub repo.
2. Go to https://vercel.com, sign in with GitHub, import the repo.
3. Click Deploy — it auto-detects Next.js. Done in ~2 minutes.
4. Copy the live URL into `lib/siteConfig.js` (`SITE_URL`) and redeploy.
