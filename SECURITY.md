# Security Policy

## What this repository is

A list of links. It ships no code, hosts no packages and serves nothing to a running Comfy install. Nothing here executes on a reader's machine.

That shapes where a report should go.

## A vulnerability in a listed project

Report it to that project, not here. Use its own issue tracker, or GitHub's private vulnerability reporting if the project has it enabled. The maintainer is the only person who can fix it, and a public report here reaches that project's users before its author does.

Custom nodes are third-party code. Comfy Org does not control, test or vet the code, models or data of a project listed under **From the community**, and listing one is not a safety claim. The [note in the README](README.md#installing-third-party-projects) says so in full.

## A vulnerability in Comfy software itself

ComfyUI has its own [security policy](https://github.com/comfyanonymous/ComfyUI/blob/master/SECURITY.md), including a threat model and what does and does not count. Other Comfy Org projects take reports through private vulnerability reporting on their own repository.

## An entry that should not be on the list

If a listed project is malicious, misleading or harmful, or if an entry exposes private information or an unauthenticated destructive action, [report the entry](https://github.com/Comfy-Org/awesome-comfy/issues/new?template=report-an-entry.yml). Removal is what that form exists for, though nothing here commits anyone to a timeframe.

Bring evidence: the version or commit, the exact file and lines, and what the code does. A scanner result can support a case but does not settle one, because node packs legitimately read files, write to disk and reach the network, and scanners produce false positives. [CONTRIBUTING.md](CONTRIBUTING.md) sets out when an entry comes out and when it gets corrected instead.

Removing an entry does nothing to the project, which stays wherever its author put it and may still be installable elsewhere.

## A vulnerability in this repository

If something in this repository's own automation can be abused, report it privately through [GitHub's vulnerability reporting](https://github.com/Comfy-Org/awesome-comfy/security/advisories/new) rather than opening a public issue.
