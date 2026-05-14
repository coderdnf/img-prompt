## Project Rules

- This project is a static prompt library for cross-border e-commerce image generation.
- Keep the deployable app in `index.html` unless the project grows enough to need separate assets.
- Store shared images and other static media in `assets/` with lowercase English filenames.
- Put reusable prompt templates directly in structured JavaScript data so they are easy to edit.
- Use Chinese UI text by default; keep image-style keywords in English when they improve generation quality.
- Keep TikTok Shop as the default platform unless F asks to change the business focus.
- TikTok Shop templates should emphasize mobile-first composition, UGC realism, scene hooks, pain points, and impulse purchase.
- Amazon / general e-commerce templates should emphasize product clarity, trust, dimensions, materials, and listing-style information.
- Do not store secrets, accounts, tokens, or private product data in this repository.
- Prefer simple static deployment so the page can be opened or hosted inside the office network.
- GitHub Pages publishes from `main` at `https://coderdnf.github.io/img-prompt/`.
- Do not run `git push` or publish changes unless F explicitly authorizes it in the current turn.
