---
description: "Create, calculate, save, and activate a natal chart from birth data"
argument-hint: "[request]"
---

# /astro-create-chart

Follow the skill's payment confirmation and fresh balance contract: after every accepted service and same-request result, show returned stars and subscription quota with the localized balance message. Unavailable balance never authorizes a repeated paid call. For INSUFFICIENT_STARS, explain lack of stars (only supplied numeric amounts), not a service outage; do not retry or offer purchases. This specific error handling overrides generic failure wording below.

Create, calculate, save, and activate one Hidden World natal chart from birth data.

Requirements: connected Hidden World account and enough chart data: birth date, birth time, and birth place. If the birth time is unknown, the user must say that explicitly.

If any required birth data is missing, ask exactly one concise question containing every missing field.

Accept either natural-language birth data or structured wording. Examples:

- Create and save a chart for <birth date> at <birth time>, <city>, <country>, and name it <chart name>.
- Create a chart for <YYYY-MM-DD>, <HH:MM>, <city>, <country>, named <chart name>.
- Create a chart for <YYYY-MM-DD>, birth time unknown, <city>, <country>, named <chart name>.

After creating the chart, say that it was saved and is now active. Show the chart title if available and the visible birth date, time, and place if returned.

Do not expose internal endpoints, raw payloads, authentication fields, implementation details, or backend errors.
