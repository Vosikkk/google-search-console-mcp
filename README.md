# Vosik Signals — Google Search Console MCP

Hosted, read-only Google Search Console integration for MCP-compatible AI assistants.

**Remote MCP endpoint:** `https://gsc.vosiksignals.win/mcp`

> This repository contains documentation and Registry metadata, **not the production server source code**. The server is hosted by Vosik Signals; no local installation is required.

Part of **[Vosik Signals](https://github.com/Vosikkk/vosik-signals)**, alongside the [Google Analytics 4 MCP](https://github.com/Vosikkk/google-analytics-mcp).

## What it does

Explore Search Console data using an AI assistant:

- Discover Search Console properties available to your Google account.
- Retrieve daily search performance and query/page breakdowns.
- Explore clicks, impressions, click-through rate, and average position.
- Inspect URL indexing status.

Google API results can be sampled, limited, delayed, or incomplete. Missing rows do not necessarily mean zero traffic.

## Connect

1. In an AI client supporting **remote Streamable HTTP MCP** and OAuth, add a custom MCP server.
2. Enter:

   ```text
   https://gsc.vosiksignals.win/mcp
   ```

3. Complete Google OAuth authorization with an account that can access your Search Console property.
4. Ask: “List the Google Search Console properties I can access.”

ChatGPT is the primary integration used during development. Compatibility with other MCP clients depends on their remote OAuth support and should be tested.

## Example prompts

- List my Search Console properties.
- Show clicks and impressions by day for the last 28 days.
- Which queries lead to a particular page?
- Inspect the indexing status of a URL.

## Privacy and security

The server uses Google OAuth with the read-only `https://www.googleapis.com/auth/webmasters.readonly` scope. The connector does not modify Search Console properties.

See the [Privacy Policy](https://vosiksignals.win/privacy) for details on data handling, credential protection, retention, and deletion.

Never share OAuth tokens, sensitive property data, or private reports in public GitHub issues.

## Support

Report bugs and client compatibility results via GitHub Issues, with sensitive information redacted.

- [Vosik Signals website](https://vosiksignals.win)
- [Main project documentation](https://github.com/Vosikkk/vosik-signals)
- [Security contact](mailto:vosikvos@gmail.com)

This documentation repository is not an open-source release of the hosted server implementation.
