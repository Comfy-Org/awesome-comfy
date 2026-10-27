# Awesome Comfy [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Things people have built with Comfy: apps and plugins people shipped, films and campaigns that aired, and workflows you can run, plus the APIs and SDKs for building your own.

For artists who want to see what is possible, and for engineers who want to know where to start.

Inside each section, entries sit under **From Comfy** for what Comfy Org's own team built and **From the community** for everything else. How to read this list, just below, says what those headings do and do not tell you, and it is worth a minute before you install anything.

Built something with Comfy? [Add it](SUBMISSION_GUIDELINES.md). Removals are as welcome as additions.

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

## How to read this list

Sections group entries by what you are trying to do. Inside most sections, entries sit under one of two headings.

**From Comfy** means Comfy Org's own team built it, and that is the whole claim. Some of it is maintained software on a release cadence, and plenty of it is a demo, an example app or a weekend build that works and that nobody is tending. So a problem belongs on that project's own issue tracker, rather than with someone you have assumed is watching. **From the community** means someone else built it, and it is listed because it is useful.

Neither heading is a quality rating, a safety rating or a support commitment. Both say who wrote the thing at the other end of the link, and nothing more than that. A partner integration is not a Comfy product either: where a hosted service or a partner model sits behind a Comfy API, the API is Comfy's and the service is the partner's.

### Installing third-party projects

An entry is checked against [the bar](CONTRIBUTING.md) for fit, not audited for safety. Comfy Org does not certify that a listed project is safe, does not control, test or vet its code, models or data, and may review a listing but does not promise to keep reviewing it. Being on this list is not an endorsement.

Custom nodes and apps are executable code, not metadata. They run with the same access as the Comfy process that loads them, which on a local install is your own user account, your files and your network. Trust a pack as much as you would trust any other software you choose to install: read the source, check who publishes it, and accept that you are the one running it.

If an entry is malicious, misleading or harmful, [report it](https://github.com/Comfy-Org/awesome-comfy/issues/new?template=report-an-entry.yml). That form is how an entry comes off the list, and no timeframe is promised for it. Removing an entry does nothing to the project itself, which stays wherever its author put it.

## Built with Comfy

Products, tools and apps that run Comfy underneath.

### From the community

Made by other people. Read [Installing third-party projects](#installing-third-party-projects) before you run any of it.

**Tools that put Comfy inside something else:**

- [krita-ai-diffusion](https://github.com/Acly/krita-ai-diffusion) - Inpainting, outpainting and live painting inside Krita, against a local or remote Comfy server.
- [OpenLayer](https://mehran-ahmadi.com/OpenLayer/) - A Photoshop panel that generates, inpaints and upscales through your own Comfy server and hands back editable layers. Alpha.
- [StableGen](https://github.com/sakalond/StableGen) - A Blender addon that textures 3D meshes through a Comfy backend using multi-view projection.
- [ComfyUI-for-Nuke](https://github.com/vinavfx/ComfyUI-for-Nuke) - Builds and runs Comfy graphs inside Foundry Nuke, against your own Comfy server.
- [ComfyUI-TD](https://github.com/JiSenHua/ComfyUI-TD) - Streams images, video, point clouds and audio from Comfy into TouchDesigner in real time.
- [SwarmUI](https://github.com/mcmonkeyprojects/SwarmUI) - A forms-first front end over the same engine, with a Comfy workflow tab when you want the graph back.

**Apps on top of your own Comfy:**

- [ComfyTV](https://github.com/jtydhr88/ComfyTV) - Turns Comfy into a canvas app where each stage is its own node, across image, video, audio and 3D.
- [Velorn](https://velorn.ai) - An open-source desktop video workstation that runs any Comfy workflow on a timeline, locally or in the cloud. ([source](https://github.com/VelornLabs/velorn))
- [ComfyLink](https://comfylink.app) - An iOS and Android remote for your own Comfy machine, paired through a node you install in Comfy. ([the node](https://github.com/huijiutian/ComfyUI-ComfyLink))
- [ComfyUI Metadata Viewer](https://huggingface.co/spaces/QES/ComfyUI_Metadata_Viewer) - Drop a Comfy output file in the browser and read back the models, parameters and prompt embedded in it.

### From Comfy

**Apps you can open right now:**

- [Emojinius](https://emojinius.comfy.org) - Upload a character and get back a pack of animated Slack emojis. Needs your own Comfy API key; generation is billed to your account.
- [Cinematic Studio](https://comfy.org/hub/apps/cinematic-studio/) - Direct a shot with a real camera, light and grade it, then run it on any image model.
- [Openjutsu](https://comfy.org/hub/apps/openjutsu/) - Swap the main person in a 5 to 15 second clip for the character in one image, keeping the scene, motion and sound. Runs MiniMax H3; needs a Comfy sign-in, and runs are billed in credits.

**Clonable app guides**, a working app plus a walkthrough of how it is wired:

- [comfy-cinematic-studio](https://github.com/Comfy-Org/comfy-cinematic-studio) - Source and development guide for Cinematic Studio above.
- [comfy-reshoot](https://github.com/Comfy-Org/comfy-reshoot) - A workflow-deployment app, built to be cloned and changed.
- [comfy-openjutsu](https://github.com/Comfy-Org/comfy-openjutsu) - Source and development guide for Openjutsu above, run on your own Comfy deployment.

- [comfy-examples](https://github.com/Comfy-Org/comfy-examples) - Thirteen smaller apps, each a handful of files behind a deploy button: a Discord image bot, object removal, virtual try-on, sketch to image, profile shots and more.

## Work made with Comfy

Films, campaigns, games and public art. The work is the makers' own, and the credit belongs to the people and studios named in each line. Most of the links are write-ups published by Comfy, so the two headings used elsewhere in this list do not apply here.

**Galleries and roundups:**

- [Gallery](https://comfy.org/gallery/) - Community images, video and 3D, each credited to its maker. The fastest way to see the range.
- [Made with ComfyUI 2025](https://blog.comfy.org/p/made-with-comfyui-2025-from-open) - A year of work in one place, from open-source releases to brand campaigns.
- [Customer stories](https://comfy.org/customers/) - Studios, brands, artists and universities, with a [machine-readable index](https://comfy.org/customers/llms.txt).

**Film and television:**

- [The Song of Drifters](https://comfy.org/customers/xindi-zhang/) - Xindi Zhang built her USC thesis film in Comfy, using her own illustrations as the style guide ([in her own words](https://blog.comfy.org/p/the-tool-that-expands-my-art-xindi)). It won a Golden Award at the [Student Academy Awards](https://www.usf.edu/arts/news/2025/20251106-from-thesis-to-oscars-shortlist-xindi-zhang-ai-driven-film-wins.aspx).
- [YUI](https://comfy.org/customers/hakoniwa-yui/) - A 4:20 animated short by 852話 Hakoniwa, made in three days of focused work. ([longer write-up](https://blog.comfy.org/p/creating-the-story-of-yui-with-852))

**Advertising and campaigns:**

- [Svedka, Shake Your Bots Off](https://comfy.org/customers/svedka-silverside/) - Silverside AI rebuilt Svedka's lost Fembot on Comfy workflows for a Super Bowl LX spot.
- [Groove Jones, Dick's Sporting Goods](https://comfy.org/customers/groove-jones/) - A hyper-realistic faux out-of-home holiday campaign for the Crocs x NFL collection, delivered against a short deadline.
- [Don Diablo, Blackout](https://www.youtube.com/watch?v=cPMNIIZkNIs) - Music video whose image work, including identity modelling and stylization, was done locally in Comfy. ([write-up](https://blogs.nvidia.com/blog/rtx-ai-garage-don-diablo-gen-ai-music-video))

**Games:**

- [ComfyCrawler](https://mowmeow.net/ComfyCrawlerTest/) - A dungeon crawler in a Windows 95 interface, with its art and music generated in Comfy. The hosted build is a read-only edition.

**Studios and 3D:**

- [Series Entertainment](https://comfy.org/customers/series-entertainment/) - Over 100,000 assets across multiple Netflix titles, kept consistent by repeatable workflows. ([case study](https://blog.comfy.org/p/case-study-how-series-entertainment))
- [Ubisoft CHORD](https://comfy.org/customers/ubisoft-chord/) - Ubisoft La Forge open-sourced its PBR material estimation model with Comfy custom nodes. ([announcement](https://blog.comfy.org/p/ubisoft-open-sources-the-chord-model))

**Public art and installations:**

- [Moment Factory](https://comfy.org/customers/moment-factory/) - Rebuilt a 3D projection mapping pipeline for architectural-scale work. ([case study](https://blog.comfy.org/p/case-study-how-moment-factory-reimagined))
- [Ina Conradi's NTU students](https://comfy.org/customers/ina-conradi/) - Ninety-second films for building-sized LED walls, shown at Hangzhou's West Lake media facade.
- [Echoes of Time](https://blog.comfy.org/p/echoes-of-time-lighting-up-a-historic) - A projection piece on Niš Fortress, produced through a Comfy community challenge.

**Studios on their own pipelines**, recorded talks:

- [Reinventing the Production Pipeline](https://comfy.org/events/production-pipeline/) - Erin Sarofsky and Ryan Summers of Sarofsky on rebuilding a studio pipeline around Comfy.
- [Beyond the Models](https://comfy.org/events/beyond-the-models/) - Building custom workflows for commercial and film production.
- [The Future of AI Post Production](https://comfy.org/events/future-ai-post-production/) - Ingi Erlingsson on custom LoRAs and motion graphics nodes in post.
- [How Black Math built a hackathon in three weeks](https://comfy.org/events/black-math-hackathon/) - A design studio shipping an event-scale build.
- [Silverside AI](https://comfy.org/customers/videos/silverside-ai/) - Why node-based workflows give a creative team more control than single-prompt tools.
- [Black Math](https://comfy.org/customers/videos/black-math/) - Artists and technical directors on building extendable creative systems while keeping art direction.

**Teaching:**

- [Golan Levin, Carnegie Mellon](https://comfy.org/customers/golan-levin/) - "It's an image-processing workstation for completely new kinds of work."
- [Kathy Smith, USC](https://comfy.org/customers/kathy-smith/) - Inside the Expanded Animation MFA that built a curriculum around it.
- [UAL Creative Computing Institute](https://comfy.org/customers/ual-cci/) - A teaching and research partnership across masters, PhD and industry programmes.

**Events:**

- [Events](https://comfy.org/events/) - Livestreams, hackathons and meetups, upcoming and recorded, with a [machine-readable index](https://comfy.org/events.md).

## Workflows

### From Comfy

- [comfy.org/workflows](https://comfy.org/workflows) - Browsable catalogue of runnable workflows with the models each one needs, including walkthroughs for [character replacement](https://comfy.org/workflows/use-cases/ai-character-replacement/), [image to video](https://comfy.org/workflows/use-cases/ai-image-to-video/), [sprite sheets](https://comfy.org/workflows/use-cases/sprite-sheet-generator/), [photo restoration](https://comfy.org/workflows/use-cases/restore-old-photos/) and [image to 3D](https://comfy.org/workflows/use-cases/image-to-3d/).
- [workflow_templates](https://github.com/Comfy-Org/workflow_templates) - The source of the templates that ship inside Comfy. Open a pull request here to add one.
- [Using templates](https://docs.comfy.org/interface/features/template) - How the built-in template browser works.
- [Workflow JSON spec](https://docs.comfy.org/specs/workflow_json) - The on-disk format, for reading or writing workflows programmatically.
- [API workflow format](https://docs.comfy.org/development/api-development/workflow-api-format) - The flattened form you POST to a server.

## Build your own

The API surfaces, SDKs and hosted endpoints for driving Comfy from your own code.

### From Comfy

- [Development overview](https://docs.comfy.org/development/overview) - Map of the API surfaces and which one you want.
- [API quickstart](https://docs.comfy.org/development/api-development/quickstart) - Submit a workflow and collect the result in a few calls, once you have [an API key](https://docs.comfy.org/development/api-development/getting-an-api-key).

**Comfy Router**, one API in front of many hosted image, video and audio models:

- [Router quickstart](https://docs.comfy.org/development/comfy-router/quickstart) - One POST, no graph to build. The [API reference](https://docs.comfy.org/development/comfy-router/api) covers run, queue, poll and cancel.
- [Model catalogue](https://docs.comfy.org/development/comfy-router/models) - Every model it can run, with per-model input and output schemas.
- [Pricing](https://docs.comfy.org/development/comfy-router/pricing) - Per-model cost, which you want before you build on it.

**Developer Platform**, for running your own workflows as a service:

- [Cloud API overview](https://docs.comfy.org/development/cloud/overview) - Assets, jobs, queue and history against hosted Comfy.
- [Serverless overview](https://docs.comfy.org/development/serverless/overview) - Turn a workflow into an endpoint you can call.

**SDKs**, which [cover the same ground in the same shape](https://docs.comfy.org/development/api-development/sdks):
- [Python SDK](https://github.com/Comfy-Org/comfy-python-sdk) - Client for self-hosted Comfy and Comfy Cloud.
- [TypeScript SDK](https://github.com/Comfy-Org/comfy-typescript-sdk) - Node client for the Comfy API v2, against Comfy Cloud, serverless or a self-hosted proxy.
- [Swift SDK](https://github.com/Comfy-Org/comfy-swift-sdk) - Thin client: submit, stream, collect outputs.

**Comfy MCP:**

- [Comfy MCP](https://comfy.org/mcp) - The hosted endpoint and what it can do.
- [comfy-mcp](https://github.com/Comfy-Org/comfy-mcp) - Exposes a local Comfy over the Model Context Protocol.
- [MCP documentation](https://docs.comfy.org/agent-tools/mcp) - Setup and the tools the server exposes.

**Talking to a Comfy server directly:**

- [Server API overview](https://docs.comfy.org/development/comfyui-server/comms_overview) - The REST and WebSocket model the editor itself uses, with a [reference for every route](https://docs.comfy.org/development/comfyui-server/comms_routes) and [working scripts](https://docs.comfy.org/development/comfyui-server/api-examples) for queueing prompts and reading results.
- [comfy-api-proxy](https://github.com/Comfy-Org/comfy-api-proxy) - Puts the v2 API in front of a self-hosted instance, so one client works against both.

### From the community

Read the third-party note above before you run any of it.

**Writing workflows as code:**

- [ComfyScript](https://github.com/Chaoses-Ib/ComfyScript) - Write workflows as Python instead of JSON.
- [ComfyUI-to-Python-Extension](https://github.com/pydn/ComfyUI-to-Python-Extension) - Exports a saved workflow as a standalone Python script.

## Node packs

Custom nodes are how Comfy grows. This list does not rank them: install counts move every day and the registry publishes them live, so a curated twenty here would only ever be a stale copy of a better table. Anything you install through either entry below is third-party code that runs inside your Comfy process, so read the third-party note above first.

**Find and install them with:**

- [ComfyUI-Manager](https://github.com/Comfy-Org/ComfyUI-Manager) - Installs, updates, disables and security-scans node packs from inside the editor. Most people's entry point.
- [Comfy Registry](https://registry.comfy.org/) - The package index, searchable and ranked by install count. Start here rather than with a clone URL someone pasted in a comment.
- [Registry overview](https://docs.comfy.org/registry/overview) - What the registry is, how versions and publishers work.
- [Publishing to the registry](https://docs.comfy.org/registry/publishing) - For node authors shipping a pack, with the [standards](https://docs.comfy.org/registry/standards) a pack is expected to follow and [CI/CD](https://docs.comfy.org/registry/cicd) for publishing on tag.
- [Installing custom nodes](https://docs.comfy.org/installation/install_custom_node) - The manual route, and what it writes to disk.
- [Custom node troubleshooting](https://docs.comfy.org/troubleshooting/custom-node-issues) - Import errors, dependency conflicts and how to bisect them.

## Writing your own nodes

### From Comfy

- [Custom node overview](https://docs.comfy.org/custom-nodes/overview) - Start here if you are writing your first node.
- [Walkthrough](https://docs.comfy.org/custom-nodes/walkthrough) - Builds a working node from an empty folder.
- [Server-side reference](https://docs.comfy.org/custom-nodes/backend/server_overview) - `INPUT_TYPES`, `RETURN_TYPES`, `FUNCTION`, lifecycle and the rest of the contract.
- [Datatypes](https://docs.comfy.org/custom-nodes/backend/datatypes) - The type system that decides which sockets connect.
- [Shipping templates with a pack](https://docs.comfy.org/custom-nodes/workflow_templates) - So users get an example workflow on install.
- [ComfyUI_frontend](https://github.com/Comfy-Org/ComfyUI_frontend) - The Vue front end the editor runs on.
- [comfyui-native-port-guide](https://github.com/Comfy-Org/comfyui-native-port-guide) - Conventions for adding native model support to core, rather than wrapping it in a pack.
- [embedded-docs](https://github.com/Comfy-Org/embedded-docs) - The help pages shown inside the editor for core nodes, and how to add yours.
- [comfy-model-tools](https://github.com/Comfy-Org/comfy-model-tools) - Scripts for merging, converting and quantizing model files for Comfy.
- [comfyui-benchmark](https://github.com/Comfy-Org/comfyui-benchmark) - Extension for measuring generation performance across configurations.

## Hosting

### From Comfy

- [Self-hosting guide](https://docs.comfy.org/development/deploy/self-hosting) - Running Comfy on a rented GPU.

### From the community

Independent providers and images. Comfy Org does not operate these services, hold your data on them, or set their prices. Read the third-party note above first.

- [ComfyUI-Docker](https://github.com/YanWenKun/ComfyUI-Docker) - Container images across several CUDA and Python combinations.
- [SaladCloud](https://docs.salad.com/container-engine/how-to-guides/ai-machine-learning/deploy-stable-diffusion-comfy) - Deploy image and video generation with ComfyUI on their container engine.
- [comfyui-api](https://github.com/SaladTechnologies/comfyui-api) - A stateless API server in front of Comfy that returns images or sends them to webhooks and S3, built for horizontal scaling.

## Getting started

### From Comfy

- [ComfyUI](https://github.com/Comfy-Org/ComfyUI) - The node-graph engine itself: a workflow runner for diffusion models with a Python backend.
- [Download page](https://comfy.org/download) - Picks the right install path for your machine. Check the [system requirements](https://docs.comfy.org/installation/system_requirements) first.
- [Desktop app](https://docs.comfy.org/installation/desktop/overview) - Packaged installer for Windows, macOS and Linux. The shortest path to a working setup.
- [Comfy Desktop source](https://github.com/Comfy-Org/Comfy-Desktop) - The official desktop app: installs and manages multiple Comfy setups side by side.
- [Manual install](https://docs.comfy.org/installation/manual_install) - Clone and pip, for when you want to control the Python environment. Windows also has a [portable build](https://docs.comfy.org/installation/comfyui_portable_windows): one folder, no installer, no system Python.
- [Your first generation](https://docs.comfy.org/get_started/first_generation) - Walks a default workflow end to end and explains what each node did. The [interface tour](https://docs.comfy.org/interface/overview) covers the canvas, the queue and the model library.
- [Comfy Cloud](https://docs.comfy.org/get_started/cloud) - Hosted Comfy, for when you do not have the GPU.
- [comfy-cli](https://github.com/Comfy-Org/comfy-cli) - Command-line installer and manager for Comfy, models and node packs. [Its docs](https://docs.comfy.org/comfy-cli/getting-started) cover launching, snapshots and switching versions.
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

- [Nerdy Rodent](https://www.youtube.com/@NerdyRodent) - Regular walkthroughs of new models and workflows.
