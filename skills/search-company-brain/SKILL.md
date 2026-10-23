---
name: "search-company-brain"
description: "Search your team's Company Brain before answering a question about the company, its customers, products, vendors, policies, plans or past decisions, and before starting substantial work for the team. Use when the user asks what the team decided, how something is done here, or anything a teammate may already have answered."
---

# Search the Company Brain

The Company Brain holds what your team saved from their Claudes, plus the company's own site and store pages. Check it before answering from general knowledge.

Use the `deliberate-company-brain` tools for this team's Company Brain. If several team memories are connected, ask which business this is for.

1. Call `search_context` with a few specific keywords from the question.
2. If nothing matches, try once or twice more with other words: a synonym, the product name, the team's shorthand, a singular or plural form. Only then say the brain doesn't have it.
3. When a result's preview isn't enough to answer, read the top result in full with `get_context`.
4. When you use something a teammate saved, say who saved it and when, for example "Ana saved this on Oct 14."
5. If two items disagree, prefer the newer one and say so.

If the `deliberate-company-brain` tools aren't available, tell the user once: "Connect the Company Brain first: Customize › Connectors › Company Brain by Deliberate › Connect." In Claude Code, connect with `/mcp`.
