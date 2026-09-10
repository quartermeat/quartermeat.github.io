# GitHub Pages site

Follow `/home/quartermeat/AGENTS.md` for workspace conventions and commit versioning.

- Published repository: `quartermeat/quartermeat.github.io`.
- GitHub Pages publishes the root of `master`. Preserve the existing personal website.
- Mood Player homepage: `https://quartermeat.github.io/mood-player/`, served from `mood-player/index.html`.
- Mood Player belongs to `quartermeat/digital-terrarium`, not `card_game`.
- Use the Mood Player homepage as the Spotify developer app's website URL.
- Spotify OAuth redirect URI: `http://127.0.0.1:8091/api/spotify/callback`. Authorization is handled by the local Digital Terrarium app, not GitHub Pages.
- Keep the homepage static and free of credentials, external tracking, and build dependencies.
- Version source: `VERSION`. Each commit advances it and has a matching annotated tag.
- Preview: `python3 -m http.server 8080 --bind 127.0.0.1`, then open `/mood-player/`.
- Verify HTML structure, links, and mobile layout before publishing. After an authorized push, confirm the Pages build succeeds and the public URL returns HTTP 200.
