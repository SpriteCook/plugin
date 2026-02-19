# SpriteCook Plugin

This plugin connects Cursor to SpriteCook through MCP and bundles a skill that teaches your agent how to create game art.

SpriteCook can generate:

- game assets
- pixel art sprites and icons
- detailed/HD game art

The bundled skill helps the agent choose settings, generate assets consistently, and follow practical game-art workflows.

## Included

- MCP config: `mcp.json`
- Skill: `skills/spritecook-generate-sprites/SKILL.md`
- Command: `commands/connect-spritecook.md` (quick guided setup flow)

## API Key Setup

`mcp.json` contains a placeholder auth header by default. Use the connection script to write your real key into Cursor MCP config.

## Quick Start After Install

1. Connect your account (recommended):
   - Windows: `iwr -useb https://www.spritecook.ai/connect-mcp.ps1 | iex`
   - macOS/Linux: `curl -fsSL https://www.spritecook.ai/connect-mcp.sh | bash`
2. Or follow manual API setup: `https://www.spritecook.ai/api-docs` and set:
   - `Authorization: Bearer sc_live_...`
3. Reload Cursor window.
4. Ask: `Check my SpriteCook credit balance`.
5. Ask: `Generate a 32x32 pixel art chicken sprite with transparent background`.
