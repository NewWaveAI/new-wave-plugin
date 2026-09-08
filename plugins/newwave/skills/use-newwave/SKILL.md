---
name: use-newwave
description: Help users connect to NewWave and use their brand workspace for campaign planning, creator and submission reviews, content research, and performance reports. Use when the user asks to work with NewWave or a campaign in NewWave.
---

# Use NewWave

NewWave helps brands run user-generated content campaigns with creators. Use the connected NewWave MCP tools to work with the user's account.

## Get connected

This plugin connects to `https://api.new-wave.ai/mcp` over Streamable HTTP. Use the assistant's MCP connection controls to select NewWave and complete its OAuth sign-in flow. Users need a NewWave account with access to a brand workspace. Account setup is available at https://app.new-wave.ai/signup.

If the connection needs authentication, direct the user to the sign-in flow. If access is denied or no workspace is available, explain the returned result and help the user check their account and workspace access.

## Find the right context

Use the available NewWave tools to locate the workspace and campaign the user named. Ask which one they mean when the results are ambiguous. Read the tool descriptions for current capabilities and inputs; use returned identifiers for follow-up actions.

Keep the requested outcome clear: a review, a draft, or a change in NewWave. Preserve a request to review without changing anything.

## Common tasks

- **Campaign planning:** Gather the product, audience, objective, and relevant constraints. Help draft the brief and scripts. Save or configure the campaign when requested, using the available tools.
- **Creator and content review:** Inspect the selected campaign's applicants or submissions. Explain recommendations using the information available, and prepare feedback for review.
- **Content research:** Find relevant examples through NewWave's research tools and link the examples used to develop ideas.
- **Performance reporting:** Specify the campaign and date range. Use NewWave analytics for reported metrics, explain comparisons, and state when data is unavailable.
- **Creator communication:** Prepare the requested message in the context of the campaign. Show creator-facing actions and destructive changes for confirmation before executing them.

When making an authorized change, check the tool result and distinguish what was saved or sent from what remains a draft. Other services, such as email or shared documents, require their own connected tools and authorization.

## Public help

Use these guides for product setup and usage questions:

- Connection guide: https://docs.new-wave.ai/mcp
- Example workflows: https://docs.new-wave.ai/ai-assistant/prompt-library
- Product website: https://www.new-wave.ai
- Support: support@new-wave.ai
