# Launch checklist

What this repository needs before it is public. Pre-launch scaffolding: it comes out of the tree once the repository is public and the items below are settled.

Checked items are done in the tree. Unchecked items are either a repository setting nobody can commit, or a decision that needs a person.

## Repository settings

None of these can be done in a commit.

- [x] **Description.** Already set, and it reads well.
- [x] **Topics.** Set: `awesome`, `awesome-list`, `comfy`, `comfyui`, `custom-nodes`, `generative-ai`, `stable-diffusion`, `workflows`. The first two are what the awesome index requires and what its scrapers key on.
- [ ] **Social preview image.** Without one, every share renders as a grey GitHub placeholder. Needs a 1280x640 image from whoever owns the brand assets.
- [ ] **Issue templates.** Already in the tree. Confirm both forms render after the repository is public, because a malformed form fails silently and falls back to a blank issue.
- [x] **Labels.** `suggestion` and `report` now exist, so both forms apply what they declare. GitHub silently drops labels that do not exist.
- [x] **Discussions.** Already off, and worth leaving off. A list has two real interactions, propose and report, and both are already issues or pull requests. An empty Discussions tab reads as abandonment, and a busy one becomes a support channel for Comfy itself, which belongs in Discord. Turn it on later if people ask for something the two issue forms cannot carry.
- [ ] **Branch protection on `main`.** Require a pull request, require one approval, dismiss stale approvals, block force pushes. Allow maintainers to merge their own trivial fixes or triage becomes slower than it needs to be. Worth turning on at launch rather than before it, because it blocks the direct pushes the remaining prep still needs.
- [ ] **Private vulnerability reporting.** `SECURITY.md` links to the advisory form, which 404s until the setting is enabled. GitHub offers the setting on public repositories only, so this one cannot be done early: it has to be the first click after the repository goes public.
- [x] **Wiki and Projects.** Already off, confirmed. Nothing will live there.
- [x] **Allow only squash merges.** Done, and branches delete on merge. Keeps the history one commit per entry, which makes a bad entry trivial to revert.
- [ ] **CODE_OF_CONDUCT.md.** Not in the tree, deliberately. Contributor Covenant needs a working enforcement address in the text, and shipping one with a placeholder is worse than not having the file. The awesome index asks for a code of conduct, so this blocks index submission.

In the tree already:

- [x] `README.md` with the affiliation split and the trust note above the table of contents.
- [x] `CONTRIBUTING.md`, the inclusion bar, the removal criteria and the evidence standard.
- [x] `SUBMISSION_GUIDELINES.md`, the two-minute path to a correct pull request.
- [x] `SECURITY.md`, routing reports to the right place.
- [x] `.github/PULL_REQUEST_TEMPLATE.md`.
- [x] `.github/ISSUE_TEMPLATE/suggest-an-entry.yml` and `report-an-entry.yml`, plus `config.yml`.
- [x] `LICENSE`, CC0-1.0.

## The report and takedown path

- [x] A report route that does not require knowing how to open a pull request: the report form.
- [x] Published removal criteria, so a removal is not a judgement call made in private.
- [x] An evidence standard, so a scanner screenshot does not take down a legitimate pack. This matters here more than it would elsewhere: a large share of flagged packs are deliberate maintainer choices rather than real findings, and a list that removes on scanner output alone will remove the wrong things.
- [x] A statement that removal from the list does nothing to the project, so nobody mistakes delisting for a fix.
- [ ] **Decide whether a named contact is needed in addition to the issue form.** See the open legal questions below.
- [ ] **Decide who can merge a removal unilaterally.** A malicious entry should come out in minutes, not after a review cycle. Branch protection and that need are in tension, so name the people who can bypass it.

## Triage

This is the largest unresolved item. A list with no named triager becomes a stale list with open pull requests, which is worse than no list.

- [ ] **Name a primary triager and a backup.** Unassigned.
- [ ] **Confirm the response time.** `SUBMISSION_GUIDELINES.md` currently promises a first reply within a week. That number is in the tree and a submitter will hold us to it. Either someone accepts it or it needs changing before launch.
- [ ] **Subscribe the triagers to the repository**, and route the `report` label somewhere a human sees it the same day. An unwatched report form is a liability, not a takedown process.
- [ ] **Decide the review depth.** The honest position, and the one the README now takes, is that an entry is checked for fit and link health, not audited. Do not let that quietly become a security review in people's heads, because the disclaimer stops being true the moment we start implying we audit.

## When a listed project turns bad after listing

Worth deciding now rather than during the first incident. Removal is not the only move, and reaching for it every time will cost goodwill on false positives.

- [ ] **Agree the ladder.** Ask the author to fix it, then correct the description, then note the limitation in the line, then remove the entry. Removal is the last rung, not the first.
- [ ] **Agree what skips the ladder.** Credential theft, data exfiltration and anything that damages an install come out immediately and get discussed afterwards.
- [ ] **Decide whether removals are announced.** A silent removal is indistinguishable from a reorganisation. One line in the pull request body costs nothing and makes the list's history readable.
- [ ] **Decide the re-listing rule.** A project that was removed and then fixed should have a way back, or authors have no incentive to fix anything.
- [ ] **Decide whether the registry and the list should talk.** A pack banned in the Comfy Registry but still listed here is an inconsistency a reader will find. There is no automation for this, and building some is a larger piece of work than launch needs.

## Staying current without a dated claim

Every one of the 167 links in `README.md` resolved on 2026-10-23. The single exception is the report form, which 404s only because the repository is still private.

Nothing in the list carries a date, a count or a status word, and that should hold. Freshness has to come from checks, not from claims.

- [x] **Add a link checker on a schedule and on pull requests.** `.github/workflows/lint.yml` runs lychee over every markdown file on each pull request, on pushes to `main`, and every Monday. A pull request fails on a dead link. The weekly run does not fail; it opens an issue labelled `report` instead, so rot lands where triage already looks. `.lycheeignore` holds the one URL a machine cannot check, the advisory form, which GitHub shows only to signed-in users.
- [x] **Add `awesome-lint` to the same workflow.** Running, and the list passes clean today.
- [ ] **Decide how the node pack ordering gets refreshed.** `CONTRIBUTING.md` publishes the query that reproduces it and says not to reorder by hand, so either someone runs it periodically or it is scripted. Right now it is neither.
- [ ] **Decide whether archived upstream repositories are removed automatically.** GitHub exposes the archived flag, so this is cheap to detect and it is the single highest-signal rot check after dead links.

## Seeding before launch

Recommend yes, narrowly.

- [ ] **Invite the authors whose work is already listed under From the community.** Most of those entries are other people's projects, listed without them being asked. Telling them before the repository is public turns a surprise into a courtesy, catches descriptions we got wrong, and means launch day has advocates rather than an audience. The node pack authors near the top of the install-count list are the ones worth a direct message.
- [ ] **Do not seed by soliciting new submissions before launch.** An empty list with a queue of pending pull requests is a worse first impression than a full list with none.
- [ ] **Decide whether the showcase entries need their subjects' sign-off.** The studios and schools in Work made with Comfy are already written up on Comfy's own pages, so this is probably covered, but the list repeats claims about named companies in a new venue.
- [x] **Checked the entries that have no public author.** Two were listed by their product site alone, Velorn and ComfyLink, and both turned out to be attributable rather than anonymous: `VelornLabs/velorn`, GPL-3.0, and `huijiutian/ComfyUI-ComfyLink`, MIT, both pushed to in October. Each entry now carries its repository, so nothing has to be dropped. Every other community entry already resolves to a named author, a company or a channel.

## Discoverability

In rough order of how much traffic each is likely to send.

- [x] **GitHub topics.** Set, see above. `awesome-list` is how the topic browsers and the awesome scrapers find a list at all.
- [ ] **Link it from the docs.** A line in the docs community pages, and in `docs.comfy.org/community/links`, which the list itself points at. Reciprocal linking is most of how lists get found.
- [ ] **Add it to `docs.comfy.org/llms.txt`.** The list is a dense, well-structured index of the ecosystem, which is exactly the shape that file exists to serve.
- [ ] **Link it from the registry and from ComfyUI-Manager**, where someone deciding what to install already is.
- [ ] **Submit to the awesome index.** See below. Highest-value single listing, and the slowest.
- [ ] **Announce once, in the places that already exist.** Discord, the forum, the blog. A list does not need a launch campaign.

## The awesome index, specifically

Getting into `sindresorhus/awesome` is worth real traffic, and the list does not currently qualify. The requirements are strict and mechanical.

- [x] **Repository named `awesome-comfy`.** The index requires a lowercase `awesome-*` slug, and `Comfy-Org/awesome-comfy` is the slug. Nothing further to do.
- [x] **The awesome badge** sits to the right of the heading. Required, and present.
- [ ] **Code of conduct required.** Same blocker as above.
- [ ] **Thirty-day age requirement**, counted from the first real commit or from going public. The first commit is 2026-10-07, so the earliest a submission can be made on that reading is 2026-11-06. If the clock runs from going public instead, it starts the day the repository flips.
- [x] **Trailing slashes are not a blocker after all.** Thirty-three entry URLs still end in one, almost all of them comfy.org pages where the slash is the canonical path. `awesome-lint` does not object, so leave them.
- [x] **`awesome-lint` passes with no errors**, and now runs in CI so it keeps passing.
- [ ] **The submission itself is manual work for a person**: the index requires reviewing several other open pull requests with substantive feedback before yours is considered.

## Open legal questions

Drafted, not cleared. Flagged in full in the handover notes, repeated here so they are not lost.

- [ ] **Does the takedown route need a named address, not just an issue form?** No comparable curated list publishes one. Every project that does publish a takedown address hosts the content in question, which this repository does not. A rights-holder complaint is the case where a form may not be an adequate route.
- [ ] **Does linking alone create any obligation?** The disclaimer is written as though it does not, which matches how comparable lists behave, but that is an observation about convention rather than advice.
- [ ] **Does CC0 on the list text interact with linking to differently-licensed projects?** The waiver is written to cover these pages only, and CC0 waives no trademark rights, which matters for a list full of other people's project names. Worth a read by someone qualified.

## Blocked on a human

| Item | Who |
|---|---|
| Primary and backup triager, and accepting the one-week reply time | Unassigned. The single thing that decides whether this list stays alive. |
| Whether the repository gets renamed to `awesome-comfy` | Deep, with whoever owns the org's repository naming |
| Code of conduct enforcement address | Unassigned. Blocks both the file and the awesome index submission. |
| Repository settings: topics, social preview, branch protection, labels, private vulnerability reporting, squash-only merges | Whoever holds admin on the org |
| Social preview image | Whoever owns brand assets |
| Legal review of the disclaimer, the takedown route and the CC0 scope | Unassigned |
| Who may merge a removal without review | Unassigned |
| Going public, and in what order relative to the announcement | Deep |
