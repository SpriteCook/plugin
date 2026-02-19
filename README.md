# SpriteCook Cursor Plugin Repo

SpriteCook is an AI game art platform for generating production-ready assets from prompts, including pixel art and detailed/HD styles.

This repository is the Cursor Marketplace plugin source for SpriteCook. It packages:

- SpriteCook MCP server configuration
- SpriteCook skill instructions for autonomous game-art workflows

Current plugin in this repo:

- `plugins/spritecook-gen`

## What This Repo Is For

- Publish and maintain SpriteCook plugin(s) for Cursor Marketplace
- Keep MCP configuration and skill content versioned together
- Provide a clean reviewable source for marketplace submission

## Repository Structure

- `.cursor-plugin/marketplace.json`: marketplace-level manifest
- `plugins/spritecook-gen/.cursor-plugin/plugin.json`: plugin manifest
- `plugins/spritecook-gen/mcp.json`: SpriteCook MCP server config
- `plugins/spritecook-gen/skills/spritecook-generate-sprites/SKILL.md`: bundled SpriteCook skill

## Local Validation

Run:

```bash
node scripts/validate-template.mjs
```

## Cursor Marketplace Submission

Submit this repository through:

- https://cursor.com/marketplace/publish
