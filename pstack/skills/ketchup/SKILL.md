---
name: ketchup
description: "Catch the user up on everything since their last message, in plain words. Give each action item an executive summary with enough context to make the call. Use for /ketchup."
disable-model-invocation: true
---

# Ketchup

Catch the user up on everything since their last message. Write in the voice that [`/bro`](../bro/SKILL.md) describes. Assume the user remembers their last message and nothing after it. Call each PR, branch, or agent by a name they would know, not by a label you invented during the work.

## Gather what changed

Collect everything since that message: your own work, reports from subagents, and messages from anyone else. Check the current state of anything that can change on its own, such as a PR, a CI run, or a running agent. Say which items you could not check.

An action item is a decision only the user can make, such as a product choice, an approval, an irreversible step, or access you lack. Work you can do yourself is not an action item. Do it, or say that you will.

## Write the reply

Open with one sentence that says how many action items there are, or that there are none. If nothing happened, say so and stop.

Then say what happened, most important first. Give each result and what it means for the user. Skip steps that changed nothing.

Then give each action item a short executive summary. Cover the decision to make, why it matters now, the options and what each costs, your recommendation, and what happens if the user does not answer. Link to the detail, and write the summary so the user can decide without opening the link.
