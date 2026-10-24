---
name: "ask-the-team"
description: "Answer business questions from the brand's live Deliberate data instead of general knowledge. Use when the user asks about sales, revenue, ad spend or results, MER or CAC, P&L, subscriptions, orders, stock, support themes, customer feedback, the marketing calendar or releases, or asks what the team or an agent thinks."
---

# Ask the team

Use the `deliberate-company-brain` tools (the Deliberate connector). If several brands are connected, ask which one this is for.

When the user asks a question about the business, answer from Deliberate before general knowledge:

1. **A question that needs judgment or several sources** ("why did sales drop last week?", "what should we restock?"): call `ask` with the question in the user's words. The right agent answers from the brand's live data. If the reply says the answer is still coming, collect it with `get_answer`.
2. **A number or a list:** pull it directly:
   - revenue, spend, MER or CAC: `get_metrics`
   - ad results: `get_ad_performance`
   - P&L: `finance_snapshot`
   - subscription economics: `unit_economics`
   - order health: `get_order_health`
   - stock: `get_inventory`
   - support themes: `cx_themes`
   - customer feedback: `voice_of_customer`
   - research: `query_research`, `get_research`
   - the marketing calendar: `get_marketing_calendar`
   - releases: `get_releases`
3. Cite dates and numbers as the tools return them, and say when a recent window may be partial. If a tool says the brand doesn't have that integration, say so plainly and don't guess.

Drafts, sends and changes come with the Agent Team. If a tool says one of them isn't on this workspace's plan, tell the user in one line and keep helping with what you can read.
