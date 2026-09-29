---
description: "Send one confirmed support message to Hidden World"
argument-hint: "[request]"
---

# /astro-contact

Send one message to Hidden World support from the verified email of the connected Hidden World account.

Required user input:

- subject;
- message.

Optional input:

- preferred contact time;
- language for the support context: English, Russian, or Ukrainian.

If subject or message is missing, ask one concise question for all missing fields. Do not ask the user to paste account credentials, tokens, or a recipient address.

Before sending, show a short user-facing summary of the subject, message, and preferred time when present. Ask for explicit confirmation. Send exactly once only after confirmation.

After success, say in the current chat language that the message was sent and that a reply will go to the verified email of the connected Hidden World account. Do not print the email unless the user explicitly asks for it.

If the account email is not verified, say that a verified Hidden World email is required and link to [Hidden World profile](https://hidden-world.space/en/profile).

On failure, say only that the message could not be sent and link to [Hidden World contacts](https://hidden-world.space/en/contacts). Do not expose the recipient, endpoint, payload, raw error, or delivery provider.

Do not open the website when the in-chat send capability is available.
