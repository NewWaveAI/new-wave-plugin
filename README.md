# NewWave for Claude

Connect Claude to your NewWave brand workspace to plan and operate user-generated content campaigns.

## What you can do

- Research content ideas and develop campaign briefs and scripts.
- Prepare campaigns and review creator applications and submissions.
- Analyze campaign results and creator performance.
- Prepare communication with your creators.

## Requirements

A NewWave account with access to a brand workspace. The service uses your existing workspace permissions. NewWave account and plan requirements apply.

## Try the plugin in Claude Code

Download this plugin directory, then run:

```sh
claude --plugin-dir /absolute/path/to/newwave-claude-plugin
```

Open `/mcp`, choose the NewWave server, and complete the NewWave OAuth sign-in flow. Authentication takes place with NewWave; the plugin does not contain passwords or API keys.

The bundled MCP connection uses Streamable HTTP at `https://api.new-wave.ai/mcp`. There are no local programs, hooks, or package dependencies to install.

## Example prompts

- "Show me the campaigns in my NewWave workspace and summarize their recent performance. Keep this read-only."
- "Compare applicants for my campaign, explain their strengths, and prepare a shortlist for me to review."
- "Help draft a campaign brief and filming script for my next product launch."

Ask Claude to show you proposed changes before approving creators, sending messages, deleting content, or taking payment-related actions. Use NewWave's analytics tools for reported metrics.

## Links

- [NewWave](https://www.new-wave.ai)
- [Connection guide](https://docs.new-wave.ai/mcp)
- [Privacy policy](https://www.new-wave.ai/privacy)
- [Terms](https://www.new-wave.ai/terms)
- [Support](mailto:support@new-wave.ai)
