---
description: "Run natal interpretation for the active saved chart"
argument-hint: "[request]"
---

# /astro-natal

Follow the skill's payment confirmation and fresh balance contract: after every accepted service and same-request result, show returned stars and subscription quota with the localized balance message. Unavailable balance never authorizes a repeated paid call. For INSUFFICIENT_STARS, explain lack of stars (only supplied numeric amounts), not a service outage; do not retry or offer purchases. This specific error handling overrides generic failure wording below.

Run only the Hidden World natal interpretation workflow.

Requirements: connected account, one active saved natal chart, explicit language, and explicit AI astrologer choice.

Supported languages: English (`en`), Russian (`ru`), Ukrainian (`ua`).

Accept clear aliases such as `русский` -> Russian, `українською` -> Ukrainian, `en` -> English, `Крейн` -> Kraine, and `Парашара` -> Parashara.

Supported AI astrologers:

- Parashara: traditional technical Jyotish reading.
- Kraine: Volodymyr Kraine's synthesis by professional astrologer Volodymyr Kraine with 20+ years of experience.

If language or AI astrologer is missing, ask exactly one concise question in the current chat language. It must include both choice groups when both are missing: English, Russian, or Ukrainian; Parashara or Kraine.

For Kraine, accept an optional focused house from 1 to 12.

If no active chart exists, ask exactly one question in the current chat language: which saved natal chart should be used?

Run the service once. If it returns a queued result, wait only for that same result. If it fails, stop with a concise message in the current chat language. Say that the natal interpretation could not be completed and no alternative calculation was used.

Do not calculate locally, switch services, expose internal execution, or invent a result.

Do not inspect or modify backend code, Lambda configuration, AWS resources, environment variables, queues, prompts, or site/service code while handling this command.

[Natal interpretation help](https://hidden-world.space/en/articles/site_help_interpretation)
