---
name: connect-spritecook
description: Guide the user through connecting SpriteCook MCP with an API key and verify the setup.
---

# Connect SpriteCook

Use this command when the user installed the plugin but has not connected their SpriteCook account yet.

## Steps

1. Explain SpriteCook MCP requires API auth before generation works.
2. Offer two setup paths:
   - Guided setup (recommended):
     - Windows: `iwr -useb https://www.spritecook.ai/connect-mcp.ps1 | iex`
     - macOS/Linux: `curl -fsSL https://www.spritecook.ai/connect-mcp.sh | bash`
   - Manual setup docs: `https://www.spritecook.ai/api-docs`
3. After setup, ask user to reload Cursor window.
4. Verify connection by calling `get_credit_balance`.
5. If verification passes, suggest a first generation test prompt.

## If It Fails

- `401/403`: invalid or expired API key; re-create key in SpriteCook dashboard.
- MCP unavailable: ensure `mcp.json` is enabled in Cursor and reload.
- No tools visible: check plugin is enabled and the `spritecook` server is active.
- Script issues: use the manual setup in `https://www.spritecook.ai/api-docs`.
