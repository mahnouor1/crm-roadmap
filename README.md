# AI Outreach CRM — Roadmap Site

Static, single-page technical roadmap documenting the AI Outreach CRM build. Plain HTML/CSS, no build step, no framework, no dependencies.

## 1. Run locally

No install needed. Either:

```bash
open index.html
```

or serve it (needed if you want relative paths to behave exactly like production):

```bash
npx serve .
```

## 2. Build

There is no build step — `index.html` and `styles.css` are deployed as-is.

## 3. Deploy on Vercel

**Option A — Vercel dashboard**
1. Push this `roadmap-site/` folder to its own GitHub repository (recommended), or push the whole project and set the repo's **Root Directory** to `roadmap-site` in the Vercel project settings.
2. Import the repo in Vercel.
3. Framework Preset: **Other** (static site). Leave Build Command and Output Directory empty.
4. Deploy.

**Option B — Vercel CLI**
```bash
cd roadmap-site
npx vercel --prod
```
When prompted for framework, choose **Other**.

## Notes

- This site is documentation only. It contains no server IPs, credentials, or API keys, and no live metrics — those weren't included on purpose, since they'd go stale or require exposing internal state.
- Content reflects the actual project state as of the last update. Update `index.html` directly as phases change; there's no CMS.
