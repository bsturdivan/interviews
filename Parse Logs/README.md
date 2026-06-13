# Parse Logs

### Part 1 — Algorithm

We have lists of logs as newline-delimited text and we need to make them queryable. Here's a sample line:
`2026-06-13T14:22:01Z [ERROR] service=auth latency=412ms msg="token expired for user 5"`
Write a parser that turns each line into a structured record. `msg` is free text and can contain spaces and equals signs, and not every line is well-formed.

### Part 2 — Expand with AI

Build an API and interface to allow for a faceted search and filtering of each column
