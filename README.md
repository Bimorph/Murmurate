# Murmurate

**Grasshopper definitions as AI tools.**

Murmurate wraps an existing Grasshopper definition, publishes it as a named tool, and makes it
callable by an AI assistant. The agent is not handed a blank canvas. It is handed a deterministic
tool which will perform the desired logic every time.

**[Find out more at bimorph.com/products/murmurate →](https://www.bimorph.com/products/murmurate)**

> This repository hosts Murmurate's releases. The source code is not published here.

---

## Download

**[Download the latest release](https://github.com/Bimorph/Murmurate/releases/latest)**

> [!WARNING]
> **Murmurate is a beta release and is not for production use.** It is still under active
> development, so expect bugs, rough edges and changes between releases. Tools published with a
> beta version may need republishing after a later update. Use it for evaluation and testing, not on
> live projects, and keep copies of your Grasshopper definitions. Please report anything that goes
> wrong to [support@bimorph.com](mailto:support@bimorph.com).

## How it works

No configuration file, terminal, API key or code. Murmurate takes the definitions that already hold
your logic and adds a name, a description, typed inputs and a place to publish.

1. **Build.** Wrap the logic in an AI tool component and describe its inputs and outputs. The inner
   canvas works exactly like a native cluster.
2. **Publish.** One click writes the tool to the library as a single self-contained file. The
   definition travels inside it, ready to version or send.
3. **Connect.** Point an AI assistant at Rhino once. Every tool published from then on appears in
   the assistant automatically, with no restart.

A prompt goes in and geometry comes back. The geometry is baked into the Rhino model, placed on the
canvas or passed into the next tool.

There is more on the [product page](https://www.bimorph.com/products/murmurate). Our article on
[self-describing clusters](https://www.bimorph.com/insights/grasshopper-ai-self-describing-clusters)
explains why Murmurate works this way.

## Requirements

- Rhino 8 or Rhino 9
- Windows
- Claude Desktop, Claude Code, or any other client that speaks the Model Context Protocol
- Node.js 18 or later, for Claude Code and Codex only

## Install

1. Close Rhino.
2. Download `Murmurate-<version>.msi` from the
   [latest release](https://github.com/Bimorph/Murmurate/releases/latest) and run it. It installs
   for the current user only, needs no administrator rights, and covers Rhino 8 and Rhino 9.
3. Start Rhino. Murmurate loads at startup.
4. Run **`AIToolsMurmurateServer`** in Rhino and follow its **Setup** tab to connect your AI
   client. It has the exact steps for Claude Desktop, Claude Code, Codex and other clients.

To upgrade, run the newer installer. To uninstall, use **Settings → Apps** in Windows.

## First tool

1. In Grasshopper, open the **Murmurate AI Tools** tab and place an **AI Tool** on the canvas.
2. Double-click it and build your definition inside. Add an **AI Tool Input** for each value it
   takes and an **AI Tool Output** for each result. Give each a clear name and description, because
   the assistant reads them to understand the tool.
3. Right-click the component and choose **Publish to AI Tools Library**.
4. Ask your assistant to do the job.

## Support

To report an issue or ask a question, email
**[support@bimorph.com](mailto:support@bimorph.com)**.

## Automate your team's definitions

Have a library of definitions worth automating? Tell us what your team runs by hand and see what an
assistant could run instead.
**[Book a discovery call →](https://www.bimorph.com/contact)**

## Licence

Murmurate is free to use under the End User Licence Agreement shown by the installer. Third-party
components and their licences are listed in `THIRD-PARTY-NOTICES.txt`, which is installed with the
plug-in. Bimorph's [privacy policy](https://www.bimorph.com/policy/privacy-policy) applies to
support email.

© Bimorph · [bimorph.com](https://www.bimorph.com) ·
[LinkedIn](https://www.linkedin.com/company/bimorph-bim/) ·
[YouTube](https://www.youtube.com/@BimorphUK)
