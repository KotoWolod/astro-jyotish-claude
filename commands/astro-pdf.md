---
description: "Order, track, and download a complete natal PDF interpretation"
argument-hint: "[language or order ID]"
---

# /astro-pdf

Use the connected Hidden World account and the active saved natal chart. The PDF is a separate Kraine interpretation with an overview, 12 life spheres, a forecast, and chart images. It is delivered to the verified account email and stored in the profile. It costs stars; a subscription does not pay for this product with request quota.

For a new order, ask the user to choose English (`en`), Russian (`ru`), or Ukrainian (`ua`) if not explicit. Read `astro_pdf_quote` before discussing a price. Show the active chart, exact current star price, delivery email requirement, and selected language and visual theme. Ask for explicit confirmation. Do not order if the quote is unavailable, the verified email is missing, or the user has not confirmed the exact cost.

After confirmation, call `astro_pdf_order` once with the quoted active chart ID, language, theme, exact star price, `confirmed: true`, and a stable `clientRequestId` of 16-100 ASCII letters, digits, hyphens, or underscores. Keep that request ID for this order. On a transport failure, check the same order before retrying; never create a new request ID for a repeat. Do not start a second paid order while the first one is pending.

The order is prepared asynchronously. Show its status and the current star balance returned by Hidden World. Use `astro_pdf_status` for the same order ID on follow-up. Do not poll indefinitely. When ready, use `astro_pdf_download` and present the short-lived URL as a clickable Markdown download link. `astro_pdf_orders` lists recent orders when the user asks or lost the order ID. `astro_pdf_email` sends a completed file again only after separate confirmation.

If Hidden World reports insufficient stars, explain the deficit using only supplied amounts. Do not treat this as a service outage, repeat the order, or start checkout. On any other failure, report that the PDF could not be ordered or retrieved without exposing implementation details.

Do not generate a PDF locally, reuse an ordinary natal reading as the document, expose private storage keys, inspect backend code, or modify the site and other services while handling this command.

[Full natal PDF on Hidden World](https://hidden-world.space/en/services?service=chart-report)
