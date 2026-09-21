# Reno Cricket Club Website

Static HTML website package designed for GitHub Pages, Vercel, Netlify, or any standard web host.

## Files
- `index.html` - complete website, CSS, and JavaScript
- `assets/rcc-logo.jpeg` - RCC logo supplied for this build
- `assets/committee/` - place committee portrait files here

## Committee portraits
The screenshots supplied show committee members, but screenshots are not clean source portrait files. The site therefore uses polished initials placeholders rather than cropping low-quality portraits out of screenshots.

To add portraits:
1. Create/add files inside `assets/committee/`, for example `rahul-saha.jpg`.
2. In `index.html`, search for `const committee=[`.
3. Change `img:""` to `img:"assets/committee/rahul-saha.jpg"` for the correct person.

## Live Match banner
Search `index.html` for:
`const LIVE_MATCH = false;`

Change it to:
`const LIVE_MATCH = true;`

Then change:
`const LIVE_URL = "https://www.youtube.com/@renocricketclub";`

to the exact YouTube livestream URL. The red LIVE banner will appear above the hero.

## Forms
The included Join RCC form uses `mailto:` so it works without a backend. For a production deployment, replace it with Formspree, Jotform, Google Forms, Wix Forms, or your own API endpoint.

## Main external links
- Official RCC: https://www.renocricketclub.org
- YouTube: https://www.youtube.com/@renocricketclub
- CricClubs: https://cricclubs.com/RenoCricketClub
- Facebook: https://www.facebook.com/RenoCricketClub/
- Instagram: https://www.instagram.com/reno_cricket_club/

## Editing
All layout, colors, text and functionality are in `index.html`. Search the CSS `:root` block to change the club colors globally.
