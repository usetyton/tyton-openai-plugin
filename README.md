![Tyton](assets/icon.png)

# Tyton for ChatGPT and Codex

Tyton helps you get Meta Pixel and the Meta Conversions API (CAPI) working on your website.

- **Audit**: checks a public website's Meta tracking and tells you, in plain words, what works, what's missing and what it couldn't confirm. No sign-in needed.
- **Setup**: with a Tyton account, connects to one website, guides you through Meta one step at a time, helps you add your Conversions API token through a secure field, and installs only the conversions you approve.

## What's in the plugin

- `plugin.json`: the plugin manifest (Agent Plugins format).
- `mcp.json`: a connection to Tyton's server at `https://mcp.usetyton.com/mcp`, with Sign in with Tyton for setup tools.
- Three skills:
  - `meta-tracking-audit` runs the audit and explains the result.
  - `meta-tracking-setup` handles sign-in, setup progress, Meta guidance and approvals.
  - `conversions-api-token` keeps your Meta token out of the chat, your code and your reports.

The plugin has no scripts, hooks or local programs.

## Install

Once Tyton is listed in the plugin directory, install it from **Plugins** in ChatGPT or Codex.

To add only the server to Codex by hand:

```
codex mcp add tyton --url https://mcp.usetyton.com/mcp
codex mcp login tyton
```

Then ask something like "Audit the Meta tracking on my website" or "Set up Meta tracking for my site with Tyton".

## How sign-in works

The audit needs no sign-in. For setup, the app shows a Sign in with Tyton prompt. At usetyton.com you sign in, choose the one website the app may work on, and approve the connection. Connecting doesn't approve any tracking: you review the conversion plan and give a clear yes first. You can remove access any time on the **Integrations** page in Tyton.

## Links

- Docs: https://usetyton.com/docs
- ChatGPT guide: https://usetyton.com/docs/connect/chatgpt
- Codex guide: https://usetyton.com/docs/connect/codex
- Support: https://usetyton.com/contact (hello@usetyton.com)
- Privacy policy: https://usetyton.com/privacy
- Terms: https://usetyton.com/terms

## License

MIT. See [LICENSE](LICENSE).
