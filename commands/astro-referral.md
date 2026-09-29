---
description: "Show referral status and explain the inviter-email program"
---

# /astro-referral

Use the authenticated referral status capability in the current chat language: English (`en`), Russian (`ru`), or Ukrainian (`ua`). Explain the existing Hidden World inviter-email system, not a referral link. Rules, eligibility, reward amounts, and limits come only from the server; never promise a bonus or hardcode numbers.

Status is read-only and never applies a referral. If the user wants to claim a bonus, ask for the inviter's email when missing. Never guess it or substitute the connected account email. Show the exact supplied email and ask for explicit confirmation to submit that email and claim the referral bonus. An email alone or a request to view status is not confirmation. A changed email requires new confirmation.

Only after confirmation, use `astro_referral_apply({inviterEmail, confirmed: true, language})` once. `/astro-referral` itself maps to `astro_referral_status({language})`. Do not expose these tool names in chat. Report success only when the server confirms it. Explain stable referral errors in the current chat language without raw codes or diagnostics; do not retry a claim or guess another email. After a transport error or uncertain claim outcome, read `astro_referral_status({language})` if available, never repeat the claim. A claimed status does not prove this attempt created the claim; if status is unavailable, report an unknown outcome rather than success.

Follow the skill's fresh account balance contract for returned stars and subscription quota. Do not infer missing values. Do not sell credits, initiate checkout, or promote an upgrade.

These capabilities may be unavailable before deployment and tool scanning. Use only tools actually available in this session. If missing, explain that referral actions are not currently available in this connection; do not invent calls, use generic RPC, inspect source, or simulate success. If disconnected, direct the user to `/astro-login`.
