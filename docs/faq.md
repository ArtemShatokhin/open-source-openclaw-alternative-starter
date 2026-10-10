# FAQ

<!-- Part of an open source Kortix project template. -->

## Is Kortix open source?

Yes. Kortix is the open-source AI Operating System. You can read it, fork it and
audit it, and self-host the whole stack for free.

## What do I actually own when I self-host?

Everything the system needs: your agents, their skills, your company memory, the
connector configuration and the triggers — all files in one git repo. Sessions
run as isolated sandboxes with your repo and your tools already on them.

## Which models can I use?

Any. Kortix is model-agnostic: pick the model per agent, per session or per
message, bring your own API key from any major provider, or sign in with the
ChatGPT subscription you already pay for. You can also point it at your own
OpenAI-compatible endpoint.

## How is this different from a personal assistant like OpenClaw?

A personal assistant serves one person on one machine. Kortix is the layer a
company runs on: shared agents and skills, roles and groups, per-tool
permissions, an audit trail, and work that lands through a reviewed change
request. See [Kortix vs OpenClaw](kortix-vs-openclaw.md).

## Can an agent act without approval?

Only if you allow it. Every tool call can be set to allow, ask or block — down
to the arguments of the call. An *ask* holds the call until a person approves it,
then the agent resumes.

## How much does it cost?

Self-hosting is free. Managed Kortix Cloud is $40 per seat per month plus usage.
You bring your own model keys either way.
