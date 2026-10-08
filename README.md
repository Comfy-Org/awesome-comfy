# Awesome Comfy

Things people have built with Comfy: apps you can open, films and campaigns that shipped, and workflows you can run, plus the APIs, SDKs and node packs for building your own.

For artists who want to see what is possible, and for engineers who want to know where to start.

New to Comfy? Install it from the [download page](https://comfy.org/download), run [your first generation](https://docs.comfy.org/get_started/first_generation), then come back.

Entries sit under **From Comfy** for what Comfy Org maintains, and **From the community** for everything else. The community half is other people's work, and listing it is not a safety audit. [How to read this list](#how-to-read-this-list) has the detail, and it is worth reading before you install anything.

## Contents

- [How to read this list](#how-to-read-this-list)
- [Built with Comfy](#built-with-comfy)
- [Work made with Comfy](#work-made-with-comfy)
- [Workflows](#workflows)
- [Build your own](#build-your-own)
- [Node packs](#node-packs)
- [Writing your own nodes](#writing-your-own-nodes)
- [Hosting](#hosting)
- [Getting started](#getting-started)
- [Learning](#learning)
- [Contributing](#contributing)
- [License](#license)

## How to read this list

Sections group entries by what you are trying to do. Inside a section, entries sit under one of two headings.

**From Comfy** means Comfy Org builds, maintains or officially supports it. Problems with it belong on that project's own issue tracker.

**From the community** means someone else builds and maintains it. It is listed because it is useful.

Neither heading is a quality or a safety rating. **From Comfy** says who maintains the thing at the other end of the link, and nothing more than that. A partner integration is not a Comfy product either: where a hosted service or a partner model sits behind a Comfy API, the API is Comfy's and the service is the partner's.

### Installing third-party projects

An entry is checked against [the bar](CONTRIBUTING.md) for fit, not audited for safety. Comfy Org does not certify that a listed project is safe, does not control, test or vet its code, models or data, and may review a listing but does not promise to keep reviewing it. Being on this list is not an endorsement.

Custom nodes and apps are executable code, not metadata. They run with the same access as the Comfy process that loads them, which on a local install is your own user account, your files and your network. Trust a pack as much as you would trust any other software you choose to install: read the source, check who publishes it, and accept that you are the one running it.

If an entry is malicious, misleading or harmful, [report it](https://github.com/Comfy-Org/comfy-awesome/issues/new?template=report-an-entry.yml) and it will be removed. Removing an entry does nothing to the project itself, which stays wherever its author put it.

## Built with Comfy

Products, tools and apps that run Comfy underneath.

### From the community

Made and maintained by other people. Read [Installing third-party projects](#installing-third-party-projects) before you run any of it.

**Tools that put Comfy inside something else:**

- [krita-ai-diffusion](https://github.com/Acly/krita-ai-diffusion) - Inpainting, outpainting and live painting inside Krita, against a local or remote Comfy server.
- [SwarmUI](https://github.com/mcmonkeyprojects/SwarmUI) - A forms-first front end over the same engine, with a Comfy workflow tab when you want the graph back.
- [sd-ppp](https://github.com/zombieyang/sd-ppp) - Drives Comfy from Photoshop, reading and writing layers directly.
- [comfyui-photoshop](https://github.com/NimaNzrii/comfyui-photoshop) - A second Photoshop bridge, with a live-update canvas.
- [ComfyUI-BlenderAI-node](https://github.com/AIGODLIKE/ComfyUI-BlenderAI-node) - Builds and runs Comfy graphs from inside Blender's node editor.

**Apps you can open right now:**

- [Playset](https://comfy-hackathon-8bb.vercel.app) - Generates every asset for a 2D game.
- [Micio](https://micio-rust.vercel.app) - Turns a photo or a chosen breed into an illustrated pet, then adds it to a shared pet cam.
- [Comfy Clash](https://dev-platform-hackathon-team-2.vercel.app) - Generates a deck of original trading cards, then plays them against an opponent.

### From Comfy

**Apps you can open right now:**

- [Emojinius](https://emojinius.comfy.org) - Upload a character and get back a pack of animated Slack emojis.
- [Cinematic Studio](https://comfy.org/hub/apps/cinematic-studio/) - Direct a shot with a real camera, light and grade it, then run it on any image model.
- [Upscale](https://comfy-web-app-template.vercel.app) - A minimal image upscaler, and the template the other web apps start from.

**Clonable app guides**, a working app plus a walkthrough of how it is wired:

- [comfy-cinematic-studio](https://github.com/Comfy-Org/comfy-cinematic-studio) - Source and development guide for Cinematic Studio above.
- [comfy-reshoot](https://github.com/Comfy-Org/comfy-reshoot) - A workflow-deployment app, built to be cloned and changed.

**One-click deploy examples** from [comfy-examples](https://github.com/Comfy-Org/comfy-examples), each a small complete app with a deploy button:

- [anime-opening-machine](https://github.com/Comfy-Org/comfy-examples/tree/main/anime-opening-machine) - Turns one character and a theme into an eight-frame anime opening.
- [comfy-radio](https://github.com/Comfy-Org/comfy-examples/tree/main/comfy-radio) - Tune a wooden radio to one of five fictional stations and ask it for a song.
- [discord-image-bot](https://github.com/Comfy-Org/comfy-examples/tree/main/discord-image-bot) - A Discord bot that generates images in a channel.
- [historical-figures-chat](https://github.com/Comfy-Org/comfy-examples/tree/main/historical-figures-chat) - Ask a historical figure a question and get a short video reply.
- [img2img-web-app](https://github.com/Comfy-Org/comfy-examples/tree/main/img2img-web-app) - Upload an image and get a four-times larger copy back.
- [impossible-food-network](https://github.com/Comfy-Org/comfy-examples/tree/main/impossible-food-network) - Turns a photo of a meal into a surreal food ad, then a six-second spot.
- [museum-of-bad-ideas](https://github.com/Comfy-Org/comfy-examples/tree/main/museum-of-bad-ideas) - Gives a questionable doodle six departments' worth of undeserved prestige.
- [object-removal](https://github.com/Comfy-Org/comfy-examples/tree/main/object-removal) - Mark an unwanted object and let a FLUX Fill workflow rebuild the area.
- [profile-picture-generator](https://github.com/Comfy-Org/comfy-examples/tree/main/profile-picture-generator) - Eight profile shots from one portrait, in five styles.
- [room-remix](https://github.com/Comfy-Org/comfy-examples/tree/main/room-remix) - Pick a room and a mood, then move the furniture around.
- [sketch-to-image](https://github.com/Comfy-Org/comfy-examples/tree/main/sketch-to-image) - Draw a rough guide, describe the result, render it guided by the sketch.
- [smile-compliance](https://github.com/Comfy-Org/comfy-examples/tree/main/smile-compliance) - People Ops has flagged your photo for insufficient enthusiasm.
- [virtual-try-on](https://github.com/Comfy-Org/comfy-examples/tree/main/virtual-try-on) - Pair a person photo with a garment photo and dress one in the other.

**Browse further:**

- [Community apps](https://comfy.org/hub/models/?type=apps) - Apps published by the community.

## Work made with Comfy

Films, campaigns, games and public art. The work is the makers' own, and the credit belongs to the people and studios named in each line. Most of the links are write-ups published by Comfy, so the two headings used elsewhere in this list do not apply here.

**Galleries and roundups:**

- [Gallery](https://comfy.org/gallery/) - Community images, video and 3D, each credited to its maker. The fastest way to see the range.
- [Made with ComfyUI 2025](https://blog.comfy.org/p/made-with-comfyui-2025-from-open) - A year of work in one place, from open-source releases to brand campaigns.
- [Customer stories](https://comfy.org/customers/) - Studios, brands, artists and universities, with a [machine-readable index](https://comfy.org/customers/llms.txt).

**Film and television:**

- [The Song of Drifters](https://comfy.org/customers/xindi-zhang/) - Xindi Zhang built her USC thesis film in Comfy, using her own illustrations as the style guide. It won a [Student Academy Award and reached the Oscar shortlist](https://www.usf.edu/arts/news/2025/20251106-from-thesis-to-oscars-shortlist-xindi-zhang-ai-driven-film-wins.aspx).
- [YUI](https://comfy.org/customers/hakoniwa-yui/) - A 4:20 animated short by 852話 Hakoniwa, made in three days of focused work. ([longer write-up](https://blog.comfy.org/p/creating-the-story-of-yui-with-852))

**Advertising and campaigns:**

- [Svedka, Shake Your Bots Off](https://comfy.org/customers/svedka-silverside/) - Silverside AI rebuilt Svedka's lost Fembot on Comfy workflows for a Super Bowl LX spot.
- [Groove Jones, Crocs x NFL](https://comfy.org/customers/groove-jones/) - A hyper-realistic faux out-of-home holiday campaign, delivered against a short deadline.
- [Silverside AI](https://comfy.org/customers/videos/silverside-ai/) - Silverside AI on why node-based workflows give a creative team more control than single-prompt tools. Video.
- [Black Math](https://comfy.org/customers/videos/black-math/) - Artists and technical directors on building extendable creative systems while keeping art direction. Video.

**Games and 3D:**

- [Series Entertainment](https://comfy.org/customers/series-entertainment/) - Over 100,000 assets across multiple Netflix titles, kept consistent by repeatable workflows. ([case study](https://blog.comfy.org/p/case-study-how-series-entertainment))
- [Ubisoft CHORD](https://comfy.org/customers/ubisoft-chord/) - Ubisoft La Forge open-sourced its PBR material estimation model with Comfy custom nodes. ([announcement](https://blog.comfy.org/p/ubisoft-open-sources-the-chord-model))
- [Doodles and SYSTMS](https://comfy.org/customers/open-story-movement/) - Doodles AI, a generative platform built on open-source infrastructure including Comfy.

**Public art and installations:**

- [Moment Factory](https://comfy.org/customers/moment-factory/) - Rebuilt a 3D projection mapping pipeline for architectural-scale work. ([case study](https://blog.comfy.org/p/case-study-how-moment-factory-reimagined))
- [Ina Conradi's NTU students](https://comfy.org/customers/ina-conradi/) - Ninety-second films for building-sized LED walls, shown at Hangzhou's West Lake media facade.
- [Echoes of Time](https://blog.comfy.org/p/echoes-of-time-lighting-up-a-historic) - A projection piece on Niš Fortress, produced through a Comfy community challenge.

**Studios on their own pipelines**, recorded talks:

- [Reinventing the Production Pipeline](https://comfy.org/events/production-pipeline/) - Erin Sarofsky and Ryan Summers of Sarofsky on rebuilding a studio pipeline around Comfy.
- [Beyond the Models](https://comfy.org/events/beyond-the-models/) - Building custom workflows for commercial and film production.
- [The Future of AI Post Production](https://comfy.org/events/future-ai-post-production/) - Ingi Erlingsson on custom LoRAs and motion graphics nodes in post.
- [How Black Math built a hackathon in three weeks](https://comfy.org/events/black-math-hackathon/) - A design studio shipping an event-scale build.

**Teaching:**

- [Golan Levin, Carnegie Mellon](https://comfy.org/customers/golan-levin/) - "It's an image-processing workstation for completely new kinds of work."
- [Kathy Smith, USC](https://comfy.org/customers/kathy-smith/) - Inside the Expanded Animation MFA that built a curriculum around it.
- [UAL Creative Computing Institute](https://comfy.org/customers/ual-cci/) - A teaching and research partnership across masters, PhD and industry programmes.

**Events:**

- [Events](https://comfy.org/events/) - Livestreams, hackathons and meetups, upcoming and recorded, with a [machine-readable index](https://comfy.org/events.md).

## Workflows

### From Comfy

- [comfy.org/workflows](https://comfy.org/workflows) - Browsable catalogue of runnable workflows with the models each one needs.
- [Character replacement](https://comfy.org/workflows/use-cases/ai-character-replacement/) - Swapping a character into existing footage.
- [Image to video](https://comfy.org/workflows/use-cases/ai-image-to-video/) - Animating a still.
- [Sprite sheets](https://comfy.org/workflows/use-cases/sprite-sheet-generator/) - Game-ready sprite sheet generation.
- [Restore old photos](https://comfy.org/workflows/use-cases/restore-old-photos/) - Damage repair and colourisation.
- [Image to 3D](https://comfy.org/workflows/use-cases/image-to-3d/) - Single image to a mesh.
- [workflow_templates](https://github.com/Comfy-Org/workflow_templates) - The source of the templates that ship inside Comfy. Open a pull request here to add one.
- [Using templates](https://docs.comfy.org/interface/features/template) - How the built-in template browser works.
- [ComfyUI_examples](https://comfyanonymous.github.io/ComfyUI_examples/) - The original example gallery. Images carry embedded workflows you can drag onto the canvas.
- [example_workflows](https://github.com/Comfy-Org/example_workflows) - Archive of example workflow JSON.
- [Workflow JSON spec](https://docs.comfy.org/specs/workflow_json) - The on-disk format, for reading or writing workflows programmatically.
- [API workflow format](https://docs.comfy.org/development/api-development/workflow-api-format) - The flattened form you POST to a server.

## Build your own

The API surfaces, SDKs and hosted endpoints for driving Comfy from your own code.

### From Comfy

- [Development overview](https://docs.comfy.org/development/overview) - Map of the API surfaces and which one you want.
- [API quickstart](https://docs.comfy.org/development/api-development/quickstart) - Submit a workflow and collect the result in a few calls.
- [Getting an API key](https://docs.comfy.org/development/api-development/getting-an-api-key) - Required for the hosted API.

**Comfy Router**, one API in front of many hosted image, video and audio models:

- [Router quickstart](https://docs.comfy.org/development/comfy-router/quickstart) - One POST, no graph to build.
- [Model catalogue](https://docs.comfy.org/development/comfy-router/models) - Every model it can run, with per-model input and output schemas.
- [Pricing](https://docs.comfy.org/development/comfy-router/pricing) - Per-model cost, which you want before you build on it.
- [API reference](https://docs.comfy.org/development/comfy-router/api) - Run, queue, poll and cancel.

**Developer Platform**, for running your own workflows as a service:

- [Cloud API overview](https://docs.comfy.org/development/cloud/overview) - Assets, jobs, queue and history against hosted Comfy.
- [Serverless overview](https://docs.comfy.org/development/serverless/overview) - Turn a workflow into an endpoint you can call.

**SDKs:**

- [SDK overview](https://docs.comfy.org/development/api-development/sdks) - What the clients cover and the shape they share.
- [Python SDK](https://github.com/Comfy-Org/comfy-python-sdk) - Client for self-hosted Comfy and Comfy Cloud.
- [TypeScript SDK](https://github.com/Comfy-Org/comfy-typescript-sdk) - Same surface, for Node and the browser.
- [Swift SDK](https://github.com/Comfy-Org/comfy-swift-sdk) - Thin client: submit, stream, collect outputs.

**Comfy MCP:**

- [Comfy MCP](https://comfy.org/mcp) - The hosted endpoint and what it can do.
- [comfy-mcp](https://github.com/Comfy-Org/comfy-mcp) - Exposes a local Comfy over the Model Context Protocol.
- [MCP documentation](https://docs.comfy.org/agent-tools/mcp) - Setup and the tools the server exposes.

**Talking to a Comfy server directly:**

- [Server API overview](https://docs.comfy.org/development/comfyui-server/comms_overview) - The REST and WebSocket model the editor itself uses.
- [Route reference](https://docs.comfy.org/development/comfyui-server/comms_routes) - Every endpoint a running server exposes.
- [API examples](https://docs.comfy.org/development/comfyui-server/api-examples) - Working scripts for queueing prompts and reading results.
- [comfy-api-proxy](https://github.com/Comfy-Org/comfy-api-proxy) - Puts the v2 API in front of a self-hosted instance, so one client works against both.

### From the community

Read [Installing third-party projects](#installing-third-party-projects) first.

**Writing workflows as code:**

- [ComfyScript](https://github.com/Chaoses-Ib/ComfyScript) - Write workflows as Python instead of JSON.
- [ComfyUI-to-Python-Extension](https://github.com/pydn/ComfyUI-to-Python-Extension) - Exports a saved workflow as a standalone Python script.

## Node packs

Custom nodes are how Comfy grows.

### From Comfy

**Install and manage them with:**

- [ComfyUI-Manager](https://github.com/Comfy-Org/ComfyUI-Manager) - Installs, updates, disables and security-scans node packs from inside the editor. Most people's entry point to everything below.
- [Comfy Registry](https://registry.comfy.org/) - The package index. Search it before you install anything from a random clone URL.
- [Registry overview](https://docs.comfy.org/registry/overview) - What the registry is, how versions and publishers work.
- [Publishing to the registry](https://docs.comfy.org/registry/publishing) - For node authors shipping a pack.
- [Node standards](https://docs.comfy.org/registry/standards) - The naming, metadata and dependency rules a pack is expected to follow.
- [Registry CI/CD](https://docs.comfy.org/registry/cicd) - Publish on tag from GitHub Actions.
- [Installing custom nodes](https://docs.comfy.org/installation/install_custom_node) - The manual route, and what it writes to disk.
- [Custom node troubleshooting](https://docs.comfy.org/troubleshooting/custom-node-issues) - Import errors, dependency conflicts and how to bisect them.

### From the community

Every pack below is third-party code that runs inside your Comfy process. Read [Installing third-party projects](#installing-third-party-projects) first.

**The 40 most-installed packs**, ordered by Comfy Registry install count. Reproduce the ordering with:

```
curl -s "https://api.comfy.org/nodes?page=1&limit=100&sort=total_install%3Bdesc&latest=true"
```

- [ComfyUI-KJNodes](https://github.com/kijai/ComfyUI-KJNodes) - Large grab-bag of utility nodes, heavy on video, masking and batch helpers.
- [rgthree-comfy](https://github.com/rgthree/rgthree-comfy) - Graph quality of life: reroutes, muting, seed control, progress bars, bookmarks.
- [ComfyUI-Easy-Use](https://github.com/yolain/ComfyUI-Easy-Use) - Condensed loader and sampler nodes that collapse common chains into one node.
- [ComfyUI-VideoHelperSuite](https://github.com/Kosinkadink/ComfyUI-VideoHelperSuite) - Load, batch and recombine video and image sequences.
- [ComfyUI-Impact-Pack](https://github.com/ltdrdata/ComfyUI-Impact-Pack) - Detection-driven detailing: detectors, detailers, upscalers and pipes.
- [ComfyUI-Custom-Scripts](https://github.com/pythongosssss/ComfyUI-Custom-Scripts) - Editor conveniences: prompt autocomplete, pinned favourites, image feed.
- [ComfyUI_essentials](https://github.com/cubiq/ComfyUI_essentials) - Image, mask and conditioning primitives missing from core. In maintenance mode.
- [comfyui_controlnet_aux](https://github.com/Fannovel16/comfyui_controlnet_aux) - The preprocessors ControlNet needs: depth, pose, lineart, normals, segmentation.
- [ComfyUI-GGUF](https://github.com/city96/ComfyUI-GGUF) - Run GGUF-quantised checkpoints and text encoders against native Comfy model code.
- [ComfyUI-Crystools](https://github.com/crystian/ComfyUI-Crystools) - Live resource monitor plus pipe, debug and metadata nodes.
- [ComfyUI-Impact-Subpack](https://github.com/ltdrdata/ComfyUI-Impact-Subpack) - The Impact Pack nodes kept out of the main pack, mostly the Ultralytics detector.
- [ComfyUI_LayerStyle](https://github.com/chflame163/ComfyUI_LayerStyle) - Photoshop-style layer, blend and mask compositing.
- [cg-use-everywhere](https://github.com/chrisgoringe/cg-use-everywhere) - Broadcasts an output to every matching input, so MODEL, CLIP and VAE wires leave the graph.
- [ComfyUI-WanVideoWrapper](https://github.com/kijai/ComfyUI-WanVideoWrapper) - Wrapper nodes for the Wan video models, with block swapping and offload controls.
- [ComfyUI-Frame-Interpolation](https://github.com/Fannovel16/ComfyUI-Frame-Interpolation) - Frame interpolation (RIFE, FILM and others) for smoothing video output.
- [ComfyUI_UltimateSDUpscale](https://github.com/ssitu/ComfyUI_UltimateSDUpscale) - Tiled diffusion upscaling, the Ultimate SD Upscale script as nodes.
- [ComfyUI-Florence2](https://github.com/kijai/ComfyUI-Florence2) - Florence-2 captioning, grounding and region detection.
- [ComfyUI_IPAdapter_plus](https://github.com/cubiq/ComfyUI_IPAdapter_plus) - Reference IPAdapter implementation for image-to-image conditioning and style transfer. In maintenance mode.
- [ComfyUI-mxToolkit](https://github.com/Smirnov75/ComfyUI-mxToolkit) - Minimal layout and control nodes: sliders, seeds, reroutes, dot markers.
- [comfyui-deno-custom-nodes](https://github.com/Deno2026/comfyui-deno-custom-nodes) - NVIDIA-oriented nodes: RTX video super resolution, nvvfx effects, compare and preview helpers.
- [was-node-suite-comfyui](https://github.com/WASasquatch/was-node-suite-comfyui) - Over 200 nodes for image processing, filters, text, logic, numbers and files.
- [efficiency-nodes-comfyui](https://github.com/jags111/efficiency-nodes-comfyui) - Collapses loader, sampler and upscale into a handful of nodes, with XY plotting.
- [ComfyUI-SeedVR2_VideoUpscaler](https://github.com/numz/ComfyUI-SeedVR2_VideoUpscaler) - SeedVR2 video restoration and upscaling.
- [gguf](https://github.com/calcuis/gguf) - A second GGUF loader implementation, independent of ComfyUI-GGUF.
- [comfy_mtb](https://github.com/melMass/comfy_mtb) - Animation-oriented utilities: interpolation curves, masks, image operations.
- [ComfyUI-Image-Saver](https://github.com/alexopus/ComfyUI-Image-Saver) - Saves images with Civitai-compatible generation metadata.
- [ComfyUI-Inspire-Pack](https://github.com/ltdrdata/ComfyUI-Inspire-Pack) - Prompt scheduling, regional conditioning and noise control nodes.
- [ComfyUI-ReActor](https://github.com/Gourieff/ComfyUI-ReActor) - Face swapping and face restoration.
- [ComfyUI-RMBG](https://github.com/1038lab/ComfyUI-RMBG) - Background removal and segmentation across RMBG-2.0, BiRefNet, SAM and others.
- [ComfyUI-Inpaint-CropAndStitch](https://github.com/lquesada/ComfyUI-Inpaint-CropAndStitch) - Crops to the mask before sampling and stitches back after, which makes inpainting much faster.
- [comfyui-art-venture](https://github.com/sipherxyz/comfyui-art-venture) - Utilities for image processing, JSON manipulation, model operations and loading assets from URLs.
- [ComfyUI-Lora-Manager](https://github.com/willmiao/ComfyUI-Lora-Manager) - Browse, tag and preview LoRAs from inside the editor.
- [ComfyUI-Detail-Daemon](https://github.com/Jonseed/ComfyUI-Detail-Daemon) - Adjusts sigmas to control fine detail, ported from sd-webui-Detail-Daemon.
- [ComfyUI-Advanced-ControlNet](https://github.com/Kosinkadink/ComfyUI-Advanced-ControlNet) - ControlNet scheduling, masking and sliding-window context.
- [ComfyUI-LogicUtils](https://github.com/aria1th/ComfyUI-LogicUtils) - Logic, math and list primitives for building conditional graphs.
- [ControlAltAI-Nodes](https://github.com/gseth/ControlAltAI-Nodes) - Quality-of-life nodes: Flux resolution calculator, Flux sampler, boolean and integer logic.
- [ComfyUI-AnimateDiff-Evolved](https://github.com/Kosinkadink/ComfyUI-AnimateDiff-Evolved) - AnimateDiff with advanced sampling and context scheduling.
- [ComfyUI_tinyterraNodes](https://github.com/TinyTerra/ComfyUI_tinyterraNodes) - Pipe-based workflow nodes, an XY plot node and a fullscreen image viewer.
- [ComfyUI-TeaCache](https://github.com/welltop-cn/ComfyUI-TeaCache) - Timestep Embedding Aware Cache, a training-free way to speed up diffusion inference.
- [ComfyUI-WD14-Tagger](https://github.com/pythongosssss/ComfyUI-WD14-Tagger) - WD14 image tagging, for captioning and dataset preparation.

## Writing your own nodes

### From Comfy

- [Custom node overview](https://docs.comfy.org/custom-nodes/overview) - Start here if you are writing your first node.
- [Walkthrough](https://docs.comfy.org/custom-nodes/walkthrough) - Builds a working node from an empty folder.
- [Server-side reference](https://docs.comfy.org/custom-nodes/backend/server_overview) - `INPUT_TYPES`, `RETURN_TYPES`, `FUNCTION`, lifecycle and the rest of the contract.
- [Datatypes](https://docs.comfy.org/custom-nodes/backend/datatypes) - The type system that decides which sockets connect.
- [Shipping templates with a pack](https://docs.comfy.org/custom-nodes/workflow_templates) - So users get an example workflow on install.
- [cookiecutter-comfy-extension](https://github.com/Comfy-Org/cookiecutter-comfy-extension) - Scaffolds a publishable node pack with the metadata already correct.
- [ComfyUI-React-Extension-Template](https://github.com/Comfy-Org/ComfyUI-React-Extension-Template) - Minimal template for a React and TypeScript front-end extension.
- [ComfyUI_devtools](https://github.com/Comfy-Org/ComfyUI_devtools) - Test fixtures and debugging aids used by the core test suites.
- [ComfyUI_frontend](https://github.com/Comfy-Org/ComfyUI_frontend) - The Vue front end the editor runs on.
- [comfyui-native-port-guide](https://github.com/Comfy-Org/comfyui-native-port-guide) - Conventions for adding native model support to core, rather than wrapping it in a pack.
- [rfcs](https://github.com/Comfy-Org/rfcs) - Design proposals for substantial changes to core, the APIs and the standards.
- [comfy-action](https://github.com/Comfy-Org/comfy-action) - GitHub Action that sets up Comfy and runs a workflow, for testing a pack in CI.
- [embedded-docs](https://github.com/Comfy-Org/embedded-docs) - The help pages shown inside the editor, and how to add yours.
- [comfy-model-tools](https://github.com/Comfy-Org/comfy-model-tools) - Scripts for packaging and converting models into the layouts Comfy expects.
- [comfyui-benchmark](https://github.com/Comfy-Org/comfyui-benchmark) - Extension for measuring generation performance across configurations.

## Hosting

### From Comfy

- [Self-hosting guide](https://docs.comfy.org/development/deploy/self-hosting) - Running Comfy on a rented GPU.

### From the community

Independent providers and images. Comfy Org does not operate these services, hold your data on them, or set their prices. Read [Installing third-party projects](#installing-third-party-projects) first.

- [ComfyUI-Docker](https://github.com/YanWenKun/ComfyUI-Docker) - Container images across several CUDA and Python combinations.
- [RunComfy](https://www.runcomfy.com/) - Hosted unmodified Comfy with preloaded models, plus a serverless API. ([API docs](https://docs.runcomfy.com/))
- [ComfyDeploy](https://www.comfydeploy.com/) - Turns a workflow into a versioned API endpoint, with a team layer on top. ([docs](https://docs.comfydeploy.com/docs/introduction))
- [Replicate](https://replicate.com/docs/guides/extend/comfyui) - Run a workflow as a Replicate model, including arbitrary custom nodes. ([cog-comfyui](https://github.com/replicate/cog-comfyui))
- [SaladCloud](https://docs.salad.com/container-engine/how-to-guides/ai-machine-learning/deploy-stable-diffusion-comfy) - Deployment recipe for their container engine. ([comfyui-api](https://github.com/SaladTechnologies/comfyui-api))

## Getting started

### From Comfy

- [ComfyUI](https://github.com/Comfy-Org/ComfyUI) - The node-graph engine itself: a workflow runner for diffusion models with a Python backend.
- [Download page](https://comfy.org/download) - Picks the right install path for your machine.
- [System requirements](https://docs.comfy.org/installation/system_requirements) - Read this before you pick an install method.
- [Desktop app](https://docs.comfy.org/installation/desktop/overview) - Packaged installer for Windows, macOS and Linux. The shortest path to a working setup.
- [Comfy Desktop source](https://github.com/Comfy-Org/Comfy-Desktop) - The desktop app repository.
- [Manual install](https://docs.comfy.org/installation/manual_install) - Clone and pip, for when you want to control the Python environment.
- [Portable Windows build](https://docs.comfy.org/installation/comfyui_portable_windows) - Self-contained folder, no installer, no system Python.
- [Your first generation](https://docs.comfy.org/get_started/first_generation) - Walks a default workflow end to end and explains what each node did.
- [Interface tour](https://docs.comfy.org/interface/overview) - The canvas, the queue, the model library and the settings that matter early.
- [Comfy Cloud](https://docs.comfy.org/get_started/cloud) - Hosted Comfy, for when you do not have the GPU.
- [comfy-cli](https://github.com/Comfy-Org/comfy-cli) - Command-line installer and manager for Comfy, models and node packs.
- [comfy-cli docs](https://docs.comfy.org/comfy-cli/getting-started) - Install, launch, snapshot and switch between versions.
- [Troubleshooting](https://docs.comfy.org/troubleshooting/overview) - Start here when something breaks, before opening an issue.

## Learning

### From Comfy

- [Official documentation](https://docs.comfy.org/) - The canonical reference for installation, nodes, models and the APIs.
- [llms.txt](https://docs.comfy.org/llms.txt) - The whole documentation index as one plain-text file, which is the fastest way to find a page.
- [Nodes](https://docs.comfy.org/basic-concepts/nodes) and [models](https://docs.comfy.org/basic-concepts/models) - The two concepts everything else is built on.
- [Basic tutorials](https://docs.comfy.org/tutorials/basic/text-to-image) - Text to image, image to image, inpaint, outpaint, upscale and LoRA, as annotated workflows.
- [Blog](https://blog.comfy.org/) - Official release notes, case studies and announcements.
- [Forum](https://forum.comfy.org/) - Longer-form questions and answers that outlive a chat message.
- [Discord](https://discord.com/invite/comfyorg) - Where most day-to-day help happens.
- [YouTube](https://www.youtube.com/@comfyorg) - Official walkthroughs and release videos.
- [Community links](https://docs.comfy.org/community/links) - The official list of community spaces.
- [Contributing to ComfyUI](https://docs.comfy.org/community/contributing) - How to get a change into core.

### From the community

- [ComfyUI Wiki](https://comfyui-wiki.com/en) - Reference covering installs, nodes and models.
- [Latent Vision](https://www.youtube.com/@latentvision) - Deep explanations of conditioning, IPAdapter and sampler behaviour, from the IPAdapter author.
- [Nerdy Rodent](https://www.youtube.com/@NerdyRodent) - Regular walkthroughs of new models and workflows.
- [Scott Detweiler](https://www.youtube.com/@sedetweiler) - Long-running beginner-to-intermediate series.

## Contributing

Built something with Comfy? Add it. [SUBMISSION_GUIDELINES.md](SUBMISSION_GUIDELINES.md) is the short path: one line, one file, one pull request. [CONTRIBUTING.md](CONTRIBUTING.md) is the bar an entry has to clear.

Removals are as welcome as additions. So is [reporting an entry](https://github.com/Comfy-Org/comfy-awesome/issues/new?template=report-an-entry.yml) that should not be here.

## License

[CC0-1.0](LICENSE). The list content is in the public domain. Linked projects keep their own licenses, and the CC0 waiver covers these pages only, not anything they point at.
