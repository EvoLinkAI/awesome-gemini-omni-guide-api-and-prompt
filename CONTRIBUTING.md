# Contributing

Contributions should help readers understand Gemini Omni or inspect a real, attributed example.

- Link to the original public source and identify the creator, publication date, and model version when available.
- Distinguish a reproducible prompt from a showcase. Copy published prompts exactly; omit the prompt block when the author has not shared one.
- Preserve the original input/output labels and source media. A video preview should link to its playable original video.
- Describe observed results without turning a single demonstration into a benchmark or general quality guarantee.
- Keep historical cases labeled by their actual version. Do not relabel older Omni results as 1.2 results.

Use `README.md` as the English source. Update all ten existing translations for changes to shared guide text or gallery content. Preserve prompt text, source URLs, media URLs, stable anchors, and legacy case identities across translations.

Before submitting a pull request, check the rendered desktop and narrow layouts, follow the changed links, verify the source/version and media pairing, and run `git diff --check`. See [the maintenance guide](docs/maintenance.md) for the content structure.
