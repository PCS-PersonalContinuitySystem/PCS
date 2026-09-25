# PCS — Personal Continuity System

**Room to think. Space to connect.**

PCS is a Windows AI companion for conversation, learning, reading, and everyday plans—with memory you can inspect and revise. Talk ideas through at your own pace and carry useful context forward in your own encrypted vault. The supported AI provider can change; your saved vault stays with you.

**[Download PCS 0.9.10 for Windows][windows]** · [Release notes][release] · [Website][website] · [Report an issue][issues]

> **Current public version: 0.9.10 — pre-release.** PCS is free, with no PCS subscription or locked features. Cloud features use your own API keys and may incur provider charges. The supported Local route uses your hardware and requires separate model/runtime downloads.

## What you can do

| Area | What it offers |
| --- | --- |
| **Conversation** | Talk or type with Google, OpenAI, or the supported Local model. On supported cloud routes, enable visual context from an OBS scene you choose. OBS is a separate download, not bundled with PCS. |
| **Continuity: Map & Library** | Explore recurring themes in Map, or search memories and notebooks in Library. Inspect original sources, corrections, revision history, and recorded authorship. Follow related records and review a **Continue this thought** draft before sending it. |
| **Materials** | Browse **Documents**, **Notebooks**, and **Reference notes**. Read original files locally, review preparation requests, gather sources into notebooks, and return to saved reading or research notes. |
| **Calendar** | Manage tasks, goals, and events in Month or Agenda view. Use month arrows, Today, date selection, and a day panel. Choose separately whether—and how—PCS may assist with your plans. |
| **Learning & research** | Organize questions and learning steps, use practice activities, and request research on supported cloud routes. Keep source material and model suggestions distinct from your own notes. |
| **Backup & restore** | Save and check encrypted vault backups, restore into an empty installation, or enable automatic encrypted backups while PCS is open and eligible. Original Materials files need a separate copy. |

**You can browse saved records, use manual Calendar, and read Materials locally without starting an AI conversation.** Model-assisted recall, preparation, and other AI features have their own sharing and availability controls.

### Memory you can examine, not just trust

Saved memories are interpretations, not guaranteed facts. Inspect their sources and recorded writer, make corrections, and review earlier revisions.

Map browsing is **local and read-only**, with no model or embedding request. Links show labels appearing in shared records—not causation or agreement. Dates mean last saved or edited, not past beliefs. Library provides paginated access to records beyond the Map’s bounded sample.

## Download and start

| Download | Choose this for |
| --- | --- |
| **[PCS-0.9.10-Windows-x64.zip][windows]** | The complete Windows application, including launchers, portable Python, pinned dependencies, offline English speech recognition, source, and Help. |
| [PCS-0.9.10-Source.zip][source] | Matching development source, tests, documentation, speech assets, and launcher source/build instructions. Not a ready-to-run Windows package. |
| [PCS-0.9.10-SHA256SUMS.txt][checksums] | SHA-256 checksums for verifying the Windows and source downloads. |

Most users need only the **Windows ZIP**. Use the named release assets, **not GitHub’s automatically generated “Source code (zip)”**. The Local conversation model and its runtime are separate from the Windows package.

### First-time setup

1. Download and verify the Windows ZIP, then **extract the complete archive into a writable folder**. Keep all its files together; do not run it inside an archive viewer or overlay an older installation.
2. Run **Start PCS.exe**. First launch prepares its bundled Python environment offline and opens the interface locally in your desktop browser. You do not need to install system Python.
3. **Create a vault** with a long, unique passphrase and keep it safe. PCS cannot recover a forgotten passphrase. Existing users should follow [Updating](#updating) rather than create another vault.
4. Open **Settings → Connection**, choose and configure your route, review memory and sharing choices, and save. Return to Conversation and choose **Start PCS**. Begin with a short typed message; select **Use microphone** before Start to use voice.

**Cloud: Google or OpenAI.** Bring your own API key and review billing, limits, and optional Memory/Preparation provider overrides. [OpenAI API usage is separate from a ChatGPT subscription][openai-billing]. Help explains feature differences, including Google free-route restrictions.

**Local: compatible Windows/NVIDIA hardware.** Use the supported model, runtime, and CUDA-library downloads identified in Settings and Help—not arbitrary substitutes. Local conversation has no API-key requirement or cloud fallback. Optional English voice uses bundled recognition and a supported installed Windows desktop voice. Local vision and network research are unavailable.

Local listening pauses during processing and replies. A warning occurs around **22 seconds**; at **30 seconds**, PCS processes the captured recording instead of discarding it. Cutoff turns cannot directly perform Calendar, notebook, Remember, or practice writes; finish the request in a new turn.

The full launch address contains an access token. **Keep it private**, including in screenshots and bug reports.

## Your information and your choices

**Local storage does not mean every AI request stays local.** Cloud features send selected content to configured providers, including permitted memories, passages, document portions, Calendar details, or screenshots. Review sharing choices and provider terms.

**Don’t save this conversation** pauses new PCS saving, not cloud-provider receipt. **Clear chat** and hiding the memory stream affect the display; neither deletes saved continuity.

Original **Materials files and readable exports are outside vault encryption**. Enabled OBS sharing can capture a visible memory inspector or document. A requested or queued save is not confirmation of completion—check the saved outcome.

## Updating

A fresh extraction does **not** automatically find your older data. Keep the old installation and backup until the new copy is verified. Choose **one** transfer method.

### Guided method: built-in backup and restore

1. Save edits and stop conversation/background work, leaving the vault unlocked. Choose **Backup & restore → Save current backup…** and save outside the installation. After confirmation, choose **Quit PCS** and wait for **PCS closed**.
2. Extract the new Windows ZIP into a fresh folder and run **Start PCS.exe**. Choose **Restore an encrypted backup instead**—do not create a new vault.
3. Select your `.pcs` backup, enter its passphrase, and choose **Check backup**. Review the counts, choose **Restore this backup**, then **Unlock existing**. Check your records and settings.
4. Copy the original files from the old **data/Materials** folder into the new **data/Materials** folder, preserving filenames, contents, and relative subfolders. With the vault unlocked and conversation stopped, choose **Materials → Refresh documents**.

**Vault backups include saved records, prepared notes, and saved settings/credentials—not original Materials files.** The in-app limit is **256 MiB**; larger vaults need the complete-folder method.

<details>
<summary><strong>Alternative: transfer the complete data folder</strong></summary>

With PCS fully quit, back up the entire old **data** folder, then copy it beside **Start PCS.exe** in a fresh extraction **before starting it**. Do not move your only copy or merge separate data folders.

Launch, **Unlock existing**, verify records, and refresh Materials while stopped. This transfers the vault and original Materials together; the originals remain unencrypted. For custom data locations, use the directory your launcher actually uses.

</details>

After either method, re-select your automatic-backup destination and update old shortcuts as needed. **Never run two instances against the same data directory simultaneously.** For custom paths or uncertain shutdowns, preserve recovery files and follow the downloaded `docs/RESTORE_VAULT.md`.

**0.9.10 introduces no vault-format migration.** Backups restore their saved state; they do not merge changes from another copy or resume a running conversation.

## New in 0.9.10

**Smoother OpenAI allowance handling:** a preventive wait can hold one never-sent answer for up to two minutes and request it once when permitted. Stop, Lock, **Cancel waiting answer**, newer input, or changed permissions can retire it. Failed/cancelled requests and completed actions are not automatically replayed. Usage labels separate conversation, memory, and indexing work.

**Documents-first Materials:** related actions sit together, notebook-source selection has independent search/paging, and refresh clears obsolete passage results. The Map/Library consolidation, Calendar navigation, and Local speech improvements from intervening builds are retained. [Read the release notes][release].

## Help and limitations

Open **Help** inside PCS, or open **`docs/HELP.html`** from the extracted package for searchable offline guidance. Other guides included in the Windows and source downloads are:

| Guide | File inside the download |
| --- | --- |
| Quick start and full setup | `START_HERE.md` and `docs/GETTING_STARTED.md` |
| Backup, restore, and folder transfers | `docs/RESTORE_VAULT.md` |
| Map controls and evidence boundaries | `docs/CONTINUITY_MAP.md` |
| Current changes and validation | `docs/RELEASE_NOTES.md` and `docs/developer/AUDIT_0.9.10.md` |
| Windows checks and development | `docs/developer/ACCEPTANCE_0.9.10.md` and `docs/developer/README.md` |

These paths are **inside the release packages**, not this repository. Use bundled Help for the exact controls in your version; the [website][website] provides an overview.

PCS remains a **pre-release**. Transcription, vision, memory, and recall can be wrong or incomplete. Google renewal failures and provider limits remain known concerns. OpenAI’s short-audio filtering is not guaranteed cough detection, and pending answers can expire. Local compatibility and performance depend on the supported configuration and other workloads.

Calendar does not synchronize Google/Outlook accounts, book appointments, invite attendees, or deliver reminders. Linking or preparing part of a document does not mean the whole document has been read. Practice assessments are provisional.

The 0.9.10 audit records passing automated checks with disclosed skips/exclusions—not complete Windows hardware, live-provider, or long-session acceptance. Passing tests do not prove freedom from defects.

**Stop PCS** ends conversation; **Lock** also closes vault access; **Quit PCS** shuts down the host. Closing the tab alone can leave it running and unlocked. Keep package files together: the launcher checks their manifest.

## Feedback and support

Use [GitHub Issues][issues] for bugs and feedback. Include the version/build, provider route, expected and actual behavior, and reproduction steps. Export **Bug report before quitting** when possible and review it before sharing; reports are not uploaded automatically. Never post keys, passphrases, full launch URLs, private vaults, or personal conversations.

**PCS is free and does not require payment.** Optional one-time contributions support development. There is no PCS subscription, and no features are locked behind payment. AI-provider charges are separate.

[![Support PCS on Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)][kofi]

## Source and development

This repository hosts releases, documentation, and issues. **The complete application source is attached to each release**, not supplied by cloning this repository or GitHub’s automatic source archive.

Download **[PCS-0.9.10-Source.zip][source]** and follow its `SOURCE_README.md` and `docs/developer/README.md`. The Windows ZIP also contains source, plus the pinned Python runtime, offline wheelhouse, and compiled launchers omitted from the source-only package. Develop and test with synthetic data, not a personal vault.

## License

Copyright (C) 2026 Courtney Dickson.

First-party PCS code is licensed under **GNU GPL version 3 only (GPL-3.0-only)**. See [LICENSE](LICENSE) and [COPYRIGHT](COPYRIGHT). PCS is provided without warranty. Separately identified third-party components retain their own licenses; see [THIRD_PARTY.md](THIRD_PARTY.md) and the notices in each download.

[windows]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.10/PCS-0.9.10-Windows-x64.zip
[source]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.10/PCS-0.9.10-Source.zip
[checksums]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.10/PCS-0.9.10-SHA256SUMS.txt
[release]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/tag/v0.9.10
[website]: https://pcs-personalcontinuitysystem.github.io/PCS-site/
[issues]: https://github.com/PCS-PersonalContinuitySystem/PCS/issues
[kofi]: https://ko-fi.com/pcssupport
[openai-billing]: https://help.openai.com/en/articles/9039756-managing-billing-for-chatgpt-and-the-api-platform
