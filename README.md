# Astro Jyotish for Claude

Astro Jyotish connects a Hidden World account to Vedic astrology (Jyotish) services by professional astrologer Volodymyr Kraine with 20+ years of experience. It works in Claude Code, the Claude desktop app, and claude.ai.

## What it does

- Create, calculate, save, and activate natal charts from birth data, and switch the active chart.
- Show active chart images: round and South Indian D-1 Rasi and D-9 Navamsha.
- Run natal interpretation, transit forecasts, Prashna (question charts), and Panchanga.
- Ask the Kraine AI astrologer about the active saved chart.
- Show account status, stars, subscription requests, and inviter-email referral status.
- Send one confirmed support message to Hidden World.

Two service modes are available. Parashara presents technical factors and traditional meanings for self-interpretation. Kraine presents holistic relationships and synthesis by Volodymyr Kraine.

## Install

In Claude Code:

```
/plugin marketplace add KotoWolod/astro-jyotish-claude
/plugin install astro-jyotish@hidden-world
```

Then connect your account with `/astro-login`, or run `/mcp`, choose `astro-jyotish`, and select Authenticate. In the Claude desktop app or claude.ai, press Connect on the Astro Jyotish connector. Hidden World sign in opens in the browser.

## Commands

`/astro-help`, `/astro-login`, `/astro-status`, `/astro-services`, `/astro-chart-setup`, `/astro-create-chart`, `/astro-charts`, `/astro-chart-images`, `/astro-set-active-chart`, `/astro-contact`, `/astro-natal`, `/astro-forecast`, `/astro-prashna`, `/astro-panchanga`, `/astro-question`, `/astro-referral`.

You can also ask in natural language, for example "Show my active chart images", "Make Kraine Panchanga in Russian for today", or "Create a Kraine Prashna in English: Should I accept this offer?".

## What the plugin sends and where

The plugin contains no local code. It declares one remote MCP server, `https://mcp.hidden-world.space/mcp`, operated by Hidden World. Claude sends the requests you make with the plugin to that server: birth data for charts you create, questions for Prashna and Kraine AI, dates and places for forecasts and Panchanga, and support messages you confirm. Chart images are returned as short-lived links on Hidden World storage.

Access uses OAuth 2.0 with PKCE. Your Hidden World password never passes through Claude, and the connection can be revoked at any time.

## Stars and subscriptions

Paid services use stars or subscription requests that already exist in your Hidden World account. The plugin does not sell subscriptions, credits, or digital services and never starts a checkout. Before a service spends an existing entitlement, Claude shows the server-provided cost and asks you to confirm the exact request. When a subscription is active, it is used before stars.

## Links

- Website: [hidden-world.space](https://hidden-world.space/en)
- Privacy Policy: [hidden-world.space/en/policy](https://hidden-world.space/en/policy)
- Terms of Use: [hidden-world.space/en/terms](https://hidden-world.space/en/terms)
- Support: [Hidden World contacts](https://hidden-world.space/en/contacts)
