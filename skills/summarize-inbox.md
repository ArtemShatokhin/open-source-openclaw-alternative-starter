# Skill: summarize-inbox

<!-- Part of an open source Kortix project template. -->

A skill tells the company how a job is done. This one is a worked example: an
inbox digest that ends as a change request instead of a wall of text.

## When to use it

On a schedule (see the `weekday-digest` trigger in `kortix.yaml`) or when asked
for "the digest".

## Steps

1. Read the connected inbox for the last working day.
2. Group the messages into: decisions needed, work already done, and noise.
3. Write a short digest file at `reports/digest-<date>.md` in the repo.
4. Open a change request with that file and a one-line summary.

## Rules

- Never send or reply to mail from this skill — this skill only reads and writes files.
- Keep the digest under one screen; link to the source thread for anything longer.
- This skill is open source and part of a Kortix project; keep its steps in this file so the company can diff and improve them.
