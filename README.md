# MP3 Booster — BassForge

A responsive, browser-based audio enhancer for deeper bass and clearer vocals. Import a local audio file, preview the sound in real time, adjust the EQ, and export the processed audio.

## Features

- Upload MP3, WAV, AAC, M4A, and other browser-supported audio files
- Adjustable deep bass, vocal clarity, low-mid cleanup, and intensity
- Balanced, Deep Bass, Vocal Focus, and Club Punch presets
- Real-time visualizer and preview
- Export enhanced audio to WAV or MP3 (192 kbps)
- Files are processed locally in your browser; no server upload

## Run locally

Open `index.html` in a modern browser (Chrome, Edge, or Firefox). Select an audio file and start editing.

For a simple local development server (optional):

```bash
python -m http.server 8000
```

Then open http://localhost:8000.

## Publish with GitHub Pages

1. Create a GitHub repository named `mp3-booster`.
2. Upload `index.html` and this `README.md` to its root.
3. In your GitHub repository go to **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
5. Open the site URL shown by GitHub Pages when deployment completes.

## Notes

- Uses the Web Audio API for local processing.
- WAV encoding works without an external library; MP3 encoding loads `lamejs` from jsDelivr and needs a network connection.
- This is EQ-based enhancement, not AI source separation: vocals are not isolated from instrumentals, and missing frequencies cannot be restored.
- Large audio files may require substantial device memory during export.

## Technology

HTML, CSS, JavaScript, Web Audio API, and lamejs.