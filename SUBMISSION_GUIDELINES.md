# Submitting an entry

Built something with Comfy? Add it. It is one line, in one file, in one pull request.

This page is the path. [CONTRIBUTING.md](CONTRIBUTING.md) is the bar an entry has to clear, and it is worth a skim before you start. Work you made yourself is the most welcome kind of submission.

## The whole thing, in one example

Open [README.md](README.md), press the edit pencil, and add one line to the group your project belongs in:

```
- [krita-ai-diffusion](https://github.com/Acly/krita-ai-diffusion) - Inpainting, outpainting and live painting inside Krita, against a local or remote Comfy server.
```

The shape is always the same:

```
- [Name](https://url) - One sentence, ending in a period.
```

- **Name** as its author writes it. The repository name is usually right.
- **URL** that a stranger with no account can open, and that returns 200 today.
- **One sentence** saying what it does. Not what it aspires to.

Then open the pull request and fill in the template. Nothing else is required.

## A worked example

Say you built a DaVinci Resolve panel. The entry line:

```
- [Lanternfish](https://github.com/example/lanternfish) - A DaVinci Resolve panel that sends a timeline clip to your own Comfy server and returns the result as a new track.
```

The pull request body, which follows the template:

```
## What are you adding or removing?

- [Lanternfish](https://github.com/example/lanternfish) - A DaVinci Resolve panel that sends a timeline clip to your own Comfy server and returns the result as a new track.

## Where does it go, and why does it belong?

Built with Comfy, From the community, under "Tools that put Comfy inside something else".
Nothing on the list reaches Resolve today, and Comfy is the only backend: the panel
does nothing without a running server.

Source: https://github.com/example/lanternfish
Demo: https://lanternfish.example/demo
Video: https://youtu.be/example (80 seconds, Resolve to Comfy and back)

## Disclosure

I wrote it.
```

Four things make that reviewable in one pass: the line itself, where it goes, links a
stranger can open, and whether you made it. Lanternfish is not real, so do not submit it.

## Where does it go

| What you have | Section | Heading |
|---|---|---|
| A product, tool or app that runs Comfy underneath | Built with Comfy | From the community |
| A film, campaign, game, installation or exhibited work | Work made with Comfy | no heading, see below |
| A runnable workflow, or a spec for the workflow format | Workflows | From the community |
| A library, SDK, client or code generator for driving Comfy | Build your own | From the community |
| A template or tool for people writing nodes | Writing your own nodes | From the community |
| A hosting provider, container image or deployment recipe | Hosting | From the community |
| An install path or first-run guide | Getting started | From the community |
| Docs, a course, a channel, a wiki, a community space | Learning | From the community |

Your entry goes under **From the community** unless Comfy Org's own team built it. Being a Comfy partner, customer or integration does not make an entry **From Comfy**.

**Work made with Comfy** has no affiliation heading, because the work there is always the maker's own. Pick the sub-group that fits: film and television, advertising and campaigns, games, studios and 3D, public art and installations, teaching.

If nothing fits, [open an issue](https://github.com/Comfy-Org/awesome-comfy/issues/new) and say what a reader cannot currently find. Adding a section is a bigger change than adding an entry.

## The description line

One sentence. What it does, who it is for if that is not obvious from the name, and what it does not do. Then stop.

Good:

```
- [ComfyUI-Inpaint-CropAndStitch](https://github.com/lquesada/ComfyUI-Inpaint-CropAndStitch) - Crops to the mask before sampling and stitches back after, which makes inpainting much faster.
- [ComfyUI-TD](https://github.com/JiSenHua/ComfyUI-TD) - Streams images, video, point clouds and audio from Comfy into TouchDesigner in real time.
- [OpenLayer](https://mehran-ahmadi.com/OpenLayer/) - A Photoshop panel that generates, inpaints and upscales through your own Comfy server and hands back editable layers. Alpha.
```

Each of those says what the thing does, and the third says what you also need to know before you install it.

Not good, and why:

| Line | Problem |
|---|---|
| `- [FooEditor](...) - The best and most powerful Comfy front end ever built!` | Superlatives. Say what it does. |
| `- [FooEditor](...) - A Comfy tool.` | Says nothing a reader can act on. |
| `- [FooEditor](...) - Edits video. Also does masks. Plus some upscaling. Work in progress, more coming soon!` | Several sentences, and a roadmap. One sentence, present tense, what exists today. |
| `- [FooApp](...) - The next-generation creative suite, reimagined` | Marketing, no period, and still does not say what it does. No emoji either. |
| `- [FooApp](...) - Generates video from text.` when it plays a pre-rendered clip | Claims behaviour the thing does not have. This gets closed. |

Limitations belong in the line. One platform only, one model family only, a weekend build rather than a product: say so. It makes the entry more useful, not less, and it is the difference between a reader thanking you and a reader filing an issue.

## What gets turned down

Most of these are fixable in a follow-up commit.

- **A stranger cannot open it.** Private repository, login wall on the landing page, invite-only space, dead link.
- **The link does not resolve.** Check it the day you submit.
- **Comfy is optional.** If Comfy is one backend among several and the project works fine without it, it is not built with Comfy.
- **Something already covers it.** Say what yours does differently. Two entries doing the same thing is a reason to replace one, not to add another.
- **It is a custom node pack.** The [Comfy Registry](https://registry.comfy.org/) indexes those, searchable and ranked by install count, and it is current in a way this list cannot be. Publish there instead.
- **Nothing has happened in a long time.** A repository needs a recent commit and must not be archived. If the author has called it finished, say so in the pull request and the line can carry that.
- **The showcase claim is not public.** For **Built with Comfy** and **Work made with Comfy**, the Comfy connection has to be stated somewhere a reader can check. Quote that sentence in the pull request and link it. "I am fairly sure they used it" does not clear the bar.
- **It is a model or a checkpoint.** This list indexes work and tools, not weights.
- **It leaks something.** Private addresses, internal URLs, keys, customer data. Also any public app that exposes a destructive action to anonymous visitors.

The full list is in [CONTRIBUTING.md](CONTRIBUTING.md).

## Scope of a pull request

One pull request per addition, unless the additions are a coherent set. If you are changing someone else's entry, or removing one, say why in the description. Removals are welcome.

## What happens after you submit

There is no response time on this and no promise of one. There is no staffed queue behind the list, so a pull request can sit, and nothing here commits anyone to replying by any particular day. Bump it if it goes quiet.

Worth knowing before you spend effort on an entry rather than after. A pull request is still the faster of the two routes, because the edit is already written and there is nothing left to do but merge it.

## If you would rather not open a pull request

[Suggest an entry](https://github.com/Comfy-Org/awesome-comfy/issues/new?template=suggest-an-entry.yml) in an issue instead. A pull request is the faster path, because the edit is already written.

## Submitting on behalf of someone else

Fine, and often useful. Link the public evidence, do not speak for the author, and do not claim features you have not seen work.

## What a listing means, and does not

Entries under **From the community** are other people's work. An entry is checked against the bar for fit, not audited for safety. Comfy Org does not certify that a listed project is safe, does not vet its code, models or data, and does not take responsibility for what it does. Readers install at their own risk, and the [note in the README](README.md#installing-third-party-projects) says so plainly.

By submitting, you are confirming that the entry text is yours to contribute under [CC0-1.0](LICENSE). That covers the line you wrote here. It does not change the license of the project you are linking to, and it does not transfer any name, logo or trademark.

If something on the list turns out to be malicious, misleading or harmful, [report it](https://github.com/Comfy-Org/awesome-comfy/issues/new?template=report-an-entry.yml). Removing an entry does nothing to the project itself, which stays wherever its author put it.
