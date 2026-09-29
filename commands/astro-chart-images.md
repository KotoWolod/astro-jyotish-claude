---
description: "Show active chart images: round and South Indian D-1 and D-9"
---

# /astro-chart-images

Show the active Hidden World chart as images.

Use the authenticated chart image capability. Display the returned images directly when available:

- round D-1 Rasi chart
- round D-9 Navamsha chart
- South Indian D-1 Rasi chart
- South Indian D-9 Navamsha chart

Render the returned chart images in the final answer with Markdown image syntax, using the returned `markdown` value or the `chartImages[].url` values. Do not save image blocks to local files. Image URLs expire after a short time; if the user asks to see them again later, call the chart image capability again. Do not merely list image names.

Never claim that chart images were shown unless the final assistant message itself contains visible Markdown image tags. If image rendering is unavailable, say that the images were generated but could not be displayed here.

If the previous visible result was these four chart images and the user replies with `1`, `2`, `3`, or `4`, show only the selected image:

- `1`: round D-1 Rasi chart
- `2`: round D-9 Navamsha chart
- `3`: South Indian D-1 Rasi chart
- `4`: South Indian D-9 Navamsha chart

If the account is disconnected, say in the current chat language that the Hidden World account is not connected and the user should run `/astro-login`.

If no active chart is selected, ask the user to create or select an active chart with `/astro-create-chart` or `/astro-set-active-chart`.

Do not expose internal endpoints, environment state, tool names, authentication fields, raw payloads, or backend implementation details.
