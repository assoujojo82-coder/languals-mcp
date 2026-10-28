# Languals MCP server

Hosted MCP server of [Languals](https://languals.fr), a voice language tutor.

- Endpoint: `https://languals.fr/mcp` (streamable HTTP)
- Without an account: languages taught, CEFR level estimate, sentence correction explained in the learner's language, translation with usage notes.
- With a Languals account (OAuth 2.1 + PKCE, dynamic client registration): tutor conversation, session notes, progress, flashcard reviews, pronunciation.
- Discovery: `/.well-known/mcp.json`, `/.well-known/oauth-protected-resource`, `/.well-known/oauth-authorization-server`.

The tool list is served live by `tools/list`.

```json
{ "mcpServers": { "languals": { "url": "https://languals.fr/mcp" } } }
```

`grok-plugin/` is the Grok Build plugin.

Support: contact@languals.fr — Équipe Languals
