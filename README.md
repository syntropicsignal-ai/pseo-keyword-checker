# pSEO Keyword Checker for Gemini CLI

Check a product or category description against the exact phrases in your SEO brief. The hosted pSEO Rewrite preview echoes the submitted text unchanged and lists the phrases it found and missed. Pilot access runs through December 21, 2026 (Warsaw time).

## Try the checker

From your terminal, run:

```sh
gemini extensions install https://github.com/syntropicsignal-ai/pseo-keyword-checker
```

Open a new Gemini CLI session and enter `/mcp list` to check that `pseo-keyword-checker` is connected. The checker requires no separate account or API key.

Ask Gemini to use the tool with this example:

> Check the exact phrases “clamp desk lamp”, “USB-C cable” and “wall plug” in this draft using the pSEO Keyword Checker. Draft: This clamp desk lamp has a USB-C cable.

The expected result lists the first two phrases as present and “wall plug” as missing. Matching is case-sensitive. Try a public paragraph you have permission to share.

## What gets sent

The extension configures one remote tool, `preview_rewrite`. The tool sends the paragraph and optional phrases supplied in the call to `https://rewrite.vectorlens.ai/mcp`. Every installation sends the same client label. The preview counts successful calls by interface and keeps a subtotal for this extension. It does not save the submitted text or phrases. There are no local scripts or hooks in this extension.

For larger workflows, see the [MCP setup guide](https://rewrite.vectorlens.ai/mcp-setup/) and [REST quickstart](https://rewrite.vectorlens.ai/docs/). For a reviewed English rewrite, use the [sample editor](https://rewrite.vectorlens.ai/#sample). [Privacy and contact](https://rewrite.vectorlens.ai/privacy/)
