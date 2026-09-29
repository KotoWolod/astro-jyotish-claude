---
description: "Answer a concrete question from its Prashna question chart"
argument-hint: "[request]"
---

# /astro-prashna

Follow the skill's payment confirmation and fresh balance contract: after every accepted service and same-request result, show returned stars and subscription quota with the localized balance message. Unavailable balance never authorizes a repeated paid call. For INSUFFICIENT_STARS, explain lack of stars (only supplied numeric amounts), not a service outage; do not retry or offer purchases. This specific error handling overrides generic failure wording below.

Run only the Hidden World Prashna question-chart workflow.

Requirements: connected account, concrete question, explicit language, and explicit AI astrologer choice.

Supported languages: English (`en`), Russian (`ru`), Ukrainian (`ua`).

Accept clear aliases such as `русский` -> Russian, `українською` -> Ukrainian, `en` -> English, `Крейн` -> Kraine, and `Парашара` -> Parashara.

Supported AI astrologers:

- Parashara: traditional technical Prashna reading.
- Kraine: Volodymyr Kraine's synthesis by professional astrologer Volodymyr Kraine with 20+ years of experience.

Default question moment: now. Use the explicitly supplied current place; otherwise use the connected profile's current place when available.

If language, AI astrologer, question, or current place cannot be resolved, ask exactly one concise question in the current chat language containing every missing user input.

Run the service once and wait only for that result. On failure, stop with a concise message in the current chat language. Say that the Prashna reading could not be completed and no alternative calculation was used.

Never answer as a natal interpretation or generic forecast. Do not calculate locally, expose internal execution, or invent a result.

Do not inspect or modify backend code, Lambda configuration, AWS resources, environment variables, queues, prompts, or site/service code while handling this command.

[Prashna help](https://hidden-world.space/en/articles/site_help_prashna)
[What question astrology is](https://hidden-world.space/en/articles/question_astrology_prashna)
