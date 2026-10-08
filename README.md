# PCS - Your personal thinking space

**Room to think. Space to connect.**

**Some thoughts need more than one conversation.**
PCS gives you a place to explore them. Talk through a question, bring in something you’re reading, collect useful notes, and follow connections across your projects and conversations. Come back later and continue with the things you chose to keep.
Choose the AI that suits you. Your saved work stays together when you change models.
Change the AI. Keep your continuity.

PCS is a free, **open-source AI companion for Windows**, with local AI and supported cloud connections. Choose the tools you want, decide what they can receive, and keep your saved continuity when you change models.

**[Download PCS 0.9.71 for Windows][windows]** · [Release notes][release] · [Website][website] · [Discord][discord] · [Report a bug][issues]

> **0.9.71 · Pre-release · Windows x64**  
> PCS has no subscription or paid feature tiers. External AI services may charge for usage. Local models, runtimes and optional speech components are separate downloads.

## Change the AI. Keep your continuity.

Your conversation model can change while your saved conversations, revisable memories and notebooks remain in PCS. Switch between supported Google, OpenAI and Local setups without starting your personal workspace over.

Conversation, memory processing and preparation can use separate supported providers. Changing one connection does not silently change another provider's key or rewrite the records in your vault. Models still differ in their abilities and how they use the context you permit.

## An AI companion with memory you control

Saving a conversation and forming memories are separate choices. With learning enabled, PCS can create model-written accounts linked to the original passages. You can inspect those sources, see earlier wording, and correct or remove an account.

- **Correct memories in ordinary language.** Mark something Incorrect, Changed or specific to a context, then review the proposed change before saving.
- **Keep your words distinct.** Your corrections and notes remain distinguishable from AI interpretations.
- **Find earlier context.** Search saved memories and, with permission, original conversation passages. Optional Search by meaning runs with a separate local search model.
- **See the evidence.** Required corrections stay with relevant recalled material, and changed or deleted sources invalidate affected pending work.

For a first conversation, **Build my starting map** offers six optional opening questions about your interests, priorities and projects. Preview them, choose what to share, and skip or stop whenever you like.

## More help getting a conversation going

Open **Conversation pace** and choose **Follow my lead**, **Share the lead** or **Help carry the conversation**. If you say, “I feel like chatting—pick something,” PCS is guided to choose a topic, offer a thought and follow your response.

Your preferred starting pace can be saved. **Quiet**, **Stay here** and **Another thread** remain temporary controls; current ideas expire and are not saved as memories. Quiet and Stay here pause topic planning until you explicitly resume. PCS does not schedule spoken openings during silence.

The default Companion instructions encourage accuracy, respectful disagreement and willingness to reconsider. You can edit them to suit the kind of help you want. Conversation quality depends on the model you choose.

## New: optional Jev conversation help

**Jev helps choose the next conversational angle.** When conversation carrying is active, your conversation model can propose up to three ideas. Jev selects one or chooses none; your model still writes the reply.

Jev is an optional TypeSafe cloud service. It starts **off**, requires a separate TypeSafe key, and works with Google and OpenAI. Local AI can use it only after you explicitly allow cloud selection.

While stopped, open **Settings → Optional tools → Jev · help choose the next direction**:

1. **Add your TypeSafe key.** Entering a key alone leaves Jev off.
2. **Choose what to share.** The default inputs are your latest complete statement, the conversation pace and the proposed ideas. Ideas can contain personal context already shared with your conversation model.
3. **Review and turn on.** Review the destination and information, approve the sharing, enable Jev and save for the next Start. Choose a carrying mode separately in Conversation pace.

An additional opt-in can include up to **four eligible recent messages**, within **6,000 characters and ten minutes**. Interrupted, stale or unconfirmed assistant output is excluded, so available context may be shorter. Conversation pace shows whether Jev ran, selected an idea, chose none or fell back, with available timing and usage information.

Jev has no independent access to your vault. It does not replace memory recall, write your memories or start conversations. With Local AI, approved Jev text leaves your computer while the local model continues generating the reply. Jev adds a service request and can add time and cost; it does not guarantee a better response. Qwen and focused research do not use it.

## Explore your visual memory map

[![PCS Continuity Map with demonstration constellations and supporting records.](https://raw.githubusercontent.com/PCS-PersonalContinuitySystem/PCS/main/assets/pcs-map-0.9.61.jpg)](https://raw.githubusercontent.com/PCS-PersonalContinuitySystem/PCS/main/assets/pcs-map-0.9.61.jpg)

*Interface example from PCS 0.9.61 using generated demonstration records. Newer Map controls are described below; this is not a live AI conversation.*

The **Continuity Map** gives personal knowledge management a visual starting point. Explore recurring wording across saved memories and notebooks, inspect the records behind a connection, and prepare a reviewed draft to continue the thought in Conversation.

- **Focus** follows one theme, with readable neighbor pages and access to the full neighborhood through List.
- **Constellations** shows connected groups; **Connections** reveals the current web.
- Back and Forward, named views, comparison layouts and your own connection notes help you return to a line of thought.
- Optional **Distinct saved content** counts reduce the visual weight of exact repeats with matching provenance. Date comparisons explain when they show a sample.

The Map works without starting an AI conversation. Its labels and counts describe saved material; they do not establish truth, personality traits or causes.

## Read, discuss and organize your documents

Use **Materials** to read supported PDFs, EPUBs, Office and OpenDocument files, tables, slides, subtitles, HTML and common text/code formats. You can discuss selected passages with your AI connection, prepare notes and collect references in notebooks.

| Task | What PCS offers |
| --- | --- |
| Find a passage | Keyword search, local section navigation, Find next and clear notices when changed files need refreshing. |
| Return to reading | Named bookmarks tied to the exact extraction, with Open at bookmark and retained reading position. |
| Listen and discuss | Read along with an available local browser/OS voice; prepare a passage and question for review before sending. |
| Keep Web evidence | Preview and retain supported public pages, feeds and PDF/EPUB sources; link exact saved snapshots to notebooks. |
| Build on your work | Keep goals, notes, lessons and source references together in notebooks. |
| Learn and plan | Use Research, Practice and local Calendar tools, with optional assistance and separate sharing controls. |

Extraction notices explain omitted content. Scanned documents need OCR elsewhere, and static Web capture does not handle every sign-in or script-rendered page. Source scripts, macros and spreadsheet formulas are not executed.

**Activity** adds context for a game, book, film, project or situation. Saved-memory approval stays separate from public research. Spoiler guidance can help, but cannot guarantee spoiler-free results. Optional proactive screen help and tutoring require their own setup and sharing review.

## Local AI assistant for Windows, or your chosen cloud connection

**Local on this PC** runs supported conversation and memory models on your hardware, with no cloud AI fallback. The recommended CUDA setup needs a compatible NVIDIA GPU. Settings guides the Gemma setup or a compatible Custom GGUF; custom files must pass compatibility checks. Typed use needs no speech pack. Optional listening, Windows/Kokoro voices and compatible OBS vision can be added separately.

For **offline AI conversations**, download the required Local components first, select Local for the roles you use, and keep online tools off. Brave lookup, Jev cloud selection and separately reviewed cloud preparation send their approved inputs outside your computer when enabled.

**Google and OpenAI** use your own API keys. Provider API access and charges are separate from consumer chat subscriptions. You can save named connections and switch while stopped.

**Alibaba Qwen** is an experimental voice-only connection with a smaller feature set. Radeon Vulkan text and Ubuntu browser/cloud operation remain previews requiring further target-hardware testing. macOS is not included in this release.

## Download and start

| Download | Contents |
| --- | --- |
| **[Windows application][windows]** | Complete PCS 0.9.71 application, launchers, bundled Python, dependencies and offline Help. |
| [Matching application source][source] | Source, tests, documentation and build support. |
| [SHA-256 checksums][checksums] | Verification values for both archives. |

Use the **Windows application ZIP** for normal setup. GitHub's automatic Source code archive contains this download repository, not the complete application.

1. Extract the complete ZIP into a fresh writable folder and keep its files together.
2. Open **Start PCS.exe**. First launch prepares its bundled Python environment offline; no system Python installation is needed.
3. Create a vault and keep the passphrase safe. Existing users should follow the included restore instructions before creating a replacement vault.
4. Set up a connection, review memory and sharing choices, and save. Try a short typed conversation before adding a microphone, Vision or optional tools.

The download includes `START_HERE.md`, `docs/GETTING_STARTED.md` and searchable offline Help. Manual reading, notebooks, Calendar and saved-record browsing do not require a running AI conversation.

## Privacy and backups

- **Your vault is encrypted; sharing is a separate decision.** Cloud tools receive the content allowed by their controls. Original Materials files and readable exports are outside vault encryption.
- **Don't save controls PCS saving.** It does not make a cloud conversation private from its provider. Corrections and deletion cannot retract information already disclosed or remove earlier backups.
- **Stop, Lock and Quit have different jobs.** Stop ends the conversation; Lock closes vault access; Quit PCS shuts down the host. Closing the browser tab alone can leave PCS running.
- **Back up before upgrading.** Keep an encrypted backup, your passphrase and the previous installation. Copy original Materials separately. Extract updates into a fresh folder and never run two copies against the same data folder.

Newly saved features can require a newer reader: retained Jev keys require **0.9.65**, Jev recent-context or Local-cloud options require **0.9.66**, and Web snapshot references in notebooks or retained notebook drafts require **0.9.71**. Opening PCS alone does not add those requirements; disabling a feature later does not remove them. Other existing vault requirements still apply. Keep a pre-upgrade backup if you need to return to an older version.

## Help, feedback and development

In-app and offline Help cover setup, reading, memory, privacy and recovery. Searches such as **stuck** or **not responding** lead to practical troubleshooting steps, and Back to results preserves your search.

PCS is under active development. AI replies, memories, transcription and research can be wrong. The 0.9.71 package passed **11,318 Python tests and 2,501 JavaScript tests**, with four platform skips, plus installation, lifecycle and browser checks. These checks do not establish live-provider quality, physical-device behavior or prolonged-session reliability.

For bugs, use [GitHub Issues][issues] or [Discord][discord]. Include the version, connection, steps and expected result. Review any bug report before sharing it; keep API keys, passphrases, launch tokens and private records out of public posts.

This repository hosts releases and project information. Application source is in the matching release ZIP; start with its `SOURCE_README.md` and `docs/developer/README.md`.

## Support and license

Optional contributions help fund PCS development. Provider charges are separate.

[Support PCS on Ko-fi][kofi]

PCS first-party code is licensed under **GPL-3.0-only**, without warranty. See [LICENSE](https://github.com/PCS-PersonalContinuitySystem/PCS/blob/main/LICENSE), [COPYRIGHT](https://github.com/PCS-PersonalContinuitySystem/PCS/blob/main/COPYRIGHT) and [third-party notices](https://github.com/PCS-PersonalContinuitySystem/PCS/blob/main/THIRD_PARTY.md). Bundled and separately downloaded components retain their own terms.

[windows]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.71/PCS-0.9.71-Windows-x64.zip
[source]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.71/PCS-0.9.71-Source.zip
[checksums]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.71/PCS-0.9.71-SHA256SUMS.txt
[release]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/tag/v0.9.71
[website]: https://pcs-personalcontinuitysystem.github.io/PCS-site/
[discord]: https://discord.com/invite/2ssCQhNgAN
[issues]: https://github.com/PCS-PersonalContinuitySystem/PCS/issues
[kofi]: https://ko-fi.com/pcssupport
