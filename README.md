# Quartz v5

> “[One] who works with the door open gets all kinds of interruptions, but [they] also occasionally gets clues as to what the world is and what might be important.” — Richard Hamming

Quartz is a set of tools that helps you publish your [digital garden](https://jzhao.xyz/posts/networked-thought) and notes as a website for free.

🔗 Read the documentation and get started: https://quartz.jzhao.xyz/

[Join the Discord Community](https://discord.gg/cRFFHYye7t)

## Sponsors

<p align="center">
  <a href="https://github.com/sponsors/jackyzha0">
    <img src="https://cdn.jsdelivr.net/gh/jackyzha0/jackyzha0/sponsorkit/sponsors.svg" />
  </a>
</p>

---

```
# 1. Clone the Quartz repository
git clone https://github.com/jackyzha0/quartz.git
cd quartz
 
# 2. Install dependencies
npm i
 
# 3. Initialize your site (choose a template, set your base URL, import content)
npx quartz create
 
# 4. Install plugins referenced by your chosen template
npx quartz plugin install --from-config
 
# 5. Preview your site locally
npx quartz build --serve
```

## Publishing to GitHub Pages

This repo already has `baseUrl` in `quartz.config.yaml` set to `guillaumekuc.github.io/vilja-cnc-ecriture`, and a workflow at `.github/workflows/deploy-gh-pages.yaml` that builds the site and deploys it to GitHub Pages on every push to `v5`.

To publish:

1. Push the `v5` branch to `origin` (your own `guillaumekuc/vilja-cnc-ecriture` repo):
   ```
   git push origin v5
   ```
2. In the GitHub repo, go to **Settings → Pages → Build and deployment → Source** and select **GitHub Actions**. This only needs to be done once.
3. Check the **Actions** tab for the "Deploy Quartz site to GitHub Pages" run. Once it completes, the site is live at https://guillaumekuc.github.io/vilja-cnc-ecriture.

Any subsequent push to `v5` redeploys the site automatically.