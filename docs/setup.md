# Set up the starter

<!-- Part of an open source Kortix project template. -->

This is the shortest path from a clone to a running agent on Kortix, the
open-source AI Operating System.

## Prerequisites

- A machine with `git` (the agent itself runs in the cloud, so this can be a laptop).
- The Kortix CLI, installed with one command:

```bash
curl -fsSL https://kortix.com/install | bash
```

## 1. Clone and scaffold

```bash
git clone https://github.com/kortix-ai/suna   # reference project
kortix init                                   # create kortix.yaml + agents, skills, config
```

`kortix init` writes a `kortix.yaml` and the `agents/` and `skills/` folders.
Copy this starter's files in if you want the worked example agent and skill.

## 2. Pick a model

Kortix is model-agnostic. Choose the model per agent, per session or per
message, and bring your own API key from any major provider — or sign in with
the ChatGPT subscription you already pay for.

## 3. Ship it

```bash
kortix ship
```

This pushes your repo and brings the whole project live. Then start a session:

```bash
kortix sessions new --prompt "Summarize this week's work and open a change request"
kortix cr ls   # review what the agent proposes
```

## What to check on day one

- A session ran on its own isolated machine and left a branch named after the session.
- The work arrived as a change request you could read as a diff.
- Nothing the agent did reached `main` without your merge.
