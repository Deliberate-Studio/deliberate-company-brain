# Company Brain by Deliberate

Your team's Claudes, one memory. Anything one person saves from their Claude, everyone's Claude can find: decisions, answers, how-tos.

## What it does

- **Searches first.** Ask Claude about your company, its customers, products, vendors, policies or past decisions, and it searches your team's Company Brain before answering. It tells you who saved what it found, and when.
- **Saves what you settle.** When a conversation settles a decision, an answer or a how-to, Claude saves it to the brain and tells you in one line. Claude can correct an item. To remove one, email hi@deliberatestudio.com.
- **Never saves** personal matters, small talk, drafts in progress, anything you call private or off the record, credentials, or customers' personal details.

## Before you start

You need a Company Brain from Deliberate: the Brain plan ($249/month, 14 days free, through the Shopify App Store), or the Agent Team, where your agents draw on what your team saves. https://deliberatestudio.com/company-brain. Each person connects once: type your workspace name (the first part of yourteam.deliberatestudio.com) and sign in with the email your team invited. Setup steps: https://deliberatestudio.com/company-brain/connect. Docs: https://deliberatestudio.com/claude

If your team already installed its own Company Brain plugin from its brain's page, use that one or this one, not both, or Claude will see the same tools twice.

## What this plugin runs, sends and fetches

This plugin has no code, scripts or hooks. It adds two skills (instructions for Claude) and one connector: Deliberate's connector at https://mcp.deliberatestudio.com/mcp, which each person signs in to themselves. People connected at the older address, https://deliberatestudio.com/api/brain/mcp, keep working. If you update this plugin, Claude asks you to sign in once more.

Deliberate receives the requests Claude makes through that connector (searches, reads of saved items and the research library, and what it saves or updates) so it can answer from your team's brain, and keeps a record of each request: the tool, when, and the network it came from. What Claude saves is kept until it's deleted. Deliberate can't read your Claude conversations, files or account. On some brains, searches are recorded too; see https://deliberatestudio.com/privacy#company-brain.

- Privacy: https://deliberatestudio.com/privacy
- Terms (Company Brain Annex): https://deliberatestudio.com/terms
- Support: hi@deliberatestudio.com
