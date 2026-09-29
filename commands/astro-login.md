---
description: "Connect your Hidden World account"
---

# /astro-login

Connect the operator's Hidden World account.

Claude (Claude Code, the Claude desktop app, or claude.ai) runs the Hidden World OAuth flow for the plugin's MCP server. If the Astro Jyotish tools are already available, call the status capability and report the result. Otherwise tell the user to connect Astro Jyotish in the host: in Claude Code run `/mcp`, choose `astro-jyotish`, and select Authenticate; in the Claude desktop app or claude.ai press Connect on the Astro Jyotish connector. Hidden World sign in then opens in the browser.

Do not replace this flow with a static website link or manual credentials.

Do not inspect or modify Hidden World backend code, Lambda configuration, AWS resources, environment variables, or OAuth server internals.

User-facing output must be in the current chat language and limited to these meanings:

- Opening Hidden World sign in.
- The Hidden World account is connected; run `/astro-status` to check it.
- The Hidden World connection could not be started; run `/astro-login` again.

Never expose authorization parameters, callbacks, tokens, tool names, commands executed, or implementation details.
