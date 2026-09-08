# NewWave for Claude and Codex

Use your NewWave brand workspace from Claude or Codex to plan campaigns, review creator work, and understand results.

## Included

- An OAuth connection to NewWave's hosted MCP server.
- The **use-newwave** skill, a short guide to finding your workspace and using NewWave's campaign tools.
- Marketplace catalogs for installing the same plugin in Claude Code and Codex.

## Requirements

A NewWave account with access to a brand workspace. The service uses your existing workspace permissions. NewWave account and plan requirements apply.

## Install in Claude Code

In Claude Code, add the NewWave marketplace and install the plugin:

```text
/plugin marketplace add NewWaveAI/new-wave-plugin
/plugin install newwave@newwave-plugins
```

Restart Claude Code after installation, then open `/mcp`, choose NewWave, and complete the NewWave OAuth sign-in flow. Your NewWave role controls which workspaces and actions you can access.

For a temporary development session, clone this repository and run `claude --plugin-dir /absolute/path/to/new-wave-plugin/plugins/newwave` instead.

## Install in Codex

Using the Codex CLI:

```sh
codex plugin marketplace add NewWaveAI/new-wave-plugin
codex plugin add newwave@newwave-plugins
```

Open a new Codex task after installation. Complete NewWave sign-in through the plugin's connection controls when prompted, then ask Codex to use NewWave.

For a local checkout, pass the repository folder to `codex plugin marketplace add` in place of the GitHub repository name. See [OpenAI's plugin packaging guide](https://developers.openai.com/plugins/build/plugins) for supported installation surfaces.

## Package layout

The shared plugin is in `plugins/newwave/`. Its Claude and Codex manifests use the same `.mcp.json` connection and `skills/use-newwave/SKILL.md` guide. Each host has a marketplace catalog at the repository root.

For a directory submission that asks for the path inside this repository, use `plugins/newwave`.

## Use NewWave

Ask your assistant to use NewWave. In Claude Code, you can also invoke `/newwave:use-newwave`. Name the workspace or campaign, the outcome you want, and whether you want a review or a change.

- "In NewWave, summarize our launch campaign for the past week, with links to the strongest videos. Read only."
- "Review applicants for our summer campaign and prepare recommendations for me to check."
- "Help me outline a creator brief for our new app. Keep it in this chat while we work on it."
- "Draft feedback on this campaign's pending submissions for me to review."

NewWave's [public prompt library](https://docs.new-wave.ai/ai-assistant/prompt-library) has more workflow examples.

## Connection and data

The MCP server URL is `https://api.new-wave.ai/mcp`, using Streamable HTTP. Sign-in takes place with NewWave. Credentials are managed by the MCP client; none are bundled with this plugin. The package contains text and JSON configuration and has no executable hooks or local server dependencies.

Connected assistants can act through your NewWave account. Review proposed creator-facing messages, approvals, destructive changes, and payment-related actions before authorizing them.

If the connection requires authentication, use `/mcp` in Claude Code or NewWave's connection controls in Codex to complete sign-in. For a missing workspace or denied action, check that the signed-in account has the expected workspace access.

## Links

- [NewWave](https://www.new-wave.ai)
- [Connection guide](https://docs.new-wave.ai/mcp)
- [Privacy policy](https://www.new-wave.ai/privacy)
- [Terms](https://www.new-wave.ai/terms)
- [Support](mailto:support@new-wave.ai)
