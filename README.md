# NeuroAtlas

Laptop-first interactive 3-D brain explorer. The app combines real anatomical geometry with qualitative educational models for emotional states, networks, scenarios, learning and meditation concepts.

## Deploy

This is a static Netlify site. Upload the files in this folder to a GitHub repository, connect the repository in Netlify, and use `.` as the publish directory. There is no build command.

## Important anatomy asset note

The app loads the open Brain Project anatomical GLB at runtime:
https://github.com/itayinbarr/brainproject

The Brain Project describes its named 3-D anatomy as derived from Z-Anatomy / BodyParts3D and related open imaging atlases, with the 3-D assets under CC BY-SA 4.0. NeuroAtlas does not claim ownership of that anatomy asset. Keep the attribution notice in the About panel and this README when deploying.

The application code is the NeuroAtlas project. The anatomy asset remains subject to its own license and attribution requirements.

## V2 product behavior

- Real segmented 3-D anatomical mesh loaded once.
- Hover and click identification.
- Large brain-first workspace.
- Cortex opacity control for seeing deeper structures.
- Left/right/both hemisphere controls.
- Functional Connections mode with visible 3-D pathways.
- Emotional-state model using qualitative labels instead of fake 0–100 neural activity numbers.
- Stress balance: dominant / elevated / strained / adaptive / background.
- Scenario builder with explicit Apply to brain action.
- Brain networks with synchronized 3-D highlighting.
- Learn mode that drives the brain visualization.
- Meditation concepts and EEG-band education are reserved for the next content layer; the current architecture is designed so this can be added without reloading the anatomical scene.

## Development

Serve over HTTP rather than opening `index.html` with `file://`, because the browser loads ES modules and the anatomical GLB at runtime.

Example:

`python3 -m http.server 8787`

Then open `http://localhost:8787/`.

## Scientific/product boundary

The colored state labels are an educational qualitative model. They are not measurements of individual neural activity, fMRI values, EEG values, diagnoses, or clinical recommendations.
