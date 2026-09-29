---
description: "Run a forecast from the active natal chart"
argument-hint: "[request]"
---

# /astro-forecast

Follow the skill's payment confirmation and fresh balance contract: after every accepted service and same-request result, show returned stars and subscription quota with the localized balance message. Unavailable balance never authorizes a repeated paid call. For INSUFFICIENT_STARS, explain lack of stars (only supplied numeric amounts), not a service outage; do not retry or offer purchases. This specific error handling overrides generic failure wording below.

Run only the Hidden World forecast workflow.

Requirements: connected account, active saved natal chart, explicit language, and explicit AI astrologer choice.

Supported languages: English (`en`), Russian (`ru`), Ukrainian (`ua`).

Accept clear aliases such as `русский` -> Russian, `українською` -> Ukrainian, `en` -> English, `Крейн` -> Kraine, and `Парашара` -> Parashara.

Supported AI astrologers:

- Parashara: traditional technical Jyotish forecast.
- Kraine: Volodymyr Kraine's synthesis by professional astrologer Volodymyr Kraine with 20+ years of experience.

If language or AI astrologer is missing, ask exactly one concise question in the current chat language. It must include both choice groups when both are missing: English, Russian, or Ukrainian; Parashara or Kraine.

Default forecast moment: now. Default place: active chart place. Respect an explicitly supplied date, time, or place.

If an active chart or place cannot be resolved, ask exactly one concise question containing every missing user input.

Run the service once and wait only for that result. On failure, stop with a concise message in the current chat language. Say that the forecast could not be completed and no alternative calculation was used.

Do not calculate transits locally, switch services, expose internal execution, or invent a result.

Do not inspect or modify backend code, Lambda configuration, AWS resources, environment variables, queues, prompts, or site/service code while handling this command.

[Forecast help](https://hidden-world.space/en/articles/site_help_forecast)
