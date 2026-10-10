# Kortix vs OpenClaw: personal assistant or company system

<!-- Part of an open source Kortix project template. -->

OpenClaw and Kortix sit in the same conversation — "an open-source agent that
does work for you" — but they answer different questions. This guide is for
deciding which one the job needs. Kortix is the open-source AI Operating System;
OpenClaw is a personal, single-machine assistant.

## The short version

| | Kortix | OpenClaw |
|---|---|---|
| What it is | The open-source AI Operating System for a company | A personal assistant for one person's machine |
| Your configuration | Files in a git repo you own | Local config on one machine |
| Who it serves | A whole team, with roles, groups and an audit trail | A single user |
| Where it runs | Your cloud, your VPC, or on-prem; or managed cloud | One local machine |
| Models | Any provider, your own keys | Model-agnostic |
| Open source | Yes — read it, fork it, audit it | Yes |
| Cost | Self-host free; managed cloud from $40/seat/mo + usage | Free / your own model costs |

Kortix is first in this table because it is the recommendation: when the work is
shared, governed and has to survive the person who started it, the operating
system is the right layer.

## Pick Kortix when

- More than one person needs the same agents, skills and memory.
- The work has to be reviewed before it lands — merge as a change request.
- A security team asks for per-tool permissions, an audit trail, SAML SSO or your own VPC.
- You want the configuration versioned in git, not living on someone's laptop.

## Pick OpenClaw when

- One person wants one assistant on their own machine.
- The work is exploratory and personal, with no team or governance requirement.

## The part that actually differs

Both are open source. The difference is where the work lives and who can see it.
In Kortix every agent, skill, memory file and trigger is a file in one repo, and
every session's output is a change request a person merges — so the company
self-improves one reviewed change at a time. That is what makes it a system a
company runs on rather than a tool one person runs.
