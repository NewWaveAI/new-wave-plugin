# NewWave for Claude

Use your NewWave brand workspace from Claude to plan campaigns, review creator work, and understand results.

## Included

- An OAuth connection to NewWave's hosted MCP server.
- The **use-newwave** skill, a short guide to finding your workspace and using NewWave's campaign tools.
- A marketplace catalog for installing the plugin from a downloaded copy of this repository.

## Requirements

A NewWave account with access to a brand workspace. The service uses your existing workspace permissions. NewWave account and plan requirements apply.

## Install in Claude Code

Download or clone this repository. In Claude Code, add its local folder and install NewWave:

```text
/plugin marketplace add /absolute/path/to/newwave-claude-plugin
/plugin install newwave@newwave-plugins
```

Restart Claude Code after installation, then open `/mcp`, choose NewWave, and complete the NewWave OAuth sign-in flow. Your NewWave role controls which workspaces and actions you can access.

For a temporary development session, run `claude --plugin-dir /absolute/path/to/newwave-claude-plugin` instead.

## Use NewWave

Ask Claude about NewWave or invoke `/newwave:use-newwave`. Name the workspace or campaign, the outcome you want, and whether you want a review or a change.

- "In NewWave, summarize our launch campaign for the past week, with links to the strongest videos. Read only."
- "Review applicants for our summer campaign and prepare recommendations for me to check."
- "Help me outline a creator brief for our new app. Keep it in this chat while we work on it."
- "Draft feedback on this campaign's pending submissions for me to review."

NewWave's [public prompt library](https://docs.new-wave.ai/ai-assistant/prompt-library) has more workflow examples.

## Connection and data

The MCP server URL is `https://api.new-wave.ai/mcp`, using Streamable HTTP. Sign-in takes place with NewWave. Credentials are managed by the MCP client; none are bundled with this plugin. The package contains text and JSON configuration and has no executable hooks or local server dependencies.

Connected assistants can act through your NewWave account. Review proposed creator-facing messages, approvals, destructive changes, and payment-related actions before authorizing them.

If the connection requires authentication, reopen `/mcp` and complete sign-in. For a missing workspace or denied action, check that the signed-in account has the expected workspace access.

## Links

- [NewWave](https://www.new-wave.ai)
- [Connection guide](https://docs.new-wave.ai/mcp)
- [Privacy policy](https://www.new-wave.ai/privacy)
- [Terms](https://www.new-wave.ai/terms)
- [Support](mailto:support@new-wave.ai)
