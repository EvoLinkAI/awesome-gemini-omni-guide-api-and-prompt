# Maintaining this collection

`README.md` is the source for shared structure and current-model guide text. The ten `README_*.md` files translate visible prose while preserving original prompts, source URLs, media URLs, and stable anchors.

The current guide and the historical collection serve different purposes. Update current specifications from Google and the selected platform's current documentation. Preserve the original model attribution of historical cases, comparisons, and community videos.

## Case and gallery structure

- Legacy cases retain category-local numbering and stable compatibility anchors. Case headings use level three; do not renumber an existing case merely to insert new material.
- Published prompts use unlabeled fenced blocks and remain verbatim. Showcase-only items have no invented prompt block.
- Official 1.2 demos use the stable `omni12-demo-N` anchors. Each poster links to the exact original playable video. The [source index](source-index.md) records their origin.
- Retain the original Google videos and inherited GitHub attachments. The eight official posters are byte-identical repository copies so GitHub can serve them as images; their original URLs are recorded in the source index. Do not substitute unrelated illustrations.
- Keep creator attribution in the source-linked case or gallery context and preserve the original input/output relationship.

## Update checklist

1. Check the model version, source date, and task-specific limits against the current primary sources.
2. Review candidate material for duplicates, exact prompt boundaries, and the matching original media.
3. Update English first, then all existing translations. Keep visible labels localized and immutable source/prompt/media fields unchanged.
4. Verify every changed local path and fragment link, open every changed source/documentation link, and check every new poster/playback pair.
5. Inspect desktop and narrow GitHub rendering. Check table cells, image loading, video destinations, and code or text overflow.
6. Run `git diff --check`, inspect the complete diff, and submit the reviewed change as a pull request.

The Quick Start uses browser trial and current task documentation. Keep executable API requests, key setup, and service-reference details in the linked documentation.
