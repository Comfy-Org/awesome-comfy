# Contributing

This list indexes what people have built with Comfy, and the tools they built it with. Work you made yourself is the most welcome kind of submission, so say it is yours and submit it.

## The bar for everything

1. **It is public and openable by a stranger.** No private repositories, no login walls on the landing page, no invite-only spaces. If a reader cannot open it, it does not go in.
2. **The link resolves.** Every URL must load and return 200. Check it the day you submit. A dead link is a bug, and a link that cannot be opened is the same as a dead one.
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

Other sections lead with the things most worth a reader's first click.

## How to propose an addition

1. Fork and branch.
2. Add one entry per line, in the section it belongs to, in the format used by the rest of the file:

   ```
   - [Name](https://example.com) - One factual line, ending in a period.
   ```

3. Open a pull request and complete the checklist in the template.

One pull request per addition, unless the additions are a coherent set.

## Removals

Removals are as welcome as additions, and usually more useful. If an entry is dead, abandoned, misleading, or exposes something it should not, open a pull request that removes it and say why.

## Changes to the structure

Adding or renaming a section is a bigger change than adding an entry. Open an issue first and explain what a reader cannot find in the list as it stands.

## License

The list is released under [CC0-1.0](LICENSE), and contributions go in under the same terms. Linked projects keep their own licenses.
