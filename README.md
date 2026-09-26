# PCS — Personal Continuity System

**Room to think. Space to connect.**

PCS is a Windows AI companion for conversation, learning, reading, and everyday plans—with continuity you can inspect and revise. Talk ideas through, work through a book, return to a project, or explore a question together. Keep useful context in your own encrypted vault instead of tying it to a single AI provider.

**[Download PCS 0.9.13 for Windows][windows]** · [Release notes][release] · [Website][website] · [Discord][discord] · [Report an issue][issues]

> **0.9.13 · Pre-release · Windows x64**  
> PCS is free, with no PCS subscription or locked features. Cloud features use your own API keys and may incur provider charges. The supported Local route uses your hardware and requires separate model and runtime downloads.

## Your context, under your control

PCS separates the AI you talk to from the saved context you keep. You can change supported providers while retaining the same local vault. Memories are not a hidden profile you must simply trust: you can inspect their sources, correct interpretations, review revisions, and remove records.

The aim is useful continuity—not a companion that claims to remember everything or always agree with you.

## What you can do

| Area | What it offers |
| --- | --- |
| **Conversation** | Talk or type with Google, OpenAI, or the supported Local model. Customize the companion's directions. On supported cloud routes, optionally share visual context from an OBS scene you choose. **OBS is a separate download, not bundled with PCS.** |
| **Continuity** | Browse saved memories and notebooks in Library, inspect evidence and revision history, and explore recurring wording and connections in Map. Review a **Continue this thought** draft before sending it. |
| **Materials** | Bring TXT, Markdown, selectable-text PDF, or EPUB documents. Consult passages, prepare reading notes, organize notebooks, and retain research notes or captured web sources for later use. |
| **Learning and research** | Work through source material, organize learning steps, use practice activities, and request research on supported cloud routes. Keep original sources, AI-prepared explanations, and your own notes distinguishable. |
| **Calendar** | Manage tasks, goals, and events in Month or Agenda view. Use it manually or choose separately how much assistance PCS may provide. |
| **Backup and control** | Create and check encrypted vault backups, restore into an empty installation, and optionally enable automatic backups or vault locking. Original local Materials files need a separate copy. |

You can browse saved records, read Materials, and use manual Calendar and notebook controls **without starting an AI conversation**. Map browsing is local and read-only: its links reflect shared record wording, not proof of agreement, causation, or a psychological profile.

## New in 0.9.13

### More room to finish your thought

OpenAI now defaults to patient semantic turn detection, with a short settling window before a spoken turn triggers a reply. When provider speech detection notices you speaking, playback yields before PCS decides whether to cancel the answer. An utterance classified as empty can release the same unheard audio without requesting another answer.

**Settings → OpenAI turn completion** offers patient or balanced semantic detection and a **1.5-second silence-based fallback**. Changes apply on the next Start. Recognition errors, network conditions, and actual provider limits can still affect timing.

### A more self-assured companion

The default direction emphasizes a calm, capable peer: accuracy over agreement, fair disagreement backed by reasons, revisable judgments, and useful follow-through without constant praise or obligatory questions. Customized directions are preserved; only exact previously shipped defaults are replaced. These instructions guide the model, rather than guarantee its behavior.

### Find once, keep in Materials

Save a supported public quiz, study guide, reference page, or walkthrough as a reusable source:

> “Find a public astronomy quiz and save the source in Materials.”

Ask during a cloud conversation with **Search** and **Materials sharing** enabled, or use **Materials → Reference notes → Saved web sources → Add from web**. A routine search does not automatically save anything.

Saved web sources keep their extracted text, source addresses, capture date, and coverage limitations. They are **encrypted vault records, separate from personal memories**. Inspect them, consult them in portions, explicitly save a bookmark or spoiler-boundary note, export them, or capture an updated version. When captured text changes, refreshing preserves the earlier snapshot and its bookmark.

Later, ask PCS to return to the saved source and your bookmark. This is reusable reference material—not an invisible, expiring cache, an automatic grader, or a guarantee that a whole guide or answer key was captured.

<details>
<summary><strong>Web capture limits</strong></summary>

Capture supports **one public HTTPS HTML, TXT, or Markdown page** per source, up to **2 MiB downloaded** and **240,000 text characters**. Oversized sources are rejected rather than silently shortened. The vault can retain up to **128 snapshots**, including refreshed versions.

PCS does not execute JavaScript or interactive quizzes, crawl linked chapters, extract images, import remote PDFs, sign in to websites, or bypass access controls. Some sites will not allow anonymous capture. Ordinary local PDF imports remain a separate Materials feature.

The conversation model reads or searches saved web text in portions of up to **6,000 characters per call**; the whole source is not automatically added to every prompt. Previously supplied passages can still accumulate in a live conversation and consume provider allowance.

Bookmarks are explicit saved notes, not inferred progress. They are not automatically moved to a changed version. Deleting a snapshot requires stopping the conversation and does not delete other versions or old backups. Readable TXT exports are unencrypted. Don't-save mode blocks saved-source changes and exports; Local mode cannot fetch new web pages. Materials sharing governs model access to already-saved sources.

</details>

## Download and start

| Download | Choose this for |
| --- | --- |
| **[PCS-0.9.13-Windows-x64.zip][windows]** | The complete Windows application, with launchers, portable Python, pinned dependencies, offline English speech-recognition assets, source, and Help. |
| [PCS-0.9.13-Source.zip][source] | Matching development source, tests, documentation, and build support. Not a ready-to-run Windows package. |
| [PCS-0.9.13-SHA256SUMS.txt][checksums] | SHA-256 checksums for both archives. |

Most people need only the **Windows ZIP**. Choose the named release asset—not GitHub's automatically generated **Source code (zip)**. Keep every extracted package file together: the launcher verifies the package manifest.

### First-time setup

1. **Download, verify, and extract** the complete Windows ZIP into a writable folder. Do not run it inside an archive viewer or overlay an older installation.
2. Open **Start PCS.exe**. First launch prepares its bundled Python environment offline and opens PCS in your desktop browser. No system Python installation is required.
3. **Create a vault** with a long, unique passphrase and store it safely. PCS cannot recover a forgotten passphrase. Existing users should follow [Updating and backups](#updating-and-backups) instead.
4. Open **Settings → Connection**, configure your route, review memory and sharing choices, and save. Return to Conversation and select **Start PCS**. Begin with a short typed message; enable **Use microphone** before Start for voice.

**Google or OpenAI:** supply your own API key and check your provider's billing and limits. Memory, preparation, and research have their own provider settings and feature restrictions. [OpenAI API usage is billed separately from a ChatGPT subscription][openai-billing]. Help explains the Google free-route restrictions.

**Local:** use the supported model, runtime, and CUDA-library downloads identified in Settings and Help on compatible Windows/NVIDIA hardware. These downloads are separate from the Windows ZIP. Local conversation supports text and optional offline English voice, requires no API key, and has no cloud fallback. Local vision and network research are unavailable; do not assume arbitrary model or runtime substitutes are supported.

The interface runs locally, but the full launch address contains an access token. **Keep that address private.**

## Your information and your choices

**Local storage does not mean every AI request stays local.** With cloud features enabled, selected content can go to the configured providers: your conversation, permitted memories, document passages, Calendar details, or OBS screenshots. Review the sharing choices and provider terms before enabling those features.

The encrypted vault holds saved continuity, prepared notes, notebooks, Calendar records, saved web sources and bookmarks, and settings or credentials you chose to remember. **Original local Materials files and readable exports are outside vault encryption.** Back up and protect them separately.

**Don't save this conversation** pauses new PCS saving; it does not prevent your cloud provider from receiving the conversation or turn off all existing sharing choices. **Clear chat** clears the display, not saved continuity. Hiding the memory stream does not stop learning.

**Stop PCS** ends the conversation and capture. **Lock** also closes vault access. **Quit PCS** shuts down the host; wait for **PCS closed** before closing the tab. Closing the browser tab alone can leave the host running and the vault unlocked.

## Updating and backups

> **Important for 0.9.13:** saving the first web source makes that vault require **PCS 0.9.13 or newer**, even after the source is deleted. Keep a **pre-feature backup** for rollback. Merely opening an older vault without saving a web source does not add this requirement. The encryption format is unchanged.

A fresh extraction does not automatically find your older data. Keep the previous installation and a verified backup until the new copy is working. Choose **one** transfer method; do not merge independent vaults.

<details>
<summary><strong>Guided method: encrypted backup and restore</strong></summary>

1. Save edits, finish or cancel background work, and stop the conversation while leaving the vault unlocked. Choose **Backup & restore → Save current backup…**, save outside the installation, and wait for confirmation. Then **Quit PCS** and wait for **PCS closed**.
2. Extract the new Windows ZIP into a fresh folder and run **Start PCS.exe**. Choose **Restore an encrypted backup instead**—do not create a new vault.
3. Select the `.pcs` backup, enter its passphrase, and choose **Check backup**. Review the counts, select **Restore this backup**, then **Unlock existing** and check your records and settings.
4. Copy the original files from the old **data/Materials** folder into the new **data/Materials** folder, preserving filenames, contents, and relative subfolders. With the vault unlocked and conversation stopped, choose **Materials → Refresh documents**.

Encrypted backups include saved web sources and bookmarks, along with other vault records and remembered credentials. They do **not** include original local Materials files. The in-app backup/restore limit is **256 MiB**; larger vaults require the complete-folder method.

</details>

<details>
<summary><strong>Alternative: copy the complete stopped data folder</strong></summary>

Use **Quit PCS** and wait for shutdown. Back up the entire old **data** folder, then place a copy beside **Start PCS.exe** in a fresh extraction **before launching it**. Keep your original copy; do not merge it with another data folder.

Launch, choose **Unlock existing**, verify your records and settings, and refresh Materials while stopped. This transfers both the vault and ordinary Materials files; the latter remain unencrypted. For custom data locations, use the directory your launcher actually uses.

</details>

After a move or restore, reselect your automatic-backup destination and update shortcuts as needed. **Never run two instances against the same data directory.** The downloaded `docs/RESTORE_VAULT.md` covers custom paths, larger vaults, and uncertain shutdowns. Preserve recovery files rather than deleting them to force a restore.

## Help and current limits

Open **Help** inside PCS, or open **`docs/HELP.html`** from the extracted package for searchable offline guidance.

| Included guide | File inside the download |
| --- | --- |
| Quick start and setup | `START_HERE.md` and `docs/GETTING_STARTED.md` |
| Backup, restore, and folder transfers | `docs/RESTORE_VAULT.md` |
| Features, controls, and boundaries | `docs/REFERENCE.md` |
| Map navigation and evidence | `docs/CONTINUITY_MAP.md` |
| Current changes and validation | `docs/RELEASE_NOTES.md` and `docs/developer/AUDIT_0.9.13.md` |
| Development and target-machine checks | `docs/developer/README.md` and `docs/developer/ACCEPTANCE_0.9.13.md` |

These files are **inside the release packages**, not this repository's root.

PCS is a **pre-release**. Transcription, vision, memory, and recall can be wrong or incomplete. Long conversations, tool activity, provider limits, or connection renewal can introduce pauses. Saved material is not proof that every page has been read; practice assessments are provisional. Calendar does not synchronize Google or Outlook accounts, book appointments, invite attendees, or deliver reminders.

The 0.9.13 validation covers automated and simulated checks with disclosed skips. It does **not** establish native Windows, live-provider, physical audio/OBS/GPU, or successful live web-capture acceptance. See the [release notes][release] and included validation documents for the tested scope. Keep backups and verify important answers and saved changes.

## Feedback and support

Report bugs through [GitHub Issues][issues] or discuss PCS in [Discord][discord]. Include the version, provider route, expected and actual behavior, and steps to reproduce. Export **Bug report before quitting** when possible and review it before sharing; reports are not uploaded automatically. Never post API keys, passphrases, full launch addresses, private vaults, or personal conversations.

**PCS is free and does not require payment.** Optional one-time contributions support development. There is no PCS subscription and no features are locked behind payment. AI-provider charges are separate.

[![Support PCS on Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)][kofi]

## Source and development

This repository hosts releases, project documentation, and issues. **The complete application source is attached to each release**; cloning this repository or downloading GitHub's automatic source archive does not provide the application source tree.

Download **[PCS-0.9.13-Source.zip][source]** and follow `SOURCE_README.md` and `docs/developer/README.md`. The Windows ZIP also includes application source, plus the pinned runtime, offline wheelhouse, and compiled launchers omitted from the source-only export. Use synthetic data and disposable vaults for development and testing.

## License

Copyright (C) 2026 Courtney Dickson.

First-party PCS code is licensed under **GNU GPL version 3 only (GPL-3.0-only)**. See [LICENSE](LICENSE) and [COPYRIGHT](COPYRIGHT). PCS is provided without warranty. Separately identified third-party components retain their own licenses; see [THIRD_PARTY.md](THIRD_PARTY.md) and the notices in each download.

[windows]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.13/PCS-0.9.13-Windows-x64.zip
[source]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.13/PCS-0.9.13-Source.zip
[checksums]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.13/PCS-0.9.13-SHA256SUMS.txt
[release]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/tag/v0.9.13
[website]: https://pcs-personalcontinuitysystem.github.io/PCS-site/
[discord]: https://discord.gg/558hSvYp4
[issues]: https://github.com/PCS-PersonalContinuitySystem/PCS/issues
[kofi]: https://ko-fi.com/pcssupport
[openai-billing]: https://help.openai.com/en/articles/9039756-managing-billing-for-chatgpt-and-the-api-platform
