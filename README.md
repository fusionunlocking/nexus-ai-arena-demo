# NEXUS AI Engineering Arena (Prototype)

A small, **simulated** dashboard for a hypothetical 50 ChatGPT agents vs. 50 Claude agents engineering challenge. Designed for a 16:9 YouTube/OBS browser source.

**This is not live telemetry.** No agents, repositories, CI services, or APIs are connected. All scores, events, activity dots, and node states are generated locally for demonstration.

## Run

Open `index.html` in a browser. Click **Start demo**, **Pause demo**, or **Reset**. No setup or dependencies needed.

For a local HTTP preview (optional):

```sh
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Publish free on GitHub Pages

1. Create a **new public repository**, e.g. `nexus-ai-arena-demo`.
2. Upload `index.html`, `README.md`, and `LICENSE` to its root.
3. In **Settings → Pages**, select **Deploy from a branch**, branch `main`, folder `/ (root)`.
4. Open the Pages URL GitHub provides, typically `https://YOUR_USERNAME.github.io/nexus-ai-arena-demo/`.

This prototype is intentionally separate from the private NEXUS V4.2 engineering repository. **Do not upload private code, logs, screenshots, API keys, tokens, or credentials.**

## OBS

Add a browser source pointed to the GitHub Pages URL or the local preview. Set source dimensions to 1920 × 1080. The demo is responsive and can run unattended, but it will not automatically restart when a simulation sequence ends.

## Future real-data integration (not included)

Replace the simulated event generator with a *read-only, sanitised* JSON or WebSocket feed containing verified event timestamps, team IDs, agent states, and acceptance evidence. Keep collection isolated from production. Never expose raw terminal output to the public stream.

## License

MIT. See `LICENSE`.