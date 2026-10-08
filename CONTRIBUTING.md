# Contributing

This list indexes what people have built with Comfy, and the tools they built it with. Work you made yourself is the most welcome kind of submission, so say it is yours and submit it.

Submitting something? [SUBMISSION_GUIDELINES.md](SUBMISSION_GUIDELINES.md) is the short path: where the entry goes, how the line is shaped, and what happens next. This file is the bar an entry has to clear, and it is the one that settles arguments.

## The bar for everything

1. **It is public and openable by a stranger.** No private repositories, no login walls on the landing page, no invite-only spaces. If a reader cannot open it, it does not go in.
2. **The link resolves.** Every URL must load and return 200. Check it the day you submit. A dead link is a bug, and a link that cannot be opened is the same as a dead one.

   A 200 is not proof the page exists. Plenty of hosts serve a soft 200 for a path that is gone, including Steam app pages, YouTube watch URLs, registry node pages, Notion sites and OpenArt. Open the page and confirm it contains what your line says. Two checks that do not lie: `https://api.comfy.org/nodes/<id>` for a node pack, and YouTube's oembed endpoint for a video.
3. **It is described honestly.** One line, factual, no marketing. If something only works on one platform, only with one model family, or is a weekend build rather than a product, the line should say so.

## The extra bar for showcase entries

For anything in **Built with Comfy** or **Work made with Comfy**:

4. **The Comfy connection is stated somewhere public.** By the maker, the studio, a named publication, or Comfy's own site. Point at that statement in the pull request and quote the sentence. "I am fairly sure they used it" is not evidence.
5. **An entry states what a thing is, plainly.** It does not hedge about how well sourced it is. If a claim is not solid enough to make without a caveat, it is not solid enough to list.
6. **It is real finished work**, or a real working app. Not a tech demo dressed up as a product, and not a screenshot.
7. **It does what the entry says it does.** If an app is a pre-rendered mockup, the line must not claim it generates anything.

## The extra bar for tools and repositories

8. **It is maintained.** A repository needs a commit in the last 18 months, and must not be archived or blocked. A site or channel needs something published in the last 18 months. If the author has declared the project finished or in maintenance mode, say so in the pull request and the entry can carry that status.
9. **Comfy is load-bearing.** A tool where Comfy is one optional backend among many is not "built with Comfy". The README should say Comfy is what it runs on.
10. **It is distinct.** If an existing entry covers the same ground, say what yours does differently. Two tools that do the same thing is a reason to replace, not append.
11. **A node pack is in the registry.** If the submission is a node pack, it is published in the [Comfy Registry](https://registry.comfy.org/).

## Which heading an entry goes under

Most sections are split into **From Comfy** and **From the community**. The split is about one thing: who maintains and supports the project at the other end of the link.

12. **From Comfy** is for projects Comfy Org builds, maintains or officially supports. In practice that is the `Comfy-Org` GitHub organisation, `comfy.org` and its subdomains, and the official Discord, forum and YouTube channel. Nothing else qualifies, including a fork of a Comfy Org project.
13. **A partner, customer or integration is not From Comfy.** A hosting provider that runs Comfy, a studio that shipped work with it, a partner model reachable through a Comfy API: all of those are **From the community**. Where a partner model sits behind a Comfy API, the API is Comfy's and the model is the partner's, and the entry follows whichever one it links to.
14. **Neither heading is a rating.** Do not move an entry between headings to signal quality, maturity or preference, and do not add a third heading for a closer relationship. If affiliation is genuinely unclear, say so in the pull request rather than picking one.

**Work made with Comfy** is the exception and carries no headings. The work in that section is always the maker's own, even though most of the links are write-ups published by Comfy.

## What does not belong

- Anything that leaks private information: addresses, internal URLs, keys, customer data. This is the fastest way to get a submission closed.
- Anything with destructive actions exposed to anonymous visitors. A public app with an unauthenticated delete button is a liability, not a showcase.
- Internal or staging sites that happen to be reachable.
- Content that puts words in the mouth of a real, named person.
- Paid products described as free, or free tiers described as the product.
- Link farms, SEO pages, and sites that wrap official documentation in ads.
- Anything abandoned, however historically important. The git history is still there.
- Models and checkpoints. This indexes work and tools, not weights.
- Forks, unless the fork is now the maintained line and the original is not.

## Ordering

The node pack section is ordered by Comfy Registry install count, not by preference. The ordering is reproducible:

```
curl -s "https://api.comfy.org/nodes?page=1&limit=100&sort=total_install%3Bdesc&latest=true"
```

Do not reorder it by hand. If a pack belongs there, it will arrive on the next refresh.

Other sections lead with the things most worth a reader's first click. That applies to the **From Comfy** and **From the community** headings too: either can come first in a section, whichever puts the better first click at the top. The headings label the groups, they do not rank them.

## How to propose an addition

[SUBMISSION_GUIDELINES.md](SUBMISSION_GUIDELINES.md) walks the whole path, including the entry format and the section table. One pull request per addition, unless the additions are a coherent set.

## Removals

Removals are as welcome as additions, and usually more useful. Open a pull request that removes the entry and say why, or [report it](https://github.com/Comfy-Org/comfy-awesome/issues/new?template=report-an-entry.yml) if you would rather not.

An entry comes out when:

- The link is dead, or the project has been deleted or archived.
- The project has been abandoned, and the entry does not say so.
- The entry misdescribes what the project does.
- The project has started doing something harmful: shipping malicious code, exfiltrating data, breaking an install, or exposing something it should not.
- A rights holder objects to how their name, mark or work appears in the entry.

A removal for malicious behaviour needs evidence, not a scanner screenshot. Name the project, the version or commit, the exact file or lines, and what the code does. More than one independent source where you can. An antivirus or registry scanner result can support a case but does not settle one on its own, because scanners produce false positives and node packs legitimately read files, write to disk and reach the network.

Not every problem is a removal. An entry whose description has drifted gets a corrected description. A project whose author has called it finished gets that stated in the line. Removal is for entries a reader is better off not seeing at all.

Taking an entry out of this list does nothing to the project. It stays wherever its author put it, and it may still be installable from the registry or from GitHub.

## Changes to the structure

Adding or renaming a section is a bigger change than adding an entry. Open an issue first and explain what a reader cannot find in the list as it stands.

## License

The list is released under [CC0-1.0](LICENSE), and contributions go in under the same terms.

The waiver covers the text of these pages: the entries, the descriptions and the way they are organised. It does not reach anything the list points at. Linked projects keep their own licenses, and CC0 waives no trademark or patent rights, so a project name or logo appearing in an entry is still its owner's.
