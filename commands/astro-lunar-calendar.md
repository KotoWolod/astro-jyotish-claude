---
description: "Show the free Hidden World lunar calendar data in chat"
---

# /astro-lunar-calendar

Use the Astro Jyotish lunar calendar capability for the current published month, a specified Kyiv date, or a published month. The calendar is free: no stars or subscription requests are consumed. It is a general calendar calculated for Kyiv, not a personalized chart reading.

Use the language explicitly requested by the user; otherwise use the current chat language. Dates and times use Europe/Kyiv. Obtain all calendar facts from the Hidden World lunar calendar capability; do not invent or recalculate them.

For a bare `/astro-lunar-calendar` or a general request to show the calendar, first get today's Kyiv date, then request that entire published month. Show the complete month in chat, not a one-day digest: all day rows in a compact table (date, phase, Moon sign, nakshatra, tithi, score, suitable activities), key lunar events with local dates and times, five favorable and five unfavorable dates, and the best dates for each available activity. Give today's row a separate detailed section with illumination, score components, sunrise/sunset, and every sign, nakshatra, and tithi change with its local date and time. Do not omit a section just to shorten the response.

When the user explicitly requests a month, show the same complete month sections and all day rows. When the user explicitly requests only today or a specific date, show the detailed day and its relevant changes without fetching the whole month unless they ask for it.

End with a short, localized "More in this calendar" help section. Tell the user they can request a specific date, any published month, favorable/unfavorable dates, or the best days for relationships, finance, purchases, documents, travel, study, health, and home. Include the returned source URL as a clickable link to the full website calendar and mention its annual overview, eclipses, methodology, and FAQ. Distinguish this free general Kyiv calendar from the personalized Rhythmeter, which uses the user's natal chart, dasha, and residence. Link to `https://hidden-world.space/{language}/services/ritometer` with the chosen language substituted; state that Rhythmeter is available on the website and has no plugin command yet. Do not replace the calendar data with a webpage link or HTML.

If the user's Hidden World account is not connected, use the documented connection flow. If the lunar calendar tool is not available in this plugin session, report that it is not yet available; do not invent values or calculate them locally.
