# PCS — Personal Continuity System

**Room to think. Space to connect.**

PCS is a Windows AI companion for conversation, learning, reading, and everyday plans—with continuity you can inspect and revise. Talk an idea through, work through a book, return to a project, or explore a question together. Keep useful context in your own encrypted vault and choose the supported AI connection that suits you.

**[Download PCS 0.9.24 for Windows][windows]** · [Release notes][release] · [Website][website] · [Discord][discord] · [Report an issue][issues]

> **0.9.24 · Pre-release · Windows x64**  
> Free, with no PCS subscription or locked features. Cloud providers may charge for API usage. Local AI uses your hardware and separately downloaded components.

## Follow the connections in your thinking

[![Detailed synthetic example of the PCS Continuity Map, with connected themes and supporting records. Click to visit the PCS website.](assets/pcs-thought-map-sample.jpg)][website]

*30 themes, 89 connections, and 96 fictional saved records in the PCS 0.9.24 interface. Click the picture to visit the website, or [open the full-size image](assets/pcs-thought-map-sample.jpg).*

The **Continuity Map** helps you explore recurring wording and topics across saved memories and notebooks. Select a theme to inspect its supporting records, follow connections, or compare saved-date windows. In **Library**, review a **Continue this thought** draft before placing it in a conversation.

Drag nodes into a useful arrangement and keep their positions in your encrypted vault. Switch between **Connections**, **By group**, and **Circle**, pin themes, or use the accessible List view. Browsing the Map needs no running AI conversation.

Connections show themes appearing together in supporting records. The view covers a bounded sample of current saved records; it does not reveal an AI's internal thoughts or establish causes, agreement, or a psychological profile.

## What you can do

| Workspace | Make it useful to you |
| --- | --- |
| **Conversation** | Talk or type using Google, OpenAI, or Local AI. Customize the companion's directions and optionally share an OBS scene on supported routes. |
| **Continuity** | Inspect memories, source evidence, and revision history. Correct interpretations, remove records with a reviewed scope, and explore connections in Library and Map. |
| **Materials** | Bring TXT, Markdown, selectable-text PDF, or EPUB documents. Consult passages, prepare reading notes, organize notebooks, and retain supported web sources. |
| **Research and Practice** | Explore questions, retain Wikipedia study notes, and work through lessons and exercises. Keep original sources, model explanations, and your own notes distinguishable. |
| **Calendar** | Manage tasks, goals, and events in Month or Agenda view, manually or with separately enabled assistance. |
| **Backup and control** | Create and check encrypted backups, restore into an empty installation, and optionally enable automatic backups and vault locking. |

You can browse saved records, read Materials, and use manual Calendar and notebook controls without starting an AI conversation. You can also change supported providers while keeping the same local vault. Saved memory remains inspectable and revisable; it is not a promise that the model will remember everything correctly.

## Highlights since 0.9.13

- **More flexible Local AI:** guided Gemma setup, experimental Custom GGUF profiles with 8K/16K/32K context options, optional OBS vision, and explicitly enabled Brave web lookup.
- **Better local voice:** installed Windows voices, Kokoro CPU or optional NVIDIA GPU voice, reduced repeated startup work, and **Skip speech** for the current reply. Ordinary Markdown bullets and emphasis are omitted from speech while the original text stays intact.
- **Easier setup and upgrades:** Google, OpenAI, and Local appear together in Connection. Download verified optional components or reuse existing model, runtime, and speech folders outside the installation.
- **A more useful Map and clearer workspaces:** saved Map layouts, improved inspectors, more readable Materials and Calendar views, and expanded searchable/offline Help.
- **More reliable edits and answers:** notebook draft protection, corrected Calendar time-zone edits and Event-to-Task conversion, and separate **PCS save results** alongside substantive Local answers.
- **Less repeated work:** faster catalogue and memory browsing, more efficient deletion previews and Map navigation, improved Local scheduling, and clearer conversation-capacity and backup-limit guidance.

See the [0.9.24 release notes][release] for the full update. Skip speech stops current and queued playback; synthesis already underway may finish silently before the Local turn ends.

## Download and start

| Download | Choose this for |
| --- | --- |
| **[PCS-0.9.24-Windows-x64.zip][windows]** | The complete portable application: Windows launchers, ordinary Python, pinned application dependencies, PCS source, and offline Help. |
| [PCS-0.9.24-Source.zip][source] | Matching editable source, tests, documentation, and build support. Not the offline Windows installer. |
| [PCS-0.9.24-SHA256SUMS.txt][checksums] | SHA-256 checksums for both downloads. |

Most people need the **Windows ZIP**. Use the named release assets; GitHub's automatic **Source code (zip)** contains this download repository, not the full application. Keep all extracted files together because PCS verifies its package manifest.

1. **Download, verify, and extract** into a fresh writable folder. Do not run inside an archive viewer or overlay an older installation.
2. Open **Start PCS.exe**. First launch prepares the bundled Python environment offline and opens PCS in your desktop browser. No system Python installation is required.
3. **Create a vault** and safely retain its passphrase. PCS cannot recover a forgotten passphrase. Existing users should follow [Updating and backups](#updating-and-backups).
4. In **Settings → Connection**, choose Google, OpenAI, or **Local on this PC**. Configure the route, review learning and sharing choices, and save.
5. Start with a short typed message. Enable **Use microphone** before Start when you want voice, and enable other sharing only as needed.

### Choose your connection

**Google or OpenAI:** bring your own API key and check the provider's billing, limits, and data-use terms. Conversation, memory, preparation, and research have their own settings and restrictions. Help explains the supported profiles and setup.

**Local on this PC:** Settings guides the recommended Gemma model and verified llama.cpp/CUDA runtime on compatible Windows/NVIDIA hardware. Experimental **Custom GGUF** profiles require **Check compatibility** before saving and starting. Local conversation and memory have no cloud AI fallback.

Local models, AI runtimes, vision projectors, and speech packs are **optional separate downloads**, not bundled in the Windows ZIP. Typed Local use needs no speech pack. Local microphone input needs the English recognition pack; speech output can use an installed Windows voice or an optional Kokoro pack. Saved component folders can be reused across upgrades.

Optional **OBS vision** uses a scene you choose; OBS is a separate installation. Optional **Brave lookup** needs a Brave Search API key and explicit online permission: public queries and page requests leave the computer, while the selected Local model interprets the results. Separately approved preparation work can use its explicitly selected cloud provider.

## Your information and your choices

- **Local storage and provider sharing are separate.** Enabled cloud features can receive conversation, permitted memories, document passages, Calendar details, or selected OBS images. Review sharing settings before use.
- **Your encrypted vault** holds saved continuity, notebooks, prepared notes, Calendar records, saved web snapshots, remembered settings and credentials, and Map layout. Original local Materials files and readable exports are outside vault encryption.
- **Don't save this conversation** controls new PCS saving; it does not prevent cloud providers from receiving the conversation or disable every sharing choice. Clear chat clears the display, not saved continuity. Hiding the memory stream does not stop learning.
- **Stop** ends the conversation and capture. **Lock** also closes vault access. **Quit PCS** shuts down the host; wait for **PCS closed**. Closing the browser tab alone can leave the host running. Keep the full launch URL private because it contains an access token.
- **Review important results.** Transcription, model answers, memory interpretations, and practice assessments can be wrong. A model's claim that it saved something is not proof: check the PCS save result and saved record. Deleting a record does not retract earlier provider disclosure or remove old backups.

## Updating and backups

**Quit PCS before upgrading. Keep the earlier installation, your passphrase, and a backup of the complete cleanly stopped data folder, including Materials.** Extract the new version into a fresh folder. A new extraction does not automatically locate older data.

Choose one transfer method:

- **Encrypted backup and restore:** save and check a backup, then restore it into the fresh installation instead of creating a new vault. Copy original local Materials separately, keeping their names and relative folders, and refresh documents while stopped.
- **Complete stopped-folder copy:** after shutdown, copy the entire old data folder beside **Start PCS.exe** in the fresh extraction before launching. Keep the original, then unlock and verify the new copy. Use the actual data directory if you configured a custom location.

Do not merge independent vaults or run two installations against the same data directory. Reselect the automatic-backup destination after moving or restoring. In-app manual and automatic backup have a **256 MiB** limit; larger vaults use the documented stopped-folder method. Capacity warnings do not mean a new backup succeeded.

Some saved features raise the minimum PCS version that can reopen a vault and its later backups. For example, NVIDIA GPU voice requires 0.9.21 or newer and Custom GGUF profiles require 0.9.22 or newer. Clearing a choice does not lower that requirement. Keep a pre-upgrade backup if rollback matters, and follow **`docs/RESTORE_VAULT.md`** inside the download.

## Help, limits, and feedback

Open **Help** inside PCS or **`docs/HELP.html`** for searchable offline guidance. The downloads also include:

- `START_HERE.md` and `docs/GETTING_STARTED.md` — setup and first use.
- `docs/RESTORE_VAULT.md` — backups, upgrades, and recovery.
- `docs/CONTINUITY_MAP.md` — Map navigation, dates, paths, and evidence.
- `docs/RELEASE_NOTES.md` — changes and feature boundaries.
- `docs/developer/README.md` — development and testing.

PCS remains a **pre-release**. Hardware compatibility, recognition quality, provider limits, and long conversations can affect results. Calendar does not synchronize Google or Outlook accounts, send invitations, or deliver reminders. Web capture supports bounded public static pages, not interactive sites, sign-ins, or a guarantee of complete capture.

For 0.9.24, **6,840 Python tests and 1,256 JavaScript tests passed**, with two documented Windows permission-dependent skips. Fresh offline installation, synthetic vault lifecycle, browser workflows, and bounded native speech checks also passed. These checks do not establish live cloud-provider, physical microphone/OBS/GPU, or every Local model's behavior.

Report bugs through [GitHub Issues][issues] or join [Discord][discord]. Include your PCS version, provider route, reproduction steps, and expected versus actual behavior. Export **Bug report before quitting** when possible, review it, and remove private information before sharing. Never post keys, passphrases, launch tokens, or private vaults.

## Support PCS

PCS is free. There is no PCS subscription and no feature is locked behind payment. Optional contributions help support development; AI-provider charges are separate.

[![Support PCS on Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)][kofi]

## Source and license

This repository hosts releases, project documentation, and issues. **The application source is attached to each release.** Download the matching [Source ZIP][source] and follow `SOURCE_README.md` and `docs/developer/README.md`. The Windows ZIP additionally contains the pinned runtime, offline wheelhouse, and compiled launchers. Use synthetic data and disposable vaults for development.

Copyright (C) 2026 Courtney Dickson. First-party PCS code is licensed under **GNU GPL version 3 only (GPL-3.0-only)**. See [LICENSE](LICENSE) and [COPYRIGHT](COPYRIGHT). PCS is provided without warranty. Separately identified components retain their own terms; see [THIRD_PARTY.md](THIRD_PARTY.md) and the notices in each download.

[windows]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.24/PCS-0.9.24-Windows-x64.zip
[source]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.24/PCS-0.9.24-Source.zip
[checksums]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.24/PCS-0.9.24-SHA256SUMS.txt
[release]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/tag/v0.9.24
[website]: https://pcs-personalcontinuitysystem.github.io/PCS-site/
[discord]: https://discord.gg/558hSvYp4
[issues]: https://github.com/PCS-PersonalContinuitySystem/PCS/issues
[kofi]: https://ko-fi.com/pcssupport
