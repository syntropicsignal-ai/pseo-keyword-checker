# pSEO Rewrite for Gemini CLI

Use this Gemini CLI extension to connect to a hosted MCP server for programmatic SEO. Give it an English product description and the exact keywords from your brief. It rewrites the description, checks every required phrase and returns the edited copy with the phrases it verified. You can also check a draft you have already edited.

## Install

```sh
gemini extensions install https://github.com/syntropicsignal-ai/pseo-keyword-checker
```

In a Gemini session, try:

> Rewrite this catalog draft and keep “clamp desk lamp” and “USB-C cable” exactly. Draft: This clamp desk lamp is supplied with a USB-C cable. The wall plug is sold separately.

Read the revised paragraph and check the product details before publishing. To review an existing edit, ask the checker which of your phrases are present or missing.

## Data and availability

`rewrite_seo_copy` sends the submitted draft and phrases to pSEO Rewrite and Anthropic to generate the edit. Submit public-facing copy you have permission to share. `preview_rewrite` runs a literal phrase check without model inference. Neither tool publishes to a shop or edits local files. The server counts usage in aggregate. All extension installations send the same client label.

The English pilot runs through December 21, 2026 (Warsaw). It has a shared usage allowance and requires no account.

[Setup and limits](https://rewrite.vectorlens.ai/mcp-setup/) · [Privacy and contact](https://rewrite.vectorlens.ai/privacy/)
