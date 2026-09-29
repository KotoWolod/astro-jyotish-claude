---
description: "Show Panchanga for a date and place"
argument-hint: "[request]"
---

# /astro-panchanga

Follow the skill's payment confirmation and fresh balance contract: after every accepted service and same-request result, show returned stars and subscription quota with the localized balance message. Unavailable balance never authorizes a repeated paid call. For INSUFFICIENT_STARS, explain lack of stars (only supplied numeric amounts), not a service outage; do not retry or offer purchases. This specific error handling overrides generic failure wording below.

Run only the Hidden World Panchanga workflow.

Requirements: explicit language and explicit AI astrologer choice.

Supported languages: English (`en`), Russian (`ru`), Ukrainian (`ua`).

Accept clear aliases such as `русский` -> Russian, `українською` -> Ukrainian, `en` -> English, `Крейн` -> Kraine, and `Парашара` -> Parashara.

Supported AI astrologers:

- Parashara: traditional technical Panchanga.
- Kraine: Volodymyr Kraine's synthesis by professional astrologer Volodymyr Kraine with 20+ years of experience.

If language or AI astrologer is missing, ask exactly one concise question in the current chat language. It must include both choice groups when both are missing: English, Russian, or Ukrainian; Parashara or Kraine.

Default date: today. Default place: active chart place. Respect an explicitly supplied date or place.

If no place can be resolved, ask exactly one question in the current chat language: which city or location should be used for the Panchanga?

Run the service once and wait only for that result. On failure, stop with a concise message in the current chat language. Say that the Panchanga could not be completed and no alternative calculation was used.

Do not retry with guessed data, use natal planetary positions as the daily chart, calculate locally, install dependencies, switch astrology engines, expose internal execution, or invent a result.

Do not inspect or modify backend code, Lambda configuration, AWS resources, environment variables, queues, prompts, or site/service code while handling this command.

[Panchanga help](https://hidden-world.space/en/articles/site_help_panchanga)
[Panchanga and muhurta](https://hidden-world.space/en/articles/panchanga_muhurta)
