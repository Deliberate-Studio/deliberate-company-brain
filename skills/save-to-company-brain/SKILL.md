---
name: "save-to-company-brain"
description: "Save what a conversation settled to your team's Company Brain so everyone's Claude can find it. Use when a decision is made, a recurring question gets answered, a customer or vendor fact or a how-to comes up, a plan or meeting outcome is agreed, or something in the brain turns out to be wrong, and when the user says to remember, save or note something for the team."
---

# Save what the team will need again

Use the `deliberate-company-brain` tools for this team's Company Brain. If several team memories are connected, ask which business this is for.

When a conversation settles something a teammate will need again, save it with `save_context` and tell the user in one line. Use the line `save_context`'s reply gives you, word for word: it says how to remove the save. If the reply has no such line, say:

> Saved to the team brain: "{title}". If you'd rather not keep it, say "undo" to remove it.

If the user says undo or asks you to remove it, call `undo_save` with the id `save_context` returned.

How to write a save:

- **Title:** the headline fact with a date, for example "Holiday returns close Jan 15 (decided Oct 22)".
- **Body:** the conclusion in the first sentence, then the reasons and details a teammate who wasn't here would need.
- **Tags:** 3 to 6, in the team's own words.
- One item per topic. Batch related facts together, and keep it to a few saves per conversation.
- If the brain already has an item on this topic, update it with `update_context` (or save with `supersedes`) instead of saving a near-duplicate.

Never save:

- personal matters, small talk, or drafts still in progress
- anything the user called private or off the record, or asked you not to save
- coding or file work that holds no company or business fact
- passwords, API keys, tokens or other credentials
- customers' personal details (names with emails, phone numbers or addresses)

If the `deliberate-company-brain` tools aren't available, tell the user once: "Connect the Company Brain first: Customize › Connectors › Company Brain by Deliberate › Connect." In Claude Code, connect with `/mcp`.
