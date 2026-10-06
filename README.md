# NeuroAtlas

Laptop-first interactive educational brain explorer.

## What is included

- Interactive 3-D-style brain visualization rendered locally with Canvas/Web APIs (no runtime CDN or npm dependency)
- Drag rotation, scroll zoom, clickable brain structures and labels
- Major regions including prefrontal cortex, amygdala, hippocampus, hypothalamus, thalamus, insula, ACC, nucleus accumbens, basal ganglia, brainstem, cerebellum, motor/somatosensory/visual cortex and corpus callosum
- Emotional states: neutral, fear, stress, anger, joy, sadness, love, focus and motivation
- State intensity control
- Qualitative brain-state activity visualization
- Brain-to-body explanations
- Scenario builder with sleep deprivation, exercise, meditation, caffeine, hunger, social rejection, novelty and chronic stress
- Network view: threat/salience, executive control, reward/motivation, memory/context and body-awareness systems
- Learning mode covering distributed processing, context, brain-body interaction, plasticity and scientific uncertainty
- Searchable anatomy inspector
- Evidence-language / scientific limitation guardrails
- Static Netlify deployment; no build step required

## Important scientific note

This is an educational visualization. The activity levels are qualitative and illustrative. They are not fMRI readings, direct neural recordings, medical advice, diagnostic output, or a claim that one brain region produces one emotion.

## Local preview

Because this is a static site, it can be opened directly as `index.html` in a modern browser. For the cleanest local preview, use any simple local HTTP server.

Example with Python:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Netlify

1. Create a new GitHub repository, e.g. `neuroatlas`.
2. Upload `index.html`, `styles.css`, `app.js`, `netlify.toml`, and this README.
3. In Netlify choose **Add new project → Import an existing project**.
4. Select GitHub and the `neuroatlas` repository.
5. Build command: leave blank.
6. Publish directory: `.`
7. Deploy.

Future pushes to the GitHub branch will trigger a new Netlify deployment.
