---
description: "List saved charts and show the active chart"
---

# /astro-charts

Show the connected Hidden World account's saved charts and identify the active chart used by personal services.

If disconnected, say in the current chat language that the Hidden World account is not connected and the user should run `/astro-login`.

If no saved charts exist, say in the current chat language that the user should create and save a chart first with `/astro-create-chart`.

Do not expose internal endpoints, raw payloads, authentication fields, or backend implementation details.

Do not inspect or modify backend code, Lambda configuration, AWS resources, environment variables, queues, prompts, or site/service code while handling this command.
