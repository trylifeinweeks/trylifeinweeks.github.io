# Life in Weeks – Hanhee Lee

This is an interactive map of my life, where each week I've been alive is a little box. The box's border color represents where I was living, the fill color what I was doing. Tap a box to see what I was doing where that week.

I made this to help myself see the bigger picture of the road I've walked.

Read more about [Life in Weeks at Wait But Why](https://waitbutwhy.com/2014/05/life-weeks.html).

This code was adapted from [Gina Trapani's Life in Weeks](https://github.com/ginatrapani/life-in-weeks) and [Buster Benson](https://busterbenson.com/life-in-weeks). It is a single webpage statically-rendered with [Hugo](https://gohugo.io/) and deployed to GitHub Pages. It consists of two [data](data/events.yml) [files](data/colors.yml), [an introduction](content/index.md), and a [template](layouts/_default/index.html).

## 🚀 Setup

1. Install Hugo:
   ```sh
   brew install hugo  # Mac
   ```
2. Clone and run locally:

```sh
    git clone https://github.com/trylifeinweeks/trylifeinweeks.github.io.git
    cd trylifeinweeks.github.io
    hugo server -D
```

3. Visit [http://localhost:1313/](http://localhost:1313/).

## ✨ Customize

- `content/` → Page content
- `layouts/` → Templates
- `assets/scss/` → Styles
- `assets/imgs/` → Site-wide images
- `static/` → Unprocessed assets
- `hugo.toml` → Site settings
- `data/events.yml` → Life events data
- `data/colors.yml` → Color scheme configuration

## 🚀 GitHub Pages Deployment

This site is automatically deployed to GitHub Pages using GitHub Actions. The workflow:

1. **Triggers**: On push to `main` branch or manual dispatch
2. **Builds**: Uses Hugo v0.147.2 with caching for performance
3. **Deploys**: Automatically to GitHub Pages

### Setup Instructions

1. **Enable GitHub Pages**:

   - Go to Repository Settings → Pages
   - Set Source to "GitHub Actions"

2. **The workflow file** `.github/workflows/hugo.yaml` is already configured with:

   - Hugo Extended version 0.147.2
   - Image caching with `:cacheDir`
   - Persistent Hugo modules
   - Automatic deployment to GitHub Pages

3. **Push changes**:
   ```sh
   git add -A
   git commit -m "Configure GitHub Pages deployment with Hugo + Hanhee's data"
   git push
   ```

The site will be available at: `https://trylifeinweeks.github.io/`

## 📊 Personal Data

- **Name**: Hanhee Lee
- **Birth Date**: December 4, 2004
- **Location**: Seoul, South Korea
- **Current Status**: University Student

## Colophon

This page uses [Bootstrap](https://getbootstrap.com/) for layout and interaction, and a smidge of [jQuery](https://jquery.com/) to reflect the current week on the map.

The font is [Red Hat Display](https://fonts.google.com/specimen/Red+Hat+Display). Colors chosen via [Color Hunt](https://colorhunt.co/).

## More Life in Weeks

There are several neat Life in Weeks examples and tools, including:

- [Weeksofyour.life](https://www.weeksofyour.life/): Make your own, completely browser-based
- [Life Calendar](https://lifecalendar.io): Make your own, with multiple layers
- [My Life in Days](https://days.sonnet.io/): Beautiful refactor, by days

🍯 "I always get to where I am going by walking away from where I have been." – Winnie the Pooh
