# PCS - Your personal thinking space

**Room to think. Space to connect.**

Some thoughts need more than one conversation. PCS brings AI conversation, revisable memory, reading, notes and planning into a workspace you own. Explore a question, work through a difficult passage, keep an idea for later, or return to a project with the context you chose to save.

**Change the AI. Keep your continuity.** Use a supported Local, Google or OpenAI connection while your saved conversations, memories and notebooks stay in PCS. Each model brings its own abilities; your workspace belongs to you.

**[Download for Windows][releases]** · [Release notes][releases] · [Website][website] · [Discord][discord] · [Report a bug][issues]

> **PCS 0.9.78 · Pre-release · Windows x64**  
> Free and open source, with no PCS subscription or paid feature tiers. Cloud API usage is billed separately by the services you choose. Local models, AI runtimes and optional speech packs are separate downloads.

![PCS Conversation with a Local model, conversation pace controls and the compact message composer.](assets/pcs-conversation-0.9.78.png)

*PCS 0.9.78 with Local Huihui, using a fictional creative-writing prompt. Experimental quiet-moment openings were enabled for this example; they are off by default.*

**A place to work through things.** Start with conversation, then add the tools that help you continue.

| When you want to… | PCS gives you… |
| --- | --- |
| Think something through | Typed or spoken conversation, editable Companion direction and a choice of conversation pace. |
| Return to an earlier thread | Saved conversations and revisable memories, with source inspection, corrections and permitted recall. |
| Keep an unfinished thought | An encrypted Keep for later shelf; Continue prepares an editable draft for you to send. |
| Build on something you kept | Reviewed quotations in an existing Notebook or lesson, or a new Calendar task, goal or event. |
| Read and learn | Materials readers, Web snapshots, bookmarks, Read Along, reading notes, lessons and recorded Practice. |
| Find connections | A Continuity Map with Focus, Constellations, Connections and the saved records behind them. |
| Find your saved work | Grouped Library search, separate Map-note and Practice-history scopes, and routes back to the owning feature. |

Manual reading, notes, Calendar entries and saved-record browsing work without starting an AI conversation. You can build up your workspace at your own pace.

**Memory you can inspect and revise.** Saving conversation text and allowing memory formation are separate choices. With learning enabled, PCS can create model-written accounts linked to original passages. Inspect the evidence, review earlier wording, correct an account in ordinary language or choose Forget. Your words, your corrections and model interpretations remain distinguishable.

Recall uses the sharing permissions you enable, and relevant corrections stay attached to the recalled material. Optional Search by meaning uses a separate local search model. Saved accounts can still be incomplete or mistaken; inspect and revise what matters to you.

For a gentle beginning, **Build my starting map** offers six optional opening questions. Preview the prompt, choose what to share, and skip or stop whenever you want. Normal saving and learning choices apply when you send it.

**Keep a thought, then decide what to do with it.** Review a note or suggestion before keeping it. Later, continue it in Conversation, mark it resolved, reopen it or remove it. Adding a quotation to a Notebook, lesson or Calendar entry preserves the original wording and authorship separately from your own framing. Quotations are local display/export content; your framing follows the destination's normal sharing settings. These actions do not schedule automatic follow-ups or reminder delivery.

**Explore the records behind a connection.** The Continuity Map lets you follow a theme, compare groups, inspect supporting records and prepare a reviewed conversation draft. Saved views, Back and Forward, and your own connection notes help you return to a line of thought.

![PCS Continuity Map showing a selected Astronomy and Photography connection beside its supporting fictional records.](assets/pcs-map-0.9.78.png)

*PCS 0.9.78 with fictional demonstration records. The selected connection opens its supporting saved material. Map labels and counts describe that material; they do not establish truth, personality traits or causes.*

**Read, discuss and learn.** Materials supports readable PDFs, EPUBs, Office and OpenDocument files, tables, slides, subtitles, HTML and common text/code formats. Search a passage, keep a bookmark, listen through an available local voice, or review an excerpt before discussing it with your selected model. Resume reading brings retained positions together while keeping their source versions clear.

Notebooks hold your notes, goals, lessons and source references. Practice can retain submitted answers and assessments when you enable it. Optional research can find public evidence and prepare study notes. Scanned documents need OCR elsewhere, and some Web pages cannot be captured. Extraction notices explain omissions; model-generated explanations and assessments need review.

**Choose how much initiative you want.** Conversation pace offers **Follow my lead**, **Think with me** and **Take the lead**. Quiet and Stay here pause topic planning until you explicitly resume. Companion instructions are editable, and reply quality depends on your chosen model.

Local also has an experimental, session-only option for a brief contribution during a quiet moment. It starts unchecked, requires Take the lead and an eligible idle Conversation page, and cannot use tools or save the contribution as a source. Typing, leaving the page, Quiet, Stay here and Stop revoke pending openings. Preparing an idea can add processing time. Google and OpenAI quiet-moment openings remain unavailable.

Optional **Jev** uses TypeSafe to choose among ideas proposed by your conversation model. It starts off, requires its own key and a sharing review, and adds a cloud request. Local use requires separate cloud consent. Jev does not independently browse your vault or write the reply. Optional screen help and tutoring have their own setup and permissions too.

**Choose where the AI runs.**

| Connection | What you need |
| --- | --- |
| **Local on this PC** | Compatible hardware, a supported model and verified runtime. The recommended Gemma/CUDA setup needs a compatible NVIDIA GPU. Experimental Custom GGUF setups have their own compatibility checks. |
| **Google or OpenAI** | Your provider API key and access to a compatible model. API usage is separate from consumer chat subscriptions. |
| **Experimental Alibaba Qwen** | Its region/workspace setup and API key. This route is voice-only and has a smaller feature set. |

Local conversation and memory have no cloud AI fallback. For offline use, download the required components first, use Local conversation and memory, and leave online tools and cloud preparation off. Brave lookup sends public queries and page requests outside your computer; Local + Jev and cloud preparation send their separately approved inputs to their stated providers.

Typed Local conversation needs no listening pack. Optional English microphone input, Windows or Kokoro speech, local semantic search and compatible OBS vision can be added separately. Saved connections let you switch setups while stopped. Windows Radeon Vulkan text and Ubuntu browser/cloud operation remain experimental previews; macOS is not included.

**Start with one short conversation.**

1. Open [Releases][releases] and download **PCS-0.9.78-Windows-x64.zip**. Extract the complete ZIP into a fresh writable folder.
2. Open **Start PCS.exe**. The first launch prepares its bundled Python environment offline; no system Python installation is needed.
3. Create a vault and keep the passphrase safe, or follow the included instructions to restore your encrypted backup.
4. In **Settings → Connections**, set up your provider or Local model. Review **Memory & sharing**, then save your settings.
5. Return to Conversation, leave **Use microphone** off, choose **Start PCS** and send a short message. Add voice, Materials sharing, Vision and optional tools after that works. Experimental Qwen requires voice instead.

The package includes `START_HERE.md`, a full Getting started guide and searchable offline Help. Keep the application files together: the launcher verifies the package manifest. Use **Quit PCS** when finished; closing the browser tab alone can leave the application running.

**Your data and your sharing choices.**

- Saved continuity lives in your local encrypted vault. Original Materials files and readable exports are outside that encryption.
- Cloud features receive the information allowed by their controls. **Don't save** controls PCS retention; it does not prevent the selected provider from receiving the conversation.
- Corrections and forgetting affect PCS records and dependent saved work. They cannot retract information already disclosed or erase earlier backups.
- Keep your vault passphrase safe. PCS cannot recover it. Changing it affects the working vault; existing backups keep their original passphrases.

Before upgrading, save an encrypted backup, copy original Materials separately and quit PCS. Extract the update into a fresh folder and keep your previous installation and pre-upgrade backup. Never run two copies against the same data folder. Saving new features can require a newer PCS reader: new certified Keep source-attribution records, quotations and Practice recovery content require **0.9.78+** once saved. Help includes the full compatibility table.

Automatic backups retain the newest copy from each of the 14 most recent days and eight most recent weeks. Copy one elsewhere if you want to retain it beyond that window; manual and protected backups are excluded from automatic pruning.

**What's new in 0.9.78?** More room for chat, Keep for later and reviewed quotations, connected saved-work search and reading, clearer conversation controls, refreshed Help, and fixes across Local replies, Materials refreshes, drafts and recovery. The [release notes][releases] cover the cumulative changes since 0.9.71.

**Help, feedback and development.** PCS is under active development. AI replies, memories, transcription and research can be wrong. The final 0.9.78 package passed 12,015 Python tests and 2,833 JavaScript tests, with six reviewed platform exclusions, plus installation, browser, lifecycle and delivered-file checks. Isolated Huihui trials exercised Local openings and interruption; these results do not establish audio overlap, every model or multi-hour reliability.

Use [GitHub Issues][issues] or [Discord][discord] for feedback. Include your version, connection, steps and expected result. Review diagnostics before sharing; exclude keys, passphrases, launch tokens and personal records.

This repository hosts project information and release downloads. Developers should choose **PCS-0.9.78-Source.zip** from the release assets, which includes the application source, tests and build support. GitHub's automatic **Source code** archive contains this download repository. The release also provides **PCS-0.9.78-SHA256SUMS.txt** for archive verification.

PCS first-party code is licensed under **GPL-3.0-only**, without warranty. See [LICENSE][license], [COPYRIGHT][copyright] and [third-party notices][third-party]. Optional contributions through [Ko-fi][kofi] help support development; provider charges remain separate.

[releases]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases
[website]: https://pcs-personalcontinuitysystem.github.io/PCS-site/
[discord]: https://discord.com/invite/2ssCQhNgAN
[issues]: https://github.com/PCS-PersonalContinuitySystem/PCS/issues
[license]: https://github.com/PCS-PersonalContinuitySystem/PCS/blob/main/LICENSE
[copyright]: https://github.com/PCS-PersonalContinuitySystem/PCS/blob/main/COPYRIGHT
[third-party]: https://github.com/PCS-PersonalContinuitySystem/PCS/blob/main/THIRD_PARTY.md
[kofi]: https://ko-fi.com/pcssupport
