# PCS — Personal Continuity System

**A Windows AI companion with memory you can inspect and revise.**

Talk ideas through, learn at your own pace, and keep useful context in your own encrypted vault. The AI provider can change; your PCS vault stays with you.

**[Download PCS 0.9.6 for Windows][windows]** · [Website][website] · [Getting started][getting-started] · [Release notes][release]

**Current public release: 0.9.6 — pre-release.** PCS is free, with no PCS subscription or locked features. Cloud routes use your own API keys and may incur provider charges. The supported Local route needs compatible hardware and separate model/runtime downloads.

## Downloads

| File | Choose this for |
| --- | --- |
| **[PCS-0.9.6-Windows-x64.zip][windows]** | The complete Windows application. Includes the launchers, Python, pinned dependencies, PCS source, offline English speech recognition, and Help. |
| [PCS-0.9.6-Source.zip][source] | Matching editable source, tests, launcher source/build instructions, documentation, speech assets, and notices. |
| [PCS-0.9.6-SHA256SUMS.txt][checksums] | SHA-256 checksums for the Windows and source ZIPs. |

Most users only need the **Windows ZIP**. The Local conversation model and its native runtime are separate downloads. Use the files attached to the release, not GitHub’s automatically generated **Source code (zip)**; see [Source and development](#source-and-development).

## What PCS can do

| Area | What you can use it for |
| --- | --- |
| **Conversation** | Talk or type with Google, OpenAI, or the supported Local model. Use optional screen context through a separately installed OBS setup on supported cloud routes. |
| **Saved continuity** | Inspect memories, linked original sources, corrections, revision history, and the revision writer recorded by PCS. Requested saves can create or revise a memory, save a verbatim note, or ask for clarification. |
| **Continuity Map v2** | Explore recurring wording and saved topic labels across current memories and notebooks. Search, filter, pin themes, compare saved-date windows, and inspect paths and their supporting records. |
| **Reading and learning** | Work with Materials, prepared reading notes, topic notebooks, and practice. Keep model suggestions distinct from your own notes, with research available on supported cloud routes. |
| **Local plans** | Organize tasks, goals, and events in Calendar, with separate controls for AI assistance. |

### Explore the evidence, not just the summary

![PCS 0.9.6 Continuity Map v2 showing themes and shared-record connections with synthetic example data][map-image]

*PCS 0.9.6 — actual Map interface rendered with synthetic example data. This illustrates the controls, not a live model result or a demonstration of memory accuracy.*

Map is **local and read-only**: browsing it makes no model or embedding requests and creates no persisted graph database. A line means labels occur in shared saved records; a path is a chain of those links, not a causal or psychological judgment. Dates mean **last saved or edited**, not when an idea was last discussed. The view uses a bounded sample of current records, not a reconstruction of past beliefs or deleted memories. [Read the Map v2 guide][map-guide].

<details>
<summary>See how PCS separates the recorded writer from editable memory content</summary>

![PCS 0.9.6 inspector separating the host-recorded revision writer from a conflicting authorship field in synthetic memory JSON][writer-image]

*The provider claim inside this synthetic payload is deliberately incorrect. “Revision writer · recorded by PCS” is stored separately; a model-authored JSON field cannot override it. Existing payloads are not silently rewritten. Correct attribution does not guarantee a correct memory.*

</details>

## Start on Windows

1. **Download and extract the entire Windows ZIP** into a fresh, writable folder. Keep its files together; do not run it inside an archive viewer or overlay an older installation.
2. Run **Start PCS.exe**. First-launch setup prepares the bundled Python runtime and dependencies, then opens PCS locally in your browser. System Python does not need to be installed separately.
3. **Create a vault** with a long, unique passphrase and keep it safe. PCS cannot recover a forgotten passphrase. For an existing encrypted backup, follow `docs/RESTORE_VAULT.md` instead.
4. Open **Settings → Connection**, choose your route, review memory and sharing permissions, and save. Start with a short typed conversation; enable the microphone after checking the browser’s permission and input controls.

**Google or OpenAI:** supply your own provider API key and check the provider’s billing and limits. [OpenAI API usage is billed separately from a ChatGPT subscription][openai-billing].

**Local:** use the supported model and matching runtime/CUDA libraries identified in Settings and Help. This route requires compatible Windows/NVIDIA hardware; it is not an arbitrary-model loader or a general hardware compatibility promise. Once set up, Local conversation uses no API key or cloud fallback. Local vision and network research are unavailable.

The launch URL includes an access token. **Do not share the full address**, including in screenshots.

[Full setup guide][getting-started] · [Memory controls][memory-guide] · [Data and privacy][privacy-guide]

## Your information and your choices

Saved continuity is stored in a **local encrypted vault**. That describes storage, not where every AI request runs. Cloud conversation and enabled features send selected content to configured providers, including permitted memories, original passages, document portions, or screenshots. Review both the conversation provider and optional Memory/Preparation provider overrides.

**“Don’t save this conversation” controls PCS saving; it does not stop a cloud provider receiving the conversation.** Clear chat clears the display, and hiding the memory stream only hides that panel. Neither action deletes saved continuity.

Original **Materials files and readable exports are outside vault encryption**. Encrypted backups do not include those original Materials; keep separate copies. Already-enabled screen sharing can capture a visible Map or memory inspector.

A requested save or a queued notice is not proof that a write finished. Inspect the saved outcome and its sources before relying on it.

## Updating and finding Help

Use **Quit PCS** and wait for shutdown. Preserve your passphrase, the old installation, and the **entire cleanly stopped data directory**, including Materials. Extract the new version into a fresh folder. With both copies stopped, copy that data directory beside the new `Start PCS.exe` without merging it into another existing vault. Encrypted-backup restore into an empty destination is an alternative; copy Materials separately.

**Never run two installations against the same data directory.** After an uncertain shutdown, preserve recovery/journal files and follow `docs/RESTORE_VAULT.md` rather than deleting them. No vault-format migration is required for 0.9.6.

The top-level `START_HERE.md` is the short entry point. Full guidance is in `docs/GETTING_STARTED.md`, `docs/RESTORE_VAULT.md`, and `docs/CONTINUITY_MAP.md`. **`docs/HELP.html` provides the same searchable Help and FAQ offline without starting PCS**, including local example pictures. Developer references and historical notes are grouped under `docs/developer` and `docs/history`. These paths are inside the downloaded application/source packages.

Do not manually reorganize the installed files: the launcher verifies the package manifest. **Stop PCS** ends the conversation; **Lock** also closes vault access; **Quit PCS** shuts down the host. Closing the browser tab can leave the host running and the vault unlocked.

## Changes since 0.9.0 Hotfix 1

The cumulative update adds Map v2, context-aware memory requests and corrections, clearer writer attribution, and refreshed Help. Targeted repairs address Local helper isolation, recall coordination, stuck listening states, background audio, transcript saving during cancellation, and browser cleanup. OpenAI gains bounded screenshot history, improved allowance estimates, and clearer pauses that preserve drafts without automatically replaying rejected requests.

Version 0.9.6 itself tidies documentation folders and updates Help/FAQ; it does not introduce another provider or memory-engine repair. See the [cumulative release notes][release] for details.

## Current limitations

PCS remains a **pre-release**, not a certified stable release. Google checkpoint-renewal failures, provider rate limits, and some memory-generation/reference failures remain open. Formation, transcription, and recall can be incomplete or wrong; saving a fact does not guarantee it will be retrieved or used correctly in every reply.

Local listening pauses while PCS processes and speaks. OpenAI may pause input for rate allowance; wait for the notice to clear, then deliberately speak or send again. These controls do not raise provider limits or eliminate browser/OS suspension.

Calendar is local: it does not synchronize Google/Outlook accounts, invite attendees, book appointments, or deliver reminders. Linking a document does not mean its entire contents have been read. Practice assessments are provisional.

The automated suite is **not fully green**, and complete Windows hardware, noisy-room, and long-session acceptance remain outstanding. The download includes the detailed audit and acceptance checklist under `docs/developer`.

## Feedback and support

Use [Issues][issues] for bugs or first-use feedback. Include the PCS version/build, provider route, what you expected, what happened, and steps to reproduce. Export and review the in-app **Bug report** before sharing it; reports are not uploaded automatically. Never include API keys, vault passphrases, complete launch URLs, private vaults, or personal conversations in a public report.

[Support PCS on Ko-fi][kofi] — optional, one-time contributions. PCS does not require payment, and no features are locked behind a PCS subscription. AI-provider charges are separate from supporting PCS.

## Source and development

**This repository is the download, documentation, and issue-tracking home. The complete application source is attached to each release.** Cloning this repository or downloading GitHub’s automatic source archive does not supply the complete application.

Use **[PCS-0.9.6-Source.zip][source]** for the source matching this release. It includes Python/browser code, tests, speech assets, documentation, and launcher source/build instructions. Follow `SOURCE_README.md` and `docs/developer/README.md` in the source package. The complete Windows ZIP also contains PCS source and supplies the pinned portable Python runtime, offline wheelhouse, and compiled launchers omitted from the reduced source archive.

## License

Copyright (C) 2026 Courtney Dickson.

First-party PCS code is licensed under the **GNU General Public License, version 3 only (GPL-3.0-only)**. See [LICENSE](LICENSE) and [COPYRIGHT](COPYRIGHT). PCS is provided without warranty. Separately identified third-party components retain their own licenses; see [THIRD_PARTY.md](THIRD_PARTY.md) and the notices included in each download.

[windows]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.6/PCS-0.9.6-Windows-x64.zip
[source]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.6/PCS-0.9.6-Source.zip
[checksums]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.6/PCS-0.9.6-SHA256SUMS.txt
[release]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/tag/v0.9.6
[website]: https://pcs-personalcontinuitysystem.github.io/PCS-site/
[getting-started]: https://pcs-personalcontinuitysystem.github.io/PCS-site/getting-started.html
[memory-guide]: https://pcs-personalcontinuitysystem.github.io/PCS-site/memory-control.html
[privacy-guide]: https://pcs-personalcontinuitysystem.github.io/PCS-site/data-and-privacy.html
[map-guide]: https://pcs-personalcontinuitysystem.github.io/PCS-site/continuity-map.html
[map-image]: https://raw.githubusercontent.com/PCS-PersonalContinuitySystem/PCS-site/main/screenshots/06-map-v2-096.webp
[writer-image]: https://raw.githubusercontent.com/PCS-PersonalContinuitySystem/PCS-site/main/screenshots/08-writer-096.webp
[issues]: https://github.com/PCS-PersonalContinuitySystem/PCS/issues
[kofi]: https://ko-fi.com/pcssupport
[openai-billing]: https://help.openai.com/en/articles/9039756
