# Self-host the starter

<!-- Part of an open source Kortix project template. -->

Kortix is open source and runs on your own infrastructure. You can self-host the
whole stack for free, run it in your own VPC, or use Kortix Cloud.

## Your own box

One Docker Compose stack brings the app up:

```bash
kortix self-host start
```

That starts the Kortix app and the services it needs on the machine you run it
on. From there, sessions run as isolated sandboxes with the same guarantees as
the managed cloud.

## What "self-hosted" gets you

- **Your data stays put.** Sessions, memory and connector config live in your repo and your infrastructure.
- **Your keys.** Model providers are called with credentials you hold, not ours.
- **Your network.** Run it inside a VPC or on-prem and reach internal tools only from inside.

## Postgres and secrets

The app expects a Postgres database and per-project secret storage. Secrets are
encrypted at rest with a key per project, and connector credentials are brokered
server-side so they never enter an agent's machine.

## When to use the cloud instead

Self-hosting is the right call when a security team needs the deployment inside
its own boundary. Kortix Cloud is the right call when you want the same system
without running the stack yourself — self-host free, or managed cloud at $40 per
seat per month plus usage. Both run the same open-source project.
