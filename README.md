# Data Slayers website

One-page site for **https://dataslayers.com**, hosted free on GitHub Pages from the `main` branch of
this repository. No build step.

| File | What it is |
|---|---|
| `index.html` | The whole site |
| `favicon.svg` | Browser-tab icon (the Dragon Eye) |
| `CNAME` | Tells GitHub Pages the site's domain. Keep it. |
| `.nojekyll` | Makes GitHub serve the files as they are |

## Updating the site

Edit the files, then from this folder:

```
git add -A
git commit -m "Describe the change"
git push
```

The live site updates a minute or two after the push.

## Domain

dataslayers.com is registered at GoDaddy. Its DNS (GoDaddy > My Products > dataslayers.com > DNS) needs:

| Type | Name | Value |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | bennelli25.github.io |

Remove GoDaddy's parked `A` record and any forwarding. Leave `MX` and `TXT` records alone (they are for email).
Once GitHub shows the domain as working (repository Settings > Pages), tick **Enforce HTTPS**.

## Still to do

- [ ] The AceMotion card copies its one-sentence description, sport list and prices from AceMotion's `llms.txt` (Nov 2026). Keep them in step when AceMotion changes. Its stick figure is the softball swing at contact from AceMotion's `motion.js` demo, labeled as made-up data.
- [ ] ACES stats (1,426 trap teams, 27 states, 29,336 scores) are a snapshot of the ACES rankings data from 2026-11-12. Update them now and then.
- [ ] Check the credit line ("created by the Aitkin County Elite Sharpshooters") describes the ACES / Data Slayers relationship the way you want.
- [ ] Set up the `hello@dataslayers.com` mailbox (or email forwarding), or change the address in `index.html`.

## Logo

The Dragon Eye: a gold slit-pupil eye under a heavy red brow. It lives in `index.html` as the `#ds-mark` symbol
(colors come from the `--mark-*` tokens, so it adapts to dark mode). `favicon.svg` is the same eye in its light colors.
