# Deliberate

Your brand's Deliberate workspace in Claude: ask the team questions answered from your live data, search what the team has filed, and save notes for the team.

## What it does

- **Asks the team.** Ask about sales, ads, orders, stock, support or customers, and Claude asks Deliberate's agents or pulls the numbers before answering from general knowledge.
- **Searches first.** Ask Claude about your company, its customers, products, vendors, policies or past decisions, and it searches what your team has filed before answering. It tells you who saved what it found, and when.
- **Saves what you settle.** When a conversation settles a decision, an answer or a how-to, Claude saves it as a note for the team and tells you in one line. Claude can correct an item. To remove one, email hi@deliberatestudio.com.
- **Never saves** personal matters, small talk, drafts in progress, anything you call private or off the record, credentials, or customers' personal details.

## Before you start

You need a Deliberate workspace, through the Shopify App Store:

- **Company Brain ($249/month):** the read-only tier, 14 days free. The Brain plan includes about $300 of usage. Ask the team, pull the numbers, save notes for the team.
- **Agent Team:** $500/month, and it includes $600 of usage. It adds drafts, sends and actions.

On both, usage above the included amount is billed through Shopify for exactly what you use.

 Each person connects once: type your workspace name (the first part of yourteam.deliberatestudio.com) and sign in with the email your team invited. Setup steps and docs: https://deliberatestudio.com/claude

If your team already installed its own plugin from its workspace's page, use that one or this one, not both, or Claude will see the same tools twice.

## What this plugin runs, sends and fetches

This plugin has no code, scripts or hooks. It adds three skills (instructions for Claude) and one connector: Deliberate's connector at https://mcp.deliberatestudio.com/mcp, which each person signs in to themselves. People connected at the older address, https://deliberatestudio.com/api/brain/mcp, keep working. If you update this plugin, Claude asks you to sign in once more.

Deliberate receives the requests Claude makes through that connector (questions to the team, the numbers it pulls, searches, reads of filed notes and research, and what it saves or updates) so it can answer from your workspace, and keeps a record of each request: the tool, when, and the network it came from. Questions and answers are kept only if your workspace turns on conversation logging. What Claude saves is kept until it's deleted. Deliberate can't read your Claude conversations, files or account. On some brains, searches are recorded too; see https://deliberatestudio.com/privacy#company-brain.

- Privacy: https://deliberatestudio.com/privacy
- Terms (Company Brain Annex): https://deliberatestudio.com/terms
- Support: hi@deliberatestudio.com
