# PCS - Your personal thinking space

**Room to think. Space to connect.**

Some thoughts need more than one conversation. PCS brings AI conversation, revisable memory, reading, notes and planning into a workspace you own. Bring an unfinished question, a difficult passage or an idea. Work on it, keep where you stopped and what you want to try next, then come back with a place to begin.

**Change the AI. Keep your continuity.** Use a supported Local, Google, OpenAI or Meta connection while your saved conversations, memories and notebooks stay in PCS. Each model brings its own abilities; your workspace belongs to you.

**[Download for Windows][windows]** · [Release notes][release] · [Website][website] · [Discord][discord] · [Report a bug][issues]

> **PCS 0.9.114 · Windows x64 · Under active development**
>
> Free and open source, with no PCS subscription or paid feature tiers. Cloud API usage is billed separately by the services you choose. Local models, AI runtimes and optional speech packs are separate downloads.

![PCS 0.9.87 showing the Astronomy and Photography connection, with a saved note about lenses open for review.](https://raw.githubusercontent.com/PCS-PersonalContinuitySystem/PCS/main/assets/pcs-continuity-map-0.9.87.png)

*Fictional demonstration workspace from PCS 0.9.87. Inspect the saved words behind a connection and choose what to carry into your next conversation. This image shows an earlier interface.*

## A place to work through things

Start with conversation, then add the tools that help you continue.

| When you want to… | PCS gives you… |
| --- | --- |
| Think something through | Typed or spoken conversation, editable Companion direction and a choice of conversation pace. |
| Return to an earlier thread | Saved conversations and revisable memories, with source inspection, corrections and permission-controlled recall. |
| Keep an unfinished thought | An encrypted Keep shelf with editable stopping points, next steps and pins, plus an editable draft when you return. |
| Follow how an idea changed | Links between exact memory revisions, settled marks and named lessons with supporting stories. |
| Explore a connection | A Continuity Map with saved evidence, guided discovery and landmarks written in your own words. |
| Read and learn | Materials readers, Web snapshots, bookmarks, Read Along, Prepared Notes, notebooks and Practice. |
| Find your saved work | A searchable Library with routes back to memories, notebooks and their sources. |
| Plan your next step | Calendar tasks, goals and events, with reviewed quotations from work you kept. |

Manual reading, notes, Calendar entries and saved-record browsing work without starting an AI conversation.

## Get started

1. Download **[PCS-0.9.114-Windows-x64.zip][windows]** and extract the complete ZIP into a fresh writable folder.
2. Open **Start PCS.exe**. First launch prepares the bundled Python environment offline; no system Python installation is needed.
3. Use **Quick Setup** to create your vault and choose a connection. Keep the passphrase safe. **Existing users: restore an encrypted backup before creating a new vault.**
4. Enter your supported provider API key, or follow **Local model & files** to install the required Local components. Review what you want to save and share. Quick Setup includes a **conversation-only** option.
5. Microphone use starts off in a new setup. Unlock the vault, type a message and choose **Start & send**. Add voice, Materials sharing, Vision and optional tools when you want them. The experimental Qwen route requires voice instead.
6. At a useful stopping point, choose **Keep a stopping point** and review what you want to retain.

The package includes `START_HERE.md`, a full Getting started guide and searchable offline Help. Keep the application files together: the launcher verifies the package manifest. Use **Quit PCS** when finished; closing the browser tab alone can leave the application running.

## Bring one unfinished thing

Start with a question, decision, passage or idea that matters to you. For example: *“I keep changing my mind about this project. Help me work through the next decision.”*

Conversation pace offers **Follow my lead**, **Think with me** and **Take the lead**. Think with me is guided to develop one manageable thought at a time and leave room for your response. **Quiet** and **Stay here** pause topic planning until you explicitly resume. Companion instructions are editable.

If you would rather begin broadly, **Build my starting map** offers six optional opening questions. Preview the prompt, choose what to share, and skip or stop whenever you want. Your saving and learning choices still apply.

Local also offers an experimental, session-only option for a brief contribution during a quiet moment. It starts off and requires **Take the lead**. Preparing an idea can add processing time.

## Leave a stopping point and return later

Choose **Keep a stopping point** beneath the message box. Give the thought a title, write where you stopped, and optionally add what you want to try next. Review it before saving to the encrypted Keep shelf.

Pin a thought to bring it forward when you return. Edit your note and next step, mark it resolved, reopen it or delete it when you choose. A kept PCS quotation retains its recorded wording and authorship separately from your own framing.

On a later visit:

1. Unlock your vault and choose **Load saved threads**.
2. Review the suggested stopping point, its sources and any changed-source warnings.
3. Choose **Review & continue** to prepare an editable draft.
4. Review the draft and decide whether to send it.

Loading the return card reads local records without a model request. Existing unsent text is protected. After continuing a thought, its title and next step remain available across Conversation, Materials, Continuity and Calendar. **Explore in Map** carries it into the Map as a temporary reminder.

## Memory you can inspect, revise and connect

Saving conversation text and allowing memory formation are separate choices. With learning enabled, PCS can create model-written accounts linked to original passages. Inspect the evidence, review earlier wording, correct an account in ordinary language or choose **Forget**. Your words, your corrections and model interpretations remain distinguishable.

Recall follows your sharing permissions and keeps relevant corrections attached. Local checks whether a question needs saved context before replying. PCS distinguishes failed or blocked lookups from completed searches with no matching result. Memories and AI answers can still be incomplete or mistaken.

### Follow how an idea developed

Open a memory and choose **Settled, links & lessons**:

- **Link memories** to record how one idea changed into another or came from an earlier experience. You can then ask how a decision developed through those saved relationships.
- **Mark settled** to identify an exact memory revision as your current word on its subject. Correcting it retires that mark until you review the new wording.
- **Keep a named lesson** with a story, takeaway and supporting memories. PCS can retrieve the complete saved story when it fits the available context.

Links and lessons retain the revisions you reviewed; changed or unavailable references are identified. Available referenced history is protected during ordinary automatic pruning, but wording already pruned by an older version cannot be recovered. Forgetting a memory still removes its revisions and updates dependent records.

Supported Google, OpenAI and Meta conversations can propose links or lessons. These remain suggestions until you accept them.

### Optional help noticing saved context

**Help notice relevant memories in conversation**, under **Settings → Memory & sharing → Personal memory**, starts off and requires existing memory-sharing permission.

When enabled, supported routes can use a compact overview of saved areas and lesson names. Google, OpenAI and Meta can receive it at startup; Local uses area and lesson names when deciding whether to look up memory. Local and Meta can also receive matching cues for typed and completed spoken turns. Stories and supporting records are retrieved separately.

The overview is built locally, follows sharing choices and is omitted when it cannot fit. A cue sent to a cloud provider still shares that information. These hints help navigate saved material; they do not guarantee that a relevant memory will be found.

## Explore the records behind a connection

The **Continuity Map** offers **Focus**, **Constellations** and **Connections**, with access to the saved records behind the display. Choose **Discover a connection** for a short guided exploration, inspect the evidence, or **Leave a landmark** in your own words. You can also explore freely.

Choose **Index the whole archive** in the coverage panel to include up to **50,000 memories**. The encrypted index stays in step with saves, corrections and forgetting. The Map supports up to **250 themes** and bundles connections between constellations into expandable lines.

Map labels and counts describe saved material. They do not establish truth, personality traits or causes. You decide what a connection means to you.

### Optional Jev exploration

In **Continuity → Library**, select a record and choose **Explore connections**. Add a question, review the proposed records, and choose which excerpts may be shared. Jev can suggest relevance, repetition, added information or possible disagreement within that reviewed set.

This optional trial requires a TypeSafe key and separate sharing permission for each request. Suggestions remain provisional and do not automatically create memories or change the Map. Ordinary Library browsing and Map exploration work without it.

Jev also has a separate conversation-carrying role that can choose among ideas proposed by your conversation model. That role starts off, has its own review, and requires additional cloud consent when used with Local.

## Read, discuss and learn

**Materials** supports readable PDFs, EPUBs, Office and OpenDocument files, tables, slides, subtitles, HTML and common text/code formats. Search a passage, keep a bookmark, listen through an available local voice, or review an excerpt before discussing it with your selected model.

**Prepared Notes** can support a longer reading project. **Prepare book** works through an explicitly approved sequence and saves a checkpoint after each portion. **Resume** lets you review the next scope. Local preparation can use portions of up to **80,000 source characters** when the complete request fits; this is a ceiling, not a guaranteed portion size. Topic search can find wording inside saved notes and open a relevant excerpt.

Notebooks hold notes, goals, lessons and source references. Practice can retain submitted answers and assessments when enabled. Optional research can find public evidence and prepare study notes. Prepared reading notes and retained research notes remain distinct.

Scanned documents need OCR elsewhere, and some Web pages cannot be captured. Extraction notices identify omissions, including blank or unextractable PDF ranges.

You can also attach or drop a UTF-8 `.txt` or `.md` file and review it before choosing **Use in this chat**, **Keep for later**, or **Save reviewed text in Materials**. Saving in Materials creates an ordinary file outside the encrypted vault; back it up separately.

Reviewed quotations can be added to a Notebook, lesson or Calendar entry while preserving their wording and authorship. Keeping a thought or creating a Calendar entry does not schedule automatic follow-ups or reminder delivery.

## Choose where the AI runs

| Connection | What you need |
| --- | --- |
| **Local on this PC** | Compatible hardware, a supported model and verified runtime. The recommended Gemma/CUDA setup needs a compatible NVIDIA GPU. Experimental Custom GGUF setups have their own compatibility checks. |
| **Google or OpenAI** | Your provider API key and access to a compatible model. Supported routes include cloud audio as well as text. API usage is separate from consumer chat subscriptions. |
| **Meta** | Your Meta API key and account access. Typed conversation needs no local language model or speech pack. Voice uses local transcription and Windows or Kokoro speech. |
| **Experimental Alibaba Qwen** | Its region/workspace setup and API key. This route is voice-only and has a smaller feature set. |

Conversation, memory processing and reading preparation have supported provider choices. Local conversation and memory have no cloud AI fallback. For offline use, download the required components first, use Local for the roles you need, and leave online tools and cloud preparation off.

Separately enabled services still send information outside your computer: Brave lookup sends public queries and page requests; Local + Jev shares separately reviewed conversation information with TypeSafe; Library exploration shares its approved excerpts; cloud preparation uses the provider and sharing choices selected for that role.

Typed Local conversation needs no listening pack. Optional English microphone input, Windows or Kokoro speech, local semantic search and compatible OBS Vision can be added separately. Windows Radeon Vulkan text and the Ubuntu source preview remain experimental. macOS is not currently included.

### More room for Local conversations

- Recommended Local on NVIDIA CUDA defaults to a **128K context window**, with selectable windows up to **256K** and **FP16 or Q8_0** cache options. Custom GGUF profiles retain their chosen window. Capacity and speed depend on your hardware, model and enabled features.
- Long Local sessions compact their working context while retaining recent complete exchanges. Older exact wording remains searchable for the rest of that session; saved originals remain unchanged.
- Local microphone turns allow up to **60 seconds**, with a warning at **50 seconds** and **1.5 seconds** of silence before ending a shorter turn.
- Active replies take priority over eligible background memory formation, which can retry later. Unchanged prompt prefixes can be reused, and interrupted model downloads can resume.

## What's new in 0.9.114?

This release brings together the work from **0.9.103–0.9.114**:

- Linked memories, settled marks, named lessons and a compact overview of saved topics.
- Whole-archive Map indexing, more themes and expandable connections between constellations.
- Larger Local context windows, working-context compaction and longer microphone turns.
- Larger Prepared Notes portions, resumable book preparation and search within saved notes.
- Clearer Quick Setup, including conversation-only use and more visible sharing choices.
- Remembered Jev and proactive-help approvals for exact reviewed model/input combinations.
- Repairs to memory saves, spoken confirmations, multilingual search, Materials, backups and shutdown.
- A **1920-pixel default maximum Vision width**, preserving proportions and explicit saved choices, plus an updated GPU-memory advisory threshold.

See the **[release notes][release]** for details, upgrade guidance and validation limits.

## Your data and sharing choices

- Saved continuity lives in your local encrypted vault. Original Materials files, imported text copies and readable exports are outside that encryption.
- Cloud features receive information allowed by their controls. **Don't save** controls PCS retention; it does not prevent your selected provider from receiving the conversation.
- Corrections and forgetting affect PCS records and dependent saved work. They cannot retract information already disclosed or erase earlier backups.
- PCS cannot recover a lost vault passphrase. Changing it affects the working vault; existing backups keep their original passphrases.
- **Stop**, **Lock** and **Quit PCS** are separate controls: end the connection, close vault access, or shut down the application.

## Upgrading and backups

Before upgrading, create an encrypted vault backup, copy original Materials files separately, and quit PCS.

Extract the update into a fresh folder. Open **Start PCS.exe** and choose **Restore an encrypted backup instead** before creating a vault. Check the backup, review its counts and restore it. Follow the included restore guide to reconnect Materials and choose your automatic-backup destination again.

Keep your previous installation and pre-upgrade backup until you have checked the restored copy. Never run two copies against the same data folder.

**Some features introduced since 0.9.102 raise the vault's minimum reader version.** These include saved memory links and lessons, whole-archive Map indexing, Local context settings, remembered proactive approvals and certain Prepared Notes checkpoints. **Check backup** reports the required reader; Help includes the compatibility table. Version 0.9.114 adds no further reader requirement beyond 0.9.113.

If you use proactive help, complete the one-time updated review through **Review model and inputs → Allow → Save settings**. The disclosure explicitly includes selected Activity and automatic Activity following when enabled.

## Development status and feedback

PCS is under active development. AI replies, memories, transcription and research can be wrong.

Use [GitHub Issues][issues] or [Discord][discord] for feedback. Include your version, connection, steps and expected result. Review diagnostics before sharing; exclude keys, passphrases, launch tokens and personal records.

## Source, checksums and license

This repository hosts project information and release downloads. Download **[PCS-0.9.114-Source.zip][source]** for the application source, tests and build support. GitHub's automatic **Source code** archive contains this download repository.

Use **[PCS-0.9.114-SHA256SUMS.txt][checksums]** to verify the release archives. Earlier versions are available under [Releases][releases].

PCS first-party code is licensed under **GPL-3.0-only**, without warranty. Third-party components retain their own license terms. See [LICENSE][license], [COPYRIGHT][copyright] and [third-party notices][third-party].

Optional contributions through [Ko-fi][kofi] help support development. Provider charges remain separate.

[windows]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.114/PCS-0.9.114-Windows-x64.zip
[source]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.114/PCS-0.9.114-Source.zip
[checksums]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.114/PCS-0.9.114-SHA256SUMS.txt
[release]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/tag/v0.9.114
[releases]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases
[website]: https://pcs-personalcontinuitysystem.github.io/PCS-site/
[discord]: https://discord.com/invite/2ssCQhNgAN
[issues]: https://github.com/PCS-PersonalContinuitySystem/PCS/issues
[license]: https://github.com/PCS-PersonalContinuitySystem/PCS/blob/main/LICENSE
[copyright]: https://github.com/PCS-PersonalContinuitySystem/PCS/blob/main/COPYRIGHT
[third-party]: https://github.com/PCS-PersonalContinuitySystem/PCS/blob/main/THIRD_PARTY.md
[kofi]: https://ko-fi.com/pcssupport
