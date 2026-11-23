# pSEO Rewrite for Gemini CLI

Use this Gemini CLI extension to connect to a hosted MCP server for programmatic SEO. Give it an English product description and the exact keywords from your brief. It rewrites the description, checks every required phrase and returns the edited copy with the phrases it verified. You can also check a draft you have already edited.

## Install

Start with an active Gemini CLI model session. Google retired consumer sign-in for Gemini CLI on June 18, 2026 and directs individual, Google AI Pro and Ultra users to Antigravity. [Check Gemini CLI account eligibility](https://developers.google.com/gemini-code-assist/docs/deprecations/code-assist-individuals).

[Register for pilot access](https://rewrite.vectorlens.ai/register/). Once your account has been approved, enter your pSEO Rewrite token when Gemini prompts for it during installation. Store the token in the extension setting.

```sh
gemini extensions install https://github.com/syntropicsignal-ai/pseo-keyword-checker
```

In a Gemini session, try:

> Rewrite this catalog draft and keep “clamp desk lamp” and “USB-C cable” exactly. Draft: This clamp desk lamp is supplied with a USB-C cable. The wall plug is sold separately.

Read the revised paragraph and check the product details before publishing. To review an existing edit, ask the checker which of your phrases are present or missing.

## Data and availability

`rewrite_seo_copy` sends the submitted draft and phrases to pSEO Rewrite and Anthropic to generate the edit. Submit public-facing copy you have permission to share. `preview_rewrite` runs a literal phrase check without model inference. Neither tool publishes to a shop or edits local files. The server counts usage in aggregate. All extension installations send the same client label.

The English pilot runs through December 21, 2026 (Warsaw). API and MCP calls require an active account token. The public website accepts individual sample requests. Approved accounts can rewrite one description at a time within their daily allowance.

[Setup and limits](https://rewrite.vectorlens.ai/mcp-setup/) · [Privacy and contact](https://rewrite.vectorlens.ai/privacy/)
