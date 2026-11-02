# Stakeholder map starter

A starting point for your own internal stakeholder map: who shapes the debate you work on, how they connect, and the source behind every link. It is the same tool as the Canada Tax Fairness Map, with invented sample data in place of the real people.

The step-by-step guide that comes with this explains everything in plain language. This page is the short version.

## What's in here

| File | What it is | Do you need to touch it? |
| --- | --- | --- |
| `index.html` | The website itself: layout, design and code. | No. |
| `data.json` | Everything on the map: people, organizations, the links between them, dates, and the map title. Starts with invented sample data. | No. You change it through **Admin** on your site. |
| `vercel.json`, `robots.txt` | Ask search engines not to list your site. | No. |

## Getting your own copy (short version)

1. On GitHub, press **Use this template** → **Create a new repository**. Pick your account, give it a name, choose **Private**, and create it.
2. On Vercel, sign up with your GitHub account, choose **Add New → Project**, import the repository you just made, and press **Deploy**. No settings to change.
3. Open your new site, press **Admin**, and follow the box: it asks for your repository name and a GitHub key that can only write to that one repository.
4. In Admin, open **Map settings** to set your title, then replace the sample people and organizations with your own. Press **Publish**. The site updates for everyone about a minute later.

## Keep it internal

- Keep the repository **Private**. The map will hold contact details and stance labels.
- Your Vercel address is not listed by search engines, but **anyone who has the link can open the site and its data**. Share the link only with your team.
- Only add contact details that the person has published themselves for work.
- Your GitHub key stays in your own browser. Never paste it anywhere else, and never put it in a file.

## data.json fields (for reference)

You don't need these to use the map; Admin fills them in for you.

- **settings**: `eyebrow` (small line above the title), `title`, `subtitle`, `counterpoint` (label for organizations that argue the other side), `leads` (things not yet verified), `parties` (name and colour for each party).
- **people**: `id`, `n` name, `g` sector, `r` role, `o` organization, `s` stance, `b` bio, `w` why they matter, `e` email, `li` LinkedIn URL, `lic` how sure you are the LinkedIn profile is theirs, `lin` what the profile shows, `p` profile page, `c` contact page, `x` social handle, `party`, `src` the page that shows their current role, `flag` check-before-contacting note, `home` part of your placement.
- **orgs**: `id`, `n` name, `short` short label, `k` kind (think tank, NGO, labour, parliament, government, party, media, university, or live file), `d` description, `u` website, `c` contact, `party`, `crit` argues the other side, `home` your placement.
- **edges**: `a` and `b` (the two ends), `t` type of link, `l` label, `u` source URL.
- **dates**: `date` (YYYY-MM-DD) and `text`. Past dates hide themselves.
