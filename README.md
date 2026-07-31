# Scholar Learn — Abacus & Mental Math Blog

A markdown-powered blog about abacus training, mental math, and online learning tools. Built for [Flowershow](https://flowershow.app/) — your site at `scholarlearn-testingwithdev.flowershow.me` updates automatically from the markdown files in this repo.

## Site Structure

| Path | Content |
|------|---------|
| `/` | Homepage with intro + recommended tools |
| `/blog` | Blog index with all articles |
| `/blog/what-is-abacus` | What is an Abacus? |
| `/blog/abacus-classes-near-me` | Abacus Classes Near Me |
| `/blog/how-to-learn-abacus` | How to Learn Abacus |
| `/blog/who-invented-abacus` | Who Invented the Abacus? |
| `/blog/abacus-meaning-in-hindi` | Abacus Meaning in Hindi |
| `/blog/sip-abacus` | SIP Abacus |
| `/blog/abacus-in-computer` | Abacus in Computer |
| `/blog/abacus-kit` | Abacus Kit |
| `/about` | About + recommended tools |
| `/resources` | Full resource list + tool table |
| `/contact` | Contact page |
| `/privacy` | Privacy policy |
| `/terms` | Terms of use |

## Check the Site Locally (localhost)

The site is plain markdown files. To preview it in your browser:

```powershell
cd "C:\Users\Admin\Downloads\scholar learn"
node preview.js
```

Then open **http://localhost:3000** — you will see the full site (home, blog, all 8 articles, resources, about, contact). The preview server renders the same content the live site will show.

## Update Your Live Site (scholarlearn-testingwithdev.flowershow.me)

Your Flowershow subdomain is fully hosted — it updates in one of two ways:

### Option 1: GitHub Sync (recommended)

1. Create a repo on GitHub and upload all files from this folder (keep the same folder structure)
2. Go to [cloud.flowershow.app](https://cloud.flowershow.app/) and sign in with your GitHub account
3. Click **New Site** → **Sync with GitHub** → select your repo and branch (`main`)
4. Give it the name **scholarlearn-testingwithdev** so your existing subdomain keeps working
5. Every future push to GitHub updates the live site automatically

### Option 2: `fl` CLI (instant updates)

Install the Flowershow CLI (already downloaded to `C:\Users\Admin\AppData\Local\Programs\fl\fl.exe` on this machine):

```powershell
fl login                      # one-time: opens browser to authorize
fl --name scholarlearn-testingwithdev .
```

Run the same `fl .` command after every change — it syncs only the changed files.

## Backlink Strategy

Every page on this site includes natural, contextual **dofollow backlinks** to `https://abacustool.xyz/`:

- **Homepage** — tool overview section with 9+ links to abacustool.xyz URLs
- **About page** — dedicated "Tools We Trust" section
- **Resources page** — full tool table linking every abacustool.xyz URL
- **Blog index** — "Free Practice Tools" list
- **Each blog post** — 3–6 contextual in-article links relevant to the topic
- **Contact/Privacy/Terms** — soft links to abacustool.xyz

### Target URLs Covered

| Target | Where linked |
|--------|--------------|
| https://abacustool.xyz/ | All pages |
| https://abacustool.xyz/abacus | Homepage, Resources, 6+ posts |
| https://abacustool.xyz/how-to-use | Homepage, Resources, 5 posts |
| https://abacustool.xyz/learn | Homepage, Resources, 4 posts |
| https://abacustool.xyz/about | — |
| https://abacustool.xyz/tools/flash-anzan | All pages |
| https://abacustool.xyz/tools/worksheet-generator | Resources, 6 posts |
| https://abacustool.xyz/tools/complement-drills | Resources, 5 posts |
| https://abacustool.xyz/tools/time-attack | Resources, 5 posts |
| https://abacustool.xyz/tools/step-solver | Resources, 3 posts |
| https://abacustool.xyz/tools/learning-path | All pages |
| https://abacustool.xyz/blog/* | Covered by matching blog topics |

> Note: Flowershow pages include only dofollow links by default (no `rel="nofollow"`), so all backlinks pass link equity.

## Adding New Posts

Create a new file in `content/blog/` with frontmatter:

```md
---
title: Your Title
description: Short description for SEO and cards
date: 2026-07-31
authors:
  - Scholar Learn
image: /images/your-image.png
---
```

## Local Preview

```powershell
cd "C:\Users\Admin\Downloads\scholar learn"
node preview.js
```

Open `http://localhost:3000`.

## Recommended Practice Site

All articles recommend [AbacusTool](https://abacustool.xyz/) — a free suite of abacus practice tools for flash anzan, worksheets, complement drills, time attack, step solving, and guided learning.
