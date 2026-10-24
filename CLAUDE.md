# CLAUDE.md

Public learning lab: a simulated ECU (SOME/IP over UDP) in Python, C and C++, one pytest suite for all three, a CAN rest-bus and CI. Everything in this repo is in English.

## How work happens here

- **The owner writes the code.** Claude does not write code for this repo: it opens each ticket as an issue (context, what to build, acceptance criteria), explains the theory before each step, and reviews the pull request like a Staff SDET. The owner creates the branch, writes it, runs it, opens the PR and merges it.
- **Claude commits directly to `main` only repository upkeep** (this file, `.gitignore`, and prose it is asked to write), then pushes without asking.
- **Explicit paths in `git add`**, never `git add -A` or `git add .`.

## What never enters this repo

- Anything from the owner's private repos: notes, tracking, personal data.
- Wireshark captures of real interfaces (`wlo1`): they carry MAC addresses, IPs and DNS queries. Only loopback (`lo`) captures, under `captures/`.
