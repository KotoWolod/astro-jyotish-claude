---
description: "Show the Astro Jyotish command menu and help links"
---

# /astro-help

Show this exact user-facing menu in English by default. If the user asks for Russian or Ukrainian help, translate every user-facing line, including headings, command descriptions, plain-language shortcuts, example questions, choice labels, and placeholder labels inside angle brackets such as `<birth date>` and `<your question>`. Preserve slash command identifiers, Markdown URLs, Astro Jyotish, Volodymyr Kraine, Parashara, Kraine, and literal language codes. English example sentences and English placeholder labels are forbidden in Russian or Ukrainian output. Do not add implementation details.

The literal text `/astro-help` is this plugin command. Never interpret it as a URL, website route, file path, or search query. Never inspect the current project or open a browser for this command.

This is a presentation-only command. Respond immediately with only the translated menu. Do not paraphrase, summarize, add recommendations, offer more help, call tools, inspect files, or send progress commentary.

```markdown
# Astro Jyotish

Astro Jyotish is by professional astrologer Volodymyr Kraine with 20+ years of experience.

## Commands

`/astro-help` - show this command menu
`/astro-login` - connect your Hidden World account
`/astro-status` - check your account, active chart images, stars, and subscription
`/astro-chart-images` - show active chart images: round D-1 Rasi, round D-9 Navamsha, South Indian D-1 Rasi, and South Indian D-9 Navamsha
`/astro-chart-setup` - learn how saved charts work
`/astro-create-chart` - create, save, and activate a natal chart
`/astro-charts` - list saved charts and show the active chart
`/astro-set-active-chart` - select the active saved chart
`/astro-contact` - send a confirmed message to Hidden World support ([Contact support](https://hidden-world.space/en/contacts))
`/astro-services` - view services, requirements, and current prices ([Services](https://hidden-world.space/en/services))
`/astro-natal` - choose language and Parashara/Kraine, then interpret your active natal chart ([How it works](https://hidden-world.space/en/articles/site_help_interpretation))
`/astro-forecast` - choose language and Parashara/Kraine, then create a forecast from your active natal chart ([How it works](https://hidden-world.space/en/articles/site_help_forecast))
`/astro-prashna` - choose language and Parashara/Kraine, then ask a concrete question using a question chart ([How it works](https://hidden-world.space/en/articles/site_help_prashna))
`/astro-panchanga` - choose language and Parashara/Kraine, then view Panchanga for a date and place ([How it works](https://hidden-world.space/en/articles/site_help_panchanga))
`/astro-question` - choose language, then ask the Kraine AI astrologer about your active chart
`/astro-referral` - view the inviter-email referral program and your status; submitting an inviter's email to claim a bonus requires your confirmation

## Plain-language shortcuts

You can also ask in plain English:

- Connect my Hidden World account.
- Show my Astro Jyotish status.
- Show my referral status and explain how to submit my inviter's email.
- Show my active chart images.
- Create and save a new chart for <birth date> at <birth time>, <city>, <country>, and name it <chart name>.
- List my saved Hidden World charts.
- Make the saved chart named "<chart name>" active.
- Contact Hidden World support about <subject>: <your message>.
- Make Kraine Panchanga in Russian for today.
- Make Parashara Panchanga in English for tomorrow in Pirovac, Croatia.
- Create a Kraine forecast in Russian for 2026-09-01.
- Interpret my active natal chart with Kraine in Russian, focus on house 10.
- Create a Kraine Prashna question chart in Russian for this situation: <your question>.
- Ask Kraine AI about my active natal chart in Russian: <your question about my chart>.

## Good Prashna questions

- Should I accept this offer?
- Can I reach an agreement with this partner?
- Is it worth launching this project this month?

## Choices

Languages: English, Russian, Ukrainian.
AI astrologers: Parashara, Kraine.

- Parashara: technical factors and their traditional Jyotish meanings for your own interpretation.
- Kraine: holistic relationships and synthesis by professional astrologer Volodymyr Kraine with 20+ years of experience.

## Referrals and balance

Hidden World uses the inviter's email, not a referral link. View your status with `/astro-referral`. Submitting a specified inviter's email to claim a bonus always requires your explicit confirmation. Eligibility, bonuses, and limits are determined by Hidden World; no bonus is promised in advance.

After an accepted service and its results, you receive the fresh available stars and subscription quota supplied by Hidden World. If the current balance is unavailable, the service is not repeated. The plugin does not sell credits, initiate checkout, or promote upgrades.
```

URLs must remain Markdown links and must not be placed in backticks or a code block in the actual response.

Before sending Russian or Ukrainian help, verify that every full example sentence and every placeholder label inside `<...>` is in the requested language. If any English text remains outside preserved identifiers and names, translate it before responding.
