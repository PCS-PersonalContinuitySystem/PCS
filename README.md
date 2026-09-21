# PCS — Personal Continuity System

PCS is a Windows desktop companion for conversation, revisable memory, notes, reading, and local plans.

[PCS website](https://pcs-personalcontinuitysystem.github.io/PCS-site/) · [Releases](https://github.com/PCS-PersonalContinuitySystem/PCS/releases)

## Downloads and source

This is the PCS application download repository. Each release supplies:

- **PCS-0.9.0-Windows-x64.zip** — the complete portable Windows application, including ordinary Python, dependencies, PCS source, and offline English speech recognition.
- **PCS-0.9.0-Source.zip** — matching editable PCS source, tests, launcher source/build recipe, and pinned speech assets/notices.
- **SHA256SUMS.txt** — SHA-256 checksums for both downloads.

Use the explicitly attached **Source.zip** for the application source. GitHub's automatically generated source archives contain this download repository's documentation.

Extract the complete Windows ZIP into a fresh folder and run **Start PCS.exe**. Do not overlay it on an older installation. Keep an encrypted vault backup when upgrading. The Local conversation model and its matching runtime are separate downloads; see the included setup guide. Cloud routes require your own provider configuration and may incur provider charges.

PCS is under active development. Read each release's known limits and verification notes before adopting it.

## Building and changing PCS

The source archive includes `README.md`, `pyproject.toml`, Python and browser code, tests, and `support/build-launchers.ps1` with its C# source. Follow the developer guide in that archive for ordinary Python development. The complete Windows archive supplies the pinned offline wheelhouse and runtime used for the portable package.

## License

Copyright (C) 2026 Courtney Dickson.

First-party PCS code is licensed under the **GNU General Public License, version 3 only (GPL-3.0-only)**. See [LICENSE](LICENSE) and [COPYRIGHT](COPYRIGHT). PCS is provided without warranty. Separately identified third-party components retain their own licenses; see [THIRD_PARTY.md](THIRD_PARTY.md) and the notices included in each download.
