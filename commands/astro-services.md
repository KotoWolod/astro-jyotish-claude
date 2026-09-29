---
description: "List Astro Jyotish services, requirements, and prices"
---

# /astro-services

Show the available services in the current chat language. Use authenticated account data for current costs and entitlements. Never infer balance, trial, or subscription state, and never offer checkout or an upgrade.

This is a presentation-only command. Respond immediately from this contract. Do not inspect files or send progress commentary. If live authenticated billing data is needed, make only the status/service call required for that data.

Do not inspect or modify backend code, Lambda configuration, AWS resources, environment variables, queues, prompts, or site/service code while handling this command.

For each service show its command, purpose, required user data, defaults, and price:

- `/astro-chart-setup`: explains how saved charts work.
- `/astro-create-chart`: connected account; creates, saves, and activates a natal chart from birth data.
- `/astro-charts`: connected account; shows saved charts and the active chart.
- `/astro-set-active-chart`: connected account and chart selection; sets the active saved chart.
- `/astro-natal`: active saved natal chart; choose language and Parashara/Kraine; optional Kraine focus house 1-12.
- `/astro-forecast`: active saved natal chart; choose language and Parashara/Kraine; forecast moment defaults to now; place defaults to the active chart place.
- `/astro-prashna`: concrete question; choose language and Parashara/Kraine; moment defaults to now; current place is required when it cannot be resolved.
- `/astro-panchanga`: choose language and Parashara/Kraine; date defaults to today; place defaults to the active chart place.
- `/astro-question`: active saved natal chart, explicit language, and subscription access; Kraine-only AI astrologer question.

Choice values:

- Languages: English (`en`), Russian (`ru`), Ukrainian (`ua`).
- AI astrologers: Parashara (`parashara`), Kraine (`kraine`).

Natural-language examples:

- "Connect my Hidden World account."
- "Show my Astro Jyotish status."
- "Create and save a new chart for <birth date> at <birth time>, <city>, <country>, and name it <chart name>."
- "List my saved Hidden World charts."
- "Make the saved chart named \"<chart name>\" active."
- "Make Kraine Panchanga in Russian for today."
- "Make Parashara Panchanga in English for tomorrow in Pirovac, Croatia."
- "Create a Kraine forecast in Russian for 2026-09-01."
- "Interpret my active natal chart with Kraine in Russian, focus on house 10."
- "Create a Kraine Prashna question chart in Russian for this situation: <question>."
- "Ask Kraine AI about my active natal chart in Russian: <question about my chart>."

Good Prashna question examples:

- "Should I accept this offer?"
- "Can I reach an agreement with this partner?"
- "Is it worth launching this project this month?"

Include these Markdown links:

- [Natal interpretation help](https://hidden-world.space/en/articles/site_help_interpretation)
- [Forecast help](https://hidden-world.space/en/articles/site_help_forecast)
- [Prashna help](https://hidden-world.space/en/articles/site_help_prashna)
- [Panchanga help](https://hidden-world.space/en/articles/site_help_panchanga)
- [Hidden World profile](https://hidden-world.space/en/profile)

Do not show backend operation names, raw service identifiers, payload requirements, or routing details.
