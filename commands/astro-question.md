---
description: "Ask the Kraine AI astrologer about the active saved chart"
argument-hint: "[request]"
---

# /astro-question

Follow the skill's payment confirmation and fresh balance contract: after every accepted service and same-request result, show returned stars and subscription quota with the localized balance message. Unavailable balance never authorizes a repeated paid call. For INSUFFICIENT_STARS, explain lack of stars (only supplied numeric amounts), not a service outage; do not retry or offer purchases. This specific error handling overrides generic failure wording below.

Ask the Kraine AI astrologer one question about the active saved Hidden World chart.

Requirements: connected account, active saved chart, a concrete question, explicit language, and subscription access. This service is Kraine-only.

Supported languages: English (`en`), Russian (`ru`), Ukrainian (`ua`).

Accept clear aliases such as `русский` -> Russian, `українською` -> Ukrainian, and `en` -> English.

AI astrologer: Kraine only, by professional astrologer Volodymyr Kraine with 20+ years of experience.

If language or question is missing, ask exactly one concise question in the current chat language containing every missing input.

Run the service once. If it returns a queued result, wait only for that same result. On failure, stop with a concise message in the current chat language. Say that the Kraine AI astrologer question could not be completed and no alternative service was used.

Never answer this as Prashna, forecast, Panchanga, or natal interpretation. Do not calculate locally, switch services, expose internal execution, or invent a result.

Do not inspect or modify backend code, Lambda configuration, AWS resources, environment variables, queues, prompts, or site/service code while handling this command.
