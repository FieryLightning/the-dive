# The Dive

A hand-picked reading list for learning AI — Claude Code, Codex, running models on your own hardware, keeping it safe, and whatever turns up next — organised by depth instead of by category. Five zones, 40 entries:

| Zone | What's in it |
|---|---|
| 🐚 **The Tide Pool** | No experience needed. Free agents, visual explainers, browser courses. |
| 🌊 **Midwater** | Building: skills, MCP, cross-model review, SDKs, benchmarks. |
| 🔦 **The Trench** | Build it yourself: backprop by hand, an LLM from an empty file, one paper. |
| 🚢 **The Wreck** | Security and data safety. What sinks other people's ships. |
| 🤿 **Build Your Own Submarine** | Running and fine-tuning models on your own Mac mini, iPad or phone. |

One file, no build step, no dependencies, no tracking.

## Deploy to GitHub Pages

```bash
cd the-dive
git init
git add .
git commit -m "The Dive: an AI learning reading list"
git branch -M main
git remote add origin https://github.com/<your-username>/the-dive.git
git push -u origin main
```

Then on GitHub: **Settings → Pages → Source: Deploy from a branch → `main` / `root` → Save.**

It goes live at `https://<your-username>.github.io/the-dive/` in a minute or two.

To preview locally before pushing, just open `index.html` in a browser. There's nothing to compile.

### Files

| File | What it is |
|---|---|
| `index.html` | The entire site — HTML, CSS and JS inline |
| `.nojekyll` | Tells GitHub Pages to serve the file as-is instead of running Jekyll |
| `README.md` | This file |

## Editing it

Each entry is one `<a class="card">` block. Copy an existing one and change four things:

- `data-tags` — `video`, `security`, `local` drive the filter buttons. (`free`, `code`, `paper` are still on the cards but no longer have chips: nearly everything is free, so the chip hid nothing.)
- the emoji in `<span class="crit">` — the creature
- `<p class="what">` — what the thing is, one sentence, no adjectives
- `<p class="why">` — **why it's worth someone's time.** This is the part that matters. Say something you'd actually tell a friend, including the drawbacks. "Dry in places, worth it" is more useful than "comprehensive resource".

To move an entry between depths, cut the block and paste it into a different `<section class="zone">`.

The depth gauge on the right is calculated from scroll position, so it adjusts itself as you add or remove cards. Nothing to update.

## Credit and copyright

Every card links directly to whoever made the thing — Anthropic, OpenAI, Google, Apple, OWASP, Hugging Face, Kaggle, fast.ai, Andrej Karpathy, Sebastian Raschka, Grant Sanderson, and the open-source authors named on each link.

A personal learning list — things worth keeping, plus a few passed along by friends. Nothing was copied from anywhere: every description here is written from scratch and every link points at the original publisher.

## Link health

All 40 outbound links returned HTTP 200 when this was built. Link rot is inevitable; if one breaks, search the publisher's own site rather than trusting a mirror.
