---
description: "Show account, active chart, stars, subscription, and chart images"
---

# /astro-status

Check the authenticated Hidden World account status.

Show only user-facing fields that are present: connection state, verified email state without printing the address unless explicitly requested, active chart label, stars, subscription or trial state, and Telegram connection state.

Always include active chart images in the same response when an active chart is present:

- round D-1 Rasi chart
- round D-9 Navamsha chart
- South Indian D-1 Rasi chart
- South Indian D-9 Navamsha chart

Render the returned chart images in the final answer with Markdown image syntax, using the returned `markdown` value or the `chartImages[].url` values. Do not save image blocks to local files. Image URLs expire after a short time; if the user asks to see them again later, call the chart image capability again. Do not merely list image names.

Never claim that chart images were shown unless the final assistant message itself contains visible Markdown image tags. If image rendering is unavailable, say that the images were generated but could not be displayed here.

If disconnected, say in the current chat language that the Hidden World account is not connected and the user should run `/astro-login`.

Do not expose internal endpoints, environment state, tool names, authentication fields, raw payloads, or backend implementation details.

Useful public destination: [Hidden World profile](https://hidden-world.space/en/profile).

Do not inspect or modify backend code, Lambda configuration, AWS resources, environment variables, queues, prompts, or site/service code while handling this command.
