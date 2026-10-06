# Reasonance Labs

Showroom site for [reasonance-lab](https://github.com/reasonance-lab) — a single-page
portfolio linking out to projects across AI & learning, chemistry & science,
robotics & hardware, and developer tools.

**Live:** https://reasonance-lab.github.io/show/

*reasonance* /ˌriː.zəˈnɑːns/ — *n.* the amplification an idea gains when
reasoning is iterated until it rings true.

## Editing content

The homepage is the self-contained `index.html` from version 1 deployed at
[Reasonance on Sites](https://reasonance.jivishov.chatgpt.site). Its content,
styles, JavaScript, favicon, and SVG illustrations are inline.

The previous GitHub version is preserved in
[`codex/reasonance-backup-2026-10-06`](https://github.com/reasonance-lab/show/tree/codex/reasonance-backup-2026-10-06)
at commit `8301a2f31981a57b76f4331a413fb621d5593897`.

## Stack

HTML/CSS/vanilla JavaScript with no build step or external runtime dependencies.
The homepage includes project previews and category filters and respects
`prefers-reduced-motion`. The earlier design's asset files remain in the repository
but are not loaded by the new homepage.

## Local development

```
py -m http.server 8080
```

then open http://localhost:8080. No build, no watch — edit and refresh.

## Deployment

Pushed to `main` → GitHub Pages ("deploy from a branch", root) publishes
automatically. `.nojekyll` keeps Pages from running Jekyll. Changes can take
up to ~10 minutes to propagate through the Pages CDN.
