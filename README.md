# PCS - Your personal thinking space

**Room to think. Space to connect.**

Some thoughts need more than one conversation. PCS brings AI conversation, revisable memory, reading, notes and planning into a workspace you own. Bring an unfinished question, a difficult passage or an idea. Work on it, keep where you stopped, and return with a place to begin.

**Change the AI. Keep your continuity.** Choose a supported Local, Google, OpenAI, Meta, Claude, signed-in ChatGPT or OpenRouter connection. Your saved conversations, memories and notebooks stay in PCS when you change connections. Each model brings its own abilities; your workspace belongs to you.

**[Download for Windows][windows]** · [What's new][release] · [Website][website] · [Discord][discord] · [Report a bug][issues]

**Other platforms:** [Older experimental Linux x64][linux-experimental] · [Older experimental macOS for Apple silicon][mac-experimental] · [Archived platform downloads][older-platforms]

> **PCS 0.9.154 · Windows x64 · Under active development**
>
> Free and open source, with no PCS subscription or paid feature tiers. Provider API charges and any subscription used for ChatGPT sign-in are separate. Local models, AI runtimes and optional speech packs are separate downloads.

![PCS 0.9.139 Continuity Map focused on Harrow Point, a place named in saved observations about astrophotography, an astronomy club and a night-sky atlas, alongside the saved records behind it.](assets/pcs-continuity-map-0.9.139.png)

*One place, several ways back in. PCS 0.9.139 in the actual app interface, with fictional demonstration records in the Local memory format; not a live AI conversation. Harrow Point links three saved subjects because it is named in observations from each. The Map runs locally without a model request.*

## A place to work through things

| When you want to… | PCS gives you… |
| --- | --- |
| Think something through | Typed or spoken conversation, editable Companion direction and a choice of conversation pace. |
| Pick up an unfinished thought | An encrypted shelf of stopping points, next steps and pins, plus an editable draft when you return. |
| Understand what was remembered | Saved conversations and revisable memories, with original passages, corrections and sharing controls. |
| Follow how an idea changed | Links between exact memory revisions, settled marks and named lessons with supporting stories. |
| Find an unexpected connection | A Continuity Map of saved topics and the people, places and projects in them, with the records behind each connection and space for your own notes. |
| See how PCS's own view develops | Optional PCS Perspective tracks PCS's interests, reflections and open questions separately from your continuity and makes them available for inspection. |
| Read and learn | Materials readers, bookmarks, Read Along, Prepared notes, notebooks and Practice. |
| Find your work and plan ahead | A searchable Library and Calendar tasks, goals and events. |

Manual reading, notes, Calendar entries and saved-record browsing work without starting an AI conversation.

## Get started

### Windows

1. Download **[PCS-0.9.154-Windows-x64.zip][windows]** (51 MB) and extract the complete ZIP into a fresh writable folder.
2. Open **Start PCS.exe**. First launch prepares the bundled Python environment offline.
3. Choose **Set up PCS**. The guide walks through **Workspace, Connection, Sharing, Voice, Screen and Review**. Keep your vault passphrase safe. If you're moving an existing vault, follow the [upgrade steps below](#upgrading-and-backups).
4. Choose a connection, then review **Recommended continuity** or **Conversation only** and what you want to save and share. OpenRouter is included in Quick setup: enter its key, load the public catalogue and choose an exact model with tool support. **Free models only** and **Image-capable models only** filter the list without changing your choice. Claude uses its Console API key. For ChatGPT, finish Quick setup, then sign in, choose a model in **Settings → Connections**, and **Save settings**. Local setup guides you to its model and runtime files. Review your choices, including any optional Voice and Screen setup, then choose **Finish setup**.
5. Type a message and choose **Start & send**. The optional **Voice** step guides local listening and speech for Meta, Claude, ChatGPT, OpenRouter and Local AI. Use **Screen** to connect OBS Studio and choose the scene PCS may see. OpenRouter Vision needs an image-capable model; Finish checks the selected model's advertised tool/image support without generating a reply.
6. At a useful stopping point, choose **Keep a stopping point** and review what you want to retain.

Not ready to set up? **See a fictional example** on the welcome screen shows PCS with demonstration records, without adding anything to your vault.

The download includes getting-started and restore guides, plus searchable offline Help. A Settings task finder helps you locate controls. Keep the application files together: the launcher checks the package manifest. Use **Quit PCS** when finished; closing the browser tab alone can leave the application running.

### Older Linux and Mac experiments

Experimental builds are available on the **[previous release page, tagged 0.9.114][older-platforms]**:

| Platform | Download |
| --- | --- |
| **Linux x64** | [PCS 0.9.115 - experimental build][linux-experimental] (`.tar.gz`) |
| **macOS - Apple silicon (arm64)** | [PCS 0.9.114 - Experimental 1][mac-experimental] (`.zip`) |

These are archived experiments, not 0.9.154 ports. They do not include the current Windows features or its verification. Follow their own bundled platform instructions. Matching source archives are on the same [release page][older-platforms].

## Bring one unfinished thing

Start with a question, decision, passage or idea that matters to you. For example: *“I keep collecting ideas for this project. Help me choose one small thing to try next.”*

Choose **Follow my lead**, **Think with me** or **Take the lead**. Think with me is guided to develop one manageable thought at a time and leave room for your response. **Quiet for now** and **Stay here** pause topic planning until you explicitly resume. Companion instructions are editable.

The default **Companion direction** now favors calm, warm and independent replies, proportionate praise, and fewer routine follow-up questions. Custom directions are preserved. **How often PCS offers new angles** and **Conversation pace** separately control initiative; the direction change does not reset those choices.

If you prefer a broader start, **Build my starting map** offers six optional opening questions. Preview the prompt, choose what to share, and skip or stop whenever you want. Your saving and learning choices still apply.

### Leave a stopping point

Keep a title, where you stopped and an optional next step. Review the note before saving it to your encrypted shelf. Pin it, edit it, mark it resolved, reopen it or delete it when you choose.

On a later visit, unlock your vault and choose **Load saved threads**. Review the suggested stopping point and its sources, then choose **Review & continue** to prepare an editable draft. You decide whether to send it. Loading the return card reads local records without a model request, and existing unsent text is protected.

A resumed thought stays available across Conversation, Materials, Continuity and Calendar. **Explore in Map** carries it into the Map as a temporary reminder.

## Follow a connection back to your own words

The **Continuity Map** opens on **Constellations**, with readable labels based on saved topics. Follow a theme into **Focus**, explore **All links**, or use **List**. The trail above the Map lets you revisit earlier steps.

- **Open the evidence.** Select a connection to inspect the saved records behind it in one panel.
- **Compare two themes.** **Compare with…** shows a route through shared records and themes.
- **Keep what matters.** Add a connection note, leave a landmark in your own words, or choose **Continue in Conversation**.
- **Explore at your own pace.** Try **Discover a connection**, or browse freely. Filters and coverage are under **Map settings**; saved views and connection notes are under **Views & notes**.

Themes come from **saved labels and repeated wording** by default, preserving phrases such as “Bread making.” **Saved labels only** is available under **Map settings**. Local memory keeps one account per subject and adds later observations to it, so the Map counts each current observation: a subject you return to often appears larger, and the people, places and projects named in it become linked themes. A name that appears under two subjects connects them. Monthly save patterns show when themes have been saved or edited more often.

The Map runs on your PC without calling a model. A line means two themes occur in the same saved record or observation. It does not establish agreement, cause or a personality trait. Open the evidence and decide what the connection means to you. Names are recognised by their capital letters, so a name written in lowercase is missed.

Whole-archive indexing supports up to **50,000 memories** and **250 themes**. The encrypted index follows saves, corrections and forgetting. If you already use it, choose **Map settings → Coverage → Finish indexing** after upgrading to refresh it locally.

## Memory you can inspect and revise

Saving conversation text and allowing memory formation are separate choices. With learning enabled, PCS can create model-written accounts linked to original passages. Inspect the evidence, review earlier wording, correct an account in ordinary language or choose **Forget**. Your words, your corrections and model interpretations remain distinguishable.

When you ask PCS to remember something, the request gets its own check, and the result card shows whether the save was confirmed, did not succeed or left a record unchanged. Correction screens show that saving your wording and rebuilding semantic search are separate steps; saved corrections keep their history and current status.

Recall follows your sharing permissions and keeps relevant corrections attached. It can bring back the original conversation passages behind a saved account, including the evidence for a correction. Recalled material labels which words were yours, which were the assistant's and which accounts you edited, so the model can tell them apart. Local checks whether a question needs saved context before replying. A blocked or failed lookup is distinguished from a completed search with no match. Memories and AI answers can still be incomplete or mistaken.

Open a memory and choose **Settled, links & lessons** to:

- Link memories to record how one idea developed from another.
- Mark an exact revision settled as your current word on its subject. A correction retires the mark until you review the new wording.
- Keep a named lesson with your story, takeaway and supporting memories.

Links and lessons retain the revisions you reviewed and identify changed or unavailable references. Forgetting a memory removes its revisions and updates dependent records.

**Memory can follow your conversation connection.** Google, OpenAI, Meta, Claude, signed-in ChatGPT, OpenRouter and Local support their permitted memory workflows within the selected model's capabilities. OpenRouter can use its own key and explicit model for learning, Remember requests, corrections and recall; another provider is not required. Optional helper choices remain explicit, and PCS does not automatically switch providers after a failure.

**Help notice relevant memories in conversation** is included in **Recommended continuity** and can be changed under **Settings → Memory & sharing**. It requires memory-sharing permission. Supported routes can use a compact overview or matching cues to help find saved context. A cue sent to a cloud provider shares that information; hints do not guarantee a relevant memory will be found.

## PCS Perspective (optional)

PCS Perspective keeps PCS's developing interests, reflections and open questions separate from your own continuity, in the same encrypted vault. **Recommended continuity** enables it with independent interests for new vaults. Open **PCS Perspective** in Conversation to review its choices and records.

- Inspect wording, supporting references, uncertainty, model authorship and revision history, or explore its dedicated Map.
- Carry current perspectives and unfinished inquiries between supported models.
- Allow independent exploration in the background with microphone input **on**. What you say interrupts that step; a completed thought can wait for a later quiet moment.
- Allow focused thinking pauses with microphone input **off** when PCS requests one or you choose **Explore now**. Use **Return to conversation** to interrupt; PCS cannot hear a spoken interruption while the microphone is off. When a pause PCS requested ends, its result goes back to the conversation so PCS can say what it concluded.

Exploration uses the displayed Preparation model and can make extra requests. It does not independently browse the web or read Materials. Relevant perspectives may also reach your conversation model under the feature's sharing notice. The contributions are optional and bounded; PCS may have nothing useful to say, or may still choose an awkward moment.

This is distinct from **Explore another perspective**, where you explicitly select saved memories for a separate reflection. Perspective records make model interpretations inspectable; they do not establish subjective experience.

## Read, discuss and learn

**Materials** supports readable PDFs, EPUBs, Office and OpenDocument files, tables, slides, subtitles, HTML and common text/code formats, with file-format tiles, reading-time estimates and highlighted passage search. Find a passage, keep a bookmark, listen through an available local voice, or review an excerpt before sharing it with your selected model.

**Prepared notes** support longer reading projects. **Prepare book** works through an explicitly approved sequence and saves checkpoints; **Resume** lets you review the next scope. Notebooks hold notes, goals, lessons and source references. Practice can retain submitted answers and assessments when enabled.

You can also attach or drop a UTF-8 `.txt` or `.md` file and review it before choosing **Use in this chat**, **Keep for later**, or **Save reviewed text in Materials**. A Materials copy is an ordinary file outside the encrypted vault; back it up separately. Scanned documents need OCR elsewhere, and some Web pages cannot be captured.

Reviewed quotations can be added to a Notebook, lesson or Calendar entry while preserving their wording and authorship. Keeping a thought or creating a Calendar entry does not schedule automatic follow-ups or reminder delivery.

Optional **Explore connections** in the Library lets you select records, add a question and review which excerpts may be shared with Jev. This trial requires a TypeSafe key and permission for each request. Its suggestions do not automatically create memories or change the Map.

## Choose where the AI runs

| Connection | Access and model choice | Listening and spoken replies |
| --- | --- | --- |
| **Local on this PC** | Compatible hardware, supported model and verified runtime. Recommended Gemma/CUDA needs a compatible NVIDIA GPU. | Optional local listening; Windows or Kokoro speech. |
| **Google API** | Google API key and a compatible Live model. Review the Personal/Public content profile for your project's terms. | Native provider audio on the supported connection. |
| **OpenAI API** | OpenAI API key and a compatible Realtime model. API billing is separate from ChatGPT subscriptions. | Native provider audio on the supported connection. |
| **Meta** | Meta API key and supported Standard model. | Optional local listening and speech. |
| **Claude API** | Anthropic Console API key and a compatible model. | Optional local listening and speech. |
| **ChatGPT sign-in** | Eligible signed-in account and an available model; no API key. | Optional local listening and speech. |
| **OpenRouter** | OpenRouter API key and an explicit model with PCS tool support; image capability is needed for Vision. | Optional local listening and speech. |

Typed cloud conversation needs no Local language model or speech pack. Cloud Vision sends approved OBS images; Local Vision also needs the matching image projector.

**ChatGPT sign-in is separate from the OpenAI API connection.** It does not import ChatGPT history, provide unlimited usage or silently fall back to API billing. Claude API uses its Console key, rather than a Claude subscription login.

**OpenRouter's native PCS features use OpenRouter.** Memory, preparation, notebooks, Practice, Calendar, topic organization, PCS Perspective, web research and Wikipedia Study are available within the chosen model's capabilities and your permissions. Memory and preparation can follow that connection; optional OpenRouter Memory and Research model/key overrides let you choose another account or model within the same provider. Free models have availability and usage limits, and web-search plugin charges can apply even to free-model inference.

Feature coverage varies by route, model and account. Only Google and OpenAI provide PCS's cloud embedding-index maintenance. Meta, Claude, ChatGPT and OpenRouter retain word/navigation recall and can use the separate optional local semantic index. Preparation and memory review can make additional model requests.

**Help notice relevant memories** can share a bounded startup overview or matching cues on supported routes. OpenRouter startup directory/map packets require Vision **off** and a known fitting model budget; image-containing requests omit optional matching cues. Ordinary permitted recall remains available. These previews help navigation, not proof that every relevant memory was found.

Local conversation and memory have no automatic cloud AI fallback. Download the components first and leave online lookups, cloud preparation and separately reviewed TypeSafe features off for offline use. Local web search needs a Brave Search key; Wikipedia Study does not need that key, but still sends public online requests. Local + Jev and Library exploration send their separately reviewed information to TypeSafe.

The direct experimental Alibaba Qwen connection is retired. Existing records remain readable, and Qwen-family models in the OpenRouter catalogue are separate choices.

### Local context and voices

Recommended Local on NVIDIA CUDA defaults to a **128K context window**, with selectable windows up to **256K**. Hardware, model and enabled features determine capacity and speed. Long Local sessions compact working context while retaining recent complete exchanges; saved originals remain unchanged. Local helpers can also handle Study, saving web material, memory-thread suggestions and supported visual observations.

Typed Local conversation needs no listening pack. Optional English microphone input, Windows or Kokoro speech, local semantic search and compatible OBS Vision can be added separately.

**Kokoro remains the recommended local voice for everyday use.** Meta, Claude, ChatGPT and OpenRouter can also try **KittenTTS 2 on CPU or NVIDIA GPU**, both experimental. Settings offers verified runtime and model downloads and a timed voice sample. Kitten is substantially heavier than Kokoro, and CPU generation can be slow. Review its model license before downloading. **Powered by KittenML.** Local AI conversations continue to use Windows or Kokoro voices.

The current 0.9.154 application download is Windows x64. Older Linux and Mac experiments are listed under **Get started** above.

## What's new in 0.9.154?

Since the previous public release, 0.9.146:

- **OpenRouter throughout PCS:** guided key and explicit model selection, optional local voice and image-capable Vision, plus native memory and other PCS tools.
- **Calmer default Companion direction:** less routine praise and follow-up, with custom directions preserved.
- **Steadier Perspective behavior:** independent thinking keeps the microphone on, completed thoughts can wait for a quiet moment, and requested thinking pauses return their result.
- **Automatic activity following removed:** permitted saved context no longer waits for model classification. Manual Activity details and approvals remain available.
- **Local and reliability repairs:** Custom GGUF weights can fit across GPU/system RAM; fixes cover startup continuity, older vaults, Notebook drafts, Calendar, research, writer attribution, playback and cancellation.
- **Current Help:** refreshed provider/setup guidance, separate Perspective controls and clearer sharing and search-index limits.

See the **[0.9.154 release notes][release]** for the full changes, validation scope and upgrade guidance.

## Your data and sharing choices

- Saved continuity lives in your local encrypted vault. Original Materials files, imported text copies and readable exports are outside that encryption.
- Cloud features receive information allowed by their controls. With OpenRouter, that includes OpenRouter and the selected upstream model provider. **Don't save** controls PCS retention; it does not prevent the selected service from receiving the conversation. Provider privacy, retention and billing terms still apply.
- Corrections and forgetting affect PCS records and dependent saved work. They cannot retract information already disclosed or erase earlier backups.
- PCS cannot recover a lost vault passphrase. Changing it affects the working vault; existing backups keep their original passphrases.
- **Stop**, **Lock** and **Quit PCS** have separate purposes: end the connection, close vault access, or shut down the application.

## Upgrading and backups

Save your work and make an encrypted backup. Choose **Quit PCS** and wait for shutdown before moving the stopped data folder, including any custom data location. Copy original Materials separately; the encrypted vault does not contain those files.

Extract the complete Windows ZIP into a fresh writable folder. Follow the **Backup & restore** guide bundled with the release to copy or restore your vault, keeping separate data folders for separate installations. Open **Start PCS.exe**, unlock with your passphrase and inspect your records. Keep the previous installation and pre-upgrade backup until you have checked the update.

**Newly saved features can raise the vault's minimum supported PCS version.** OpenRouter connection data requires **0.9.151 or later**; OpenRouter helper data and Practice assessments exceeding the former 4 KiB record limit require **0.9.152 or later**. Earlier feature requirements still apply. Opening the app alone does not activate these requirements, and deleting newer records does not lower a recorded requirement. Use **Check backup** to see the copy's actual reader requirement.

A saved direct-Qwen connection must be replaced explicitly. **Automatically follow my current activity** and its classification tools are removed; manual activity controls remain. Jev needs a fresh approval if its earlier review included automatic activity following. The old proactive-help controls also remain retired.

Existing settings are preserved apart from retired controls and recognized factory Companion direction wording. New Recommended defaults apply to new vaults; review optional features in your own setup.

## Feedback, source and license

PCS is under active development. AI replies, memories, transcription and research can be wrong. Share feedback through [GitHub Issues][issues] or [Discord][discord]. Include your PCS version, connection and reproduction steps. Review diagnostics before sharing and remove keys, passphrases, launch tokens and personal records.

The 0.9.154 final source passed **2,513 Python checks** with **3 skips** and **3,486 JavaScript checks**. Live OpenRouter checks exercised corrected-memory recall/read, Notebook review/save/reopen and the complete Calendar journey with fictional data and a selected model. These are targeted checks, not qualification of every model, physical audio/OBS device or a fresh installer launch. The tested Gemma 4 26B Custom GGUF still showed long-prompt crashes; the Recommended model remains the starting choice.

This repository hosts project information and downloads. **[PCS-0.9.154-Source.zip][source]** contains the application source, tests and build support. GitHub's automatic **Source code** archive contains this download repository.

Use **[PCS-0.9.154-SHA256SUMS.txt][checksums]** to verify the release archives. Earlier versions are under [Releases][releases].

PCS first-party code is licensed under **GPL-3.0-only**, without warranty. Third-party components retain their own terms. See [LICENSE][license], [COPYRIGHT][copyright] and [third-party notices][third-party]. Optional contributions through [Ko-fi][kofi] help support development.

[windows]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.154/PCS-0.9.154-Windows-x64.zip
[source]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.154/PCS-0.9.154-Source.zip
[checksums]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.154/PCS-0.9.154-SHA256SUMS.txt
[release]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/tag/v0.9.154
[releases]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases
[older-platforms]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/tag/v0.9.114
[linux-experimental]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.114/PCS-0.9.115-Linux-x64-Experimental.tar.gz
[mac-experimental]: https://github.com/PCS-PersonalContinuitySystem/PCS/releases/download/v0.9.114/PCS-0.9.114-macOS-arm64-Experimental-1.zip
[website]: https://pcs-personalcontinuitysystem.github.io/PCS-site/
[discord]: https://discord.com/invite/2ssCQhNgAN
[issues]: https://github.com/PCS-PersonalContinuitySystem/PCS/issues
[license]: https://github.com/PCS-PersonalContinuitySystem/PCS/blob/main/LICENSE
[copyright]: https://github.com/PCS-PersonalContinuitySystem/PCS/blob/main/COPYRIGHT
[third-party]: https://github.com/PCS-PersonalContinuitySystem/PCS/blob/main/THIRD_PARTY.md
[kofi]: https://ko-fi.com/pcssupport

