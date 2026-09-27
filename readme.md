# ⚙️ ORION
### The Ultimate Cross-Platform Personal AI Assistant — By ShayanMitra


A real-time voice AI that can hear, see, speak, and control your computer — on any OS. Supports Windows, macOS, and Linux. Built on the Gemini Live API for native audio streaming, delivering zero subscriptions and total digital autonomy.

---

## ✨ Overview

**ORION is the release where ATLAS gets a face.** A holographic head sits at the centre of the HUD and **speaks your assistant's words with real lip-sync** — not a jaw flapping to the volume meter, but actual mouth shapes: lips closing on *m*, *b*, *p*, spreading on *i*, rounding on *u*. Brows ride the sentence, the eyes flick between fixation points, and it blinks. Turn the sound down and you can follow roughly what it just said.

It ships as **zero extra dependencies and one 25 KB asset**. The face is real measured human geometry; everything else — the skull, the rig, the lighting — is generated at startup and drawn in software, so it looks identical on a gaming rig and a 2013 laptop, with no GPU driver in the loop.

The face is also the fastest status indicator in the app: it looks away while thinking, meets your eyes while listening, and lets its lids fall while asleep.

Underneath, Orion rebuilt how the assistant knows itself — what it is, what machine it runs on, what it can do and, new, **what it cannot do** — all assembled from the live system at session start rather than written into a prompt that goes stale.

It's not just an assistant — it's an extension of your digital life.

---

## 🚀 Capabilities

### Core Features
| Feature | Description |
|---|---|
| 🧑‍🎤 Holographic Avatar | An animated human head in the HUD — real facial geometry, lit and drawn in software, no GPU or extra packages |
| 👄 Real Lip-Sync | ~50 mouth shapes a second from the audio's formants **and** the transcript — closures, spreads and rounds, not a volume meter |
| 🌍 Language-Free Mouth | Articulation is derived by Unicode reduction, so Latin, Cyrillic and Greek scripts all work from one rule set — and scripts that hide pronunciation fall back cleanly |
| 🙂 Facial Acting | Brows track the phrase, gaze saccades between fixations, natural blinking, a small nod on stressed syllables |
| 😐 Face as Status | Looks away while thinking, meets your eyes while listening, lids fall while asleep, glances down at new content |
| 🎚️ Push-to-Talk | Hold **Ctrl+Space** and the mic opens — closed the rest of the time. Truly global on Windows, window-scoped elsewhere |
| 🔇 Self-Echo Guard | Never answers its own last sentence: the tail of its own voice is recognised and dropped without muting you |
| 🪪 Runtime Self-Knowledge | Name, OS, abilities **and limits** are generated from the live system each session — rename it or add a plugin and it knows |
| 🎙️ Wake Word | Local **"Hey Atlas"** detection — sleeps until called, auto-sleeps after 2 min of silence, and never streams audio while asleep |
| ⚡ Instant Acknowledgment | Speaks a short, context-aware reply in **your language** the instant a longer task starts — no more silent waiting |
| 🚀 Faster Live Engine | Runs on **Gemini 3.1 Flash Live** — roughly 2× faster time-to-first-word than the previous model |
| 🧩 Self-Describing Skills | Actions and plugins share one shape (`TOOL` / `PLUGIN` dict + `run()`), auto-discovered at launch — adding a skill is a single file |
| 🧠 Recallable Memory | No size limit and nothing silently forgotten — the prompt carries what fits, the rest is looked up on demand from a local search |
| 👁️ Memory Panel | See every fact ATLAS has stored about you, when it learned it, and delete any of it in one click |
| ↩️ Undo | Take back what the assistant did — files it moved, renamed, created or wrote, and settings it changed |
| ⚠️ Real Confirmation | Shutdown, restart and WiFi wait for a button **you** press — the model cannot confirm its own irreversible actions |
| 🎧 Audio Device Picker | Choose the microphone and speakers by name, filtered to the short list your OS shows — and measured, so every entry actually works |
| 🔗 Session Continuity | A dropped connection, a voice change or a device change no longer wipes the conversation |
| 🧩 Plugin System | Drop a single `.py` file into `plugins/` — ATLAS learns a new skill on next launch |
| 🎙️ Real-time Voice | Ultra-low latency conversation in any language via Gemini Live API |
| 🎨 Live Theming | Recolour the entire HUD from a hue wheel or hex — the avatar retints with it |
| 〰️ Reactive HUD | Waveform pulses to real audio — your mic while listening, ATLAS while speaking |
| 🎙️ Voice Picker | Choose from 5 native Gemini voices and switch live from the UI — no restart |
| ♾️ Unlimited Sessions | Sliding-window context compression — one conversation can last for hours |
| 🖥️ System Control | Launch apps, adjust volume/brightness, WiFi, shortcuts, power — all by voice |
| 🧩 Autonomous Tasks | High-level planning for complex multi-step goals via agent mode |
| 👁️ Visual Awareness | Screen capture and webcam vision piped into your main Gemini session, labelled by source |
| 🧠 Persistent Memory | Deeply remembers projects, preferences, and personal context across sessions |
| ⌨️ Hybrid Input | Seamlessly switch between keyboard typing and voice commands |
| 🌅 Morning Briefing | On first boot: greets you, reads the time, recaps yesterday, and fetches live news |
| 🔔 Proactive 2.0 | Time-aware, context-aware check-ins — knows the time of day, your projects, and what you've been discussing |
| 🗓️ Session Memory | Summarises each conversation and mentions it naturally next morning — consumed after use, never repeats |
| 👁️‍🗨️ Background Monitoring | User-configured topic watching — checks for new headlines once a day and alerts naturally |
| 📊 Hardware Monitoring | Continuous CPU, RAM, GPU and temperature telemetry with localized voice alerts |
| 🌤️ Weather Report | Live weather data for your city, personalized from memory |
| 🗺️ Dynamic Content Panel | Scrollable display layer beneath the HUD that renders web results, news, and search data |
| 🔍 Multi-Mode Web Search | `news` / `research` / `price` / `compare` / `search` — Gemini Grounded first, DDG fallback |
| ⏰ Smart Reminders | OS-native scheduled notifications (Windows Task Scheduler / macOS LaunchAgent / Linux systemd) |
| ✈️ Flight Finder | Live flight price and availability lookup |
| 🎮 Game Updater | Checks and triggers game updates on Steam and Epic Games on demand |
| 📂 File Processor | Read, summarize, and answer questions about local files |
| 💻 Code Helper | Inline code review, debugging, and generation |
| 🌐 Browser Control | Open URLs, navigate tabs, and interact with the browser by voice |
| 📨 Send Message | Compose and send messages through WhatsApp, Telegram, and more |
| 🎬 YouTube Control | Search, play, and control YouTube playback by voice |
| 🖱️ Desktop Control | Taskbar, window management, and desktop-level operations |
| 🧑‍💻 Silent Language Memory | Detects spoken language on first use — all future sessions adapt automatically |
| 📱 Remote Dashboard | Control the assistant from your phone via QR code pairing |
| ⚡ Auto-Start on Boot | Registers with the OS startup system (registry / LaunchAgent / .desktop) |
| 📋 Clipboard Intelligence | Copy any text → floating panel with Translate / Summarise / Explain / Fix |
| 🪪 Assistant Customization | Change the assistant name, your name, voice, and colour from the UI — takes effect immediately |

---

## 🆕 What's New in Orion

No hardcoded language, no GPU requirement, no new dependencies — identical on Windows, macOS and Linux.

### The face

#### 🧑‍🎤 A real head, rendered in software
The centre of the HUD is now an animated human head. Its face is **real measured human geometry** — MediaPipe's canonical face model, with actual eyelids, nostrils, lips and cheekbones. The skull, neck, jaw rig and lip rig are generated around it at startup, and the whole thing is lit and drawn with **QPainter**, which means:

* **no new dependencies** — it runs on the PyQt6 and numpy the app already needed;
* **no OpenGL, no shaders, no GPU driver** to disagree with you — a VM, a remote desktop session and an old integrated laptop all render the same picture;
* **one 25 KB asset**, and everything else is a formula.

It breathes, sways, blinks, and retints instantly when you change the HUD colour.

#### 👄 Lip-sync you can actually read
The old mouth opened to the volume meter, five times a second. The new one produces **~50 mouth shapes per second** from two sources at once:

* **the audio** — a formant read of each 20 ms slice gives openness (how far the jaw drops) and width (spread for *i* and *e*, rounded for *u* and *o*). This is physics, so it is language-independent by construction.
* **the transcript** — because no spectrum can tell you the lips are *closed*. /m/, /b/ and /p/ look identical to a filter bank and completely different on a face. The words supply the shape; the audio supplies the timing and the force.

#### 🌍 One rule set, every alphabet
There is no per-language table. Every character is reduced to a bare Latin letter — Unicode decomposition strips accents (é, ü, ş, ğ, ế, ñ, å…), and Cyrillic and Greek transliterate — then articulation is looked up on the sound.

**Turkish, English, Hindi, Bengali, German, French, Spanish, Polish, Vietnamese, Czech, Russian, Ukrainian and Greek all work from the same twenty-odd rules.** Scripts whose spelling doesn't reveal pronunciation (Arabic, Chinese, Japanese, Hindi, Korean, Hebrew, Thai) are detected automatically and the mouth runs on the audio-only shape — less detail, never wrong. Adding a language costs nothing, because there is nothing to add.

#### 🙂 It acts while it talks
Brows ride the *phrase*, not the syllable, with a slow asymmetry between them. The eyes make real saccades between fixation points, more often while speaking. It blinks. Loud syllables tip the head. Everything relaxes to neutral in silence — and the mouth **only** moves for the assistant's own voice, never for yours.

#### ◉ Two HUDs, one toggle
Not everyone wants a face looking back at them. ⚙ → **HUD** swaps the centrepiece between the animated head and a **reactor core** — a gauge ring, three arcs that turn at a rate the state sets, a spectrum ring driven by the real audio level, and a core that brightens with the voice. Both render in the same software painter and cost the same; the choice is taste, and it survives a restart.

Nothing on the core moves for decoration. The rings speed up when ATLAS is thinking, the spikes are the actual waveform, and the colour is the state — the same language the face speaks, without the face.

#### 🗣️ It answers before it works
Some replies used to open with three or four seconds of silence: not because a tool was slow, but because ATLAS was still *writing the tool call* — a set of quiz questions, the findings from a contract. The tool was instant; the composing was not, and from the user's side those are the same thing.

The rule is now about the silence rather than the tool: if a gap would form, say one sentence naming what you are starting, then do it. It applies to anything that takes a moment to run **or** a moment to write, without a list of which tools those are.

#### 😐 The face is a status light
You read a gaze faster than you read a word, so the head tells you what the assistant is doing before it says anything. It **looks away and holds it while thinking** — brows drawn down, blinking suppressed, the way concentration actually looks — **meets your eyes while listening**, and **lets its lids fall while asleep**. When something appears in the content panel below, it **glances down at it**: a wordless "that landed".

### Talking to it

#### 🎚️ Push-to-talk
Wake word is hands-free, but in a meeting or a noisy room a key is faster and never mishears. Turn on **⚙ → PUSH-TO-TALK** and the microphone stays **closed** until you hold **Ctrl+Space** — nothing leaves the machine while you are not holding it. Holding the chord also wakes the assistant, so it doubles as a silent alternative to saying the wake word.

On **Windows** the chord is genuinely global: it works while any other application has focus, implemented by polling two virtual-key codes thirty times a second, with **no new dependency** and no message loop. On **macOS and Linux** there is no dependency-free way to read global key state, so the chord is bound inside the window instead — and the app **says so in the log** rather than pretending otherwise.

#### 🔇 It no longer talks itself into replying
Writing audio to a device returns when the buffer *accepts* the sound, not when the speaker has finished with it — so for a moment after a reply "ends", it is still in the room. Streaming the microphone during that gap is how an assistant hears its own last sentence, decides it was addressed, and answers itself.

ORION holds a guard open across that gap, sized from the **device's own reported latency** rather than a guessed constant, so a machine with a large audio buffer gets a longer guard and one with a small buffer is not penalised. The microphone is **not muted** during it: both streams are reduced to band energies and as much of what was just played is subtracted from the microphone as fits, so only your assistant's own voice is dropped — replying the instant it stops still works.

> Interrupting it mid-sentence by voice is built on the same machinery and is deliberately **switched off** in this release. It depends too much on the listener's room to ship without testing on real hardware.

### How it understands itself

#### 🪪 It knows what it is, and what it isn't
Who it is, what machine it runs on, what it can do and **what it cannot do** are assembled from the live system at session start — the configured name, the real OS, the tools actually discovered. Install a plugin and it knows it gained an ability; remove one and it stops claiming it.

The **limits** half is the important one: it knows its sight is a single frame on demand rather than a live feed, that it acts on this machine only, and that anything outside its tool list should be stated plainly instead of improvised.

All prompt wording lives in `core/prompt.txt` with `{tokens}` the app fills in — so you can rewrite the personality without touching Python, and a stray brace in your own wording can't break startup.

### 🩹 Fixes
* Answers were sometimes **logged and spoken twice** — the Live API re-sends the tail of a transcript across the several turn-completes a tool call produces. Now de-duplicated at both the chunk and the flush level.
* Asking ATLAS to look at the screen produced **two different answers** — the flow made it speak once *before* the image arrived, so it improvised, and again after. The frame is now attached to the same exchange as its tool result: one turn, one answer, one fewer round trip.
* Screen captures were **unlabelled**, so a screenshot of this app — which has a face in the middle of it — could be read as a photo of the user. Images now carry their source.
* On a non-UTF-8 console (cp1254, cp1251, cp932…) the emoji in the status lines **crashed the session on startup**. Streams are reconfigured at launch, so it starts the same way in every locale.
* The HUD kept rendering the avatar **while the window was hidden or minimised**. It now stops, and resumes mid-motion rather than snapping.
* Activity-log lines were fixed amber and ignored the theme; they now follow the accent colour.
* Dependencies had no upper bounds, so the next major release of any of them would break every fresh clone. The load-bearing ones are now capped.
* The mouth **ran ahead of the words, then behind them**. Three separate faults compounded: each 200 ms of audio only produced 160 ms of mouth shapes, every new batch overwrote the previous one instead of continuing it, and the schedule was anchored to the moment audio was *handed to the device* rather than the moment it becomes *audible*. The mouth now follows one continuous playback clock — measured at **15 ms** of timing error whether the sound card buffers 100 ms or 500 ms.
* The jaw was driven by the **waveform meter**, which deliberately holds peaks so the bars don't flicker. That hold spanned exactly the consonants the mouth needed to close on. It now reads the audio's own 20 ms levels, so the gaps between words are real gaps.
* Mouth timing was measured in **frames rather than seconds**, so the same constants meant three different mouths at 60, 30 and 20 fps, and a closure shorter than one frame could vanish entirely. Timing is now in seconds and the mouth is stepped once per 20 ms of audio, not once per repaint.
* The **brows barely moved** — 6 px of travel on a 250 px head, because the rig weights halved an already small constant. Derived from the anatomy instead: 19 px.
* The activity log opened with **a dozen lines of plumbing** — one per plugin loaded, plus wake-word and briefing status. The console still carries the full boot transcript; the log now shows your conversation, state changes and anything you have to act on, and nothing else.

> Built on the Orion OI–OIII foundation: the **🧩 Plugin System**, **♾️ Unlimited Sessions**, **🎨 Live Theming**, **🎙️ Wake Word** and **🧩 Self-Describing Skills** are all still here.

---

## 🔄 The Foundation Update — in every Mark from LII

These four landed across **Orion OII, OIII, OIV and OV at the same time**, after each of those releases had already shipped. They are not what any one of those versions originally introduced; they are the floor all of them now stand on, so moving up a Mark never costs you something the one below it had.

No new dependencies. No bundled asset files. No hardcoded language, and nothing that assumes one operating system.

### 🧠 A memory that actually remembers

The store was capped at **2,200 characters — the whole memory, not per entry** — because all of it was pasted into the system prompt on every connect, so growing the memory grew every request. When it filled, the oldest entries were deleted and one line was printed to a console nobody reads. An assistant advertised as remembering "projects, preferences and personal context" was in practice a two-page notepad that quietly forgot your sister's name after a few weeks.

Storage and prompt budget are now separate problems:

* **Nothing is deleted.** The cap is a runaway guard normal use never approaches, and if it is ever hit it says so in the activity log instead of on stdout.
* **The prompt carries a core, not a dump.** Identity in full, then the most recently updated facts, budgeted — measured at **971 characters on a memory holding 62 stored facts.** That is *smaller* than the old whole-store cap, so sessions now connect with fewer tokens than before.
* **The rest is fetched on demand.** A `recall_memory` tool searches the full store locally — no network, no second model, well under a millisecond.

The part that is easy to get wrong: **a model cannot look something up if it doesn't know the thing exists.** So the prompt also carries an **index of the keys** it had no room for. Without it, "who is Ayşe?" gets "I don't know" while `ayse_sister` sits on disk unread. That index interleaves categories rather than sorting by recency — sorted like the core, a memory with forty preferences pushed the one entry the index existed for off the end.

⚙ → **🧠 MEMORY** shows every stored fact, when it was learned, and a ✕ to forget it. Everything stays in `memory/long_term.json` on your machine.

### ↩️ Undo — it can take back what it did

ATLAS moves files, renames them, writes to them and changes your settings. None of that had a way back; if it misheard you, the only remedy was to fix it by hand.

Say **"undo"** — in any language — and it reverses its own last action:

| | |
|---|---|
| **Files** | move · rename · create · copy · write · delete · organize desktop |
| **Settings** | volume · brightness · dark mode |

Three things it deliberately does *not* do:

* **It does not guess.** Settings undo reads the current value *before* changing it. Where a platform won't report that value, nothing is registered — an undo that restores a guess is worse than no undo.
* **It does not hoard.** Undoing a write means keeping the old contents in memory, so files over 1 MB are excluded and it says so rather than holding a 200 MB log for the session.
* **It does not delete your files to undo a copy.** The reverse of a copy is removing the copy; the reverse of "create a folder" is removing it *only while it's still empty*.

`organize_desktop` gets special treatment — one command that moves dozens of files, which made it the least reversible thing the assistant could do. It journals every move and puts all of them back in one go, cleaning up the folders it created if they're still empty.

**Undo costs nothing at runtime.** It appends a closure to a list; nothing in it runs unless you ask.

### ⚠️ A confirmation the model can't forge

The old gate read like this:

```python
if action in _DANGEROUS_ACTIONS:            # {"restart", "shutdown"}
    confirmed = str(params.get("confirmed", "")).lower()
```

`confirmed` is a **tool parameter, which means the model fills it in.** Nothing stopped it sending `confirmed=yes` on the first call and nothing checked that a human was ever involved. It was a convention, not a gate. And its coverage was two actions — so `toggle_wifi`, which cuts the assistant's own connection to the Live API and therefore *cannot be asked to undo itself*, went through with no gate at all.

The token is now issued by the interface. Shutdown, restart and WiFi put a banner on the HUD and **return immediately**; the action runs only if you press CONFIRM. Nothing blocks — ATLAS keeps talking while the banner is up — so this is **cheaper than the old gate**, which burned two tool round trips on every power command.

> The split between the two mechanisms is about reversibility, not about how alarming a word sounds. Anything undoable is done at once; only the genuinely irreversible asks. An assistant that checks with you before turning the volume down is one you stop talking to.

### 🎧 It finally asks which microphone

Both audio streams opened with no device argument at all, so they always took whatever the OS called "default" — and on Windows that *moves on its own* the moment you plug a headset in. "ATLAS can't hear me" almost always meant "ATLAS is listening to the webcam".

⚙ → **🎧 AUDIO DEVICES** lets you pick the microphone and the speakers by name. Two things matter more than the dropdown:

**The list is short.** `query_devices()` returns one entry per *device × host API*, not per device — measured on an ordinary Windows machine, **41 entries for what the sound settings show as 4 microphones and 4 speakers.** The same microphone appears four times, under MME, DirectSound, WASAPI and WDM-KS, with nothing to say which is which. That is not a choice, it's a quiz. The picker takes one host API per direction, drops the "Sound Mapper" and "Primary Sound Driver" pseudo-devices that just mean "default", and deduplicates. **41 → 8.**

**Every entry has been measured, not assumed.** The obvious approach is to pick the host API with the nicest names — WASAPI on Windows, which in shared mode **doesn't resample**, so with 16 kHz in and 24 kHz out against 48 kHz hardware every open failed. Adding a rate check and moving to DirectSound passes that test on both sides, and PortAudio's DirectSound **output is a silent sink**: the stream opens, every write returns success in ~0 ms, and not one sample reaches the speakers.

| | write(2.0 s) took | |
|---|---|---|
| MME | **2.02 s** | consumed in real time |
| DirectSound | **0.00 s** | swallowed instantly |

No capability flag reports that. So the app measures it — once per host API per direction, on a background thread at startup, using silence. Two consequences worth stating plainly:

* **Each direction picks its own host API.** On Windows this lands on DirectSound for the microphone and MME for the speakers — a split no amount of reasoning would have produced.
* **The probe runs in the mode the app actually ships.** DirectSound input passes a callback stream and fails a blocking read; probing the wrong mode rejected a microphone that works perfectly.

Your choice is stored **by name, not by index** — indices shift whenever something is plugged in. If the saved device is gone, it falls back to the system default and says so in the log rather than failing to start.

### 🔗 It stops forgetting the conversation when the connection drops

`session_resumption` was switched on in the config and the handle the server sent back was **never read** — so every reconnect started an empty session. A dropped packet, or simply changing the voice, wiped the conversation. "Unlimited sessions" leaked through exactly this hole.

The handle is captured and replayed now. A network blip, or switching your microphone, keeps the conversation intact.

It is held in memory only, deliberately: writing it to disk would make a fresh launch continue yesterday's chat, which sounds appealing but breaks the session-summary flow — a conversation that never ends never produces a summary, and the "yesterday we talked about…" line in the morning briefing silently disappears. Changing the **voice** also starts clean on purpose, since resuming restores the server's session state and would likely bring the old voice back with it.

### 🩹 Fixes that came with it

* **The assistant could die on a log line.** Status lines carry emoji and arrows (`📤 file_controller → Moved: a.txt → Documents/`). On a non-UTF-8 console — cp1254 on a Turkish Windows, cp1251 on a Russian one, cp932 on a Japanese one — printing one raises `UnicodeEncodeError`, and because that print sits *after* the tool's own `try/except`, it escaped into the receive loop and took the session down.
* **Every computer command paid for two model round trips.** `computer_settings` made an *entire second Gemini call, inside the tool*, purely to translate the request into one of its own action names — because the declaration only said "The action to perform", so the model rarely filled it in. When that second call failed, the fallback was `description.lower().replace(" ", "_")`, which turns the Turkish for "turn it down" into `sesi_kis` and straight into "Unknown action". The declaration now names all 56 actions and the rest is spelling tolerance handled locally by `difflib` in microseconds. When nothing matches it suggests real action names instead of dead-ending.
* An unresolvable saved audio device, or one the driver refuses to open, falls back to the system default and says so — on both the microphone and the speakers.
* A rejected session-resumption handle is dropped after one attempt, so an expired handle can never be replayed on every retry and prevent the reconnect it exists to protect.



---

## 🗺️ Mark Roadmap

| Mark | Focus |
|---|---|
| **XOIX** | Auto-start · clipboard intelligence · assistant customization |
| **O** | Session memory · background monitoring · proactive 2.0 · instant vision |
| **OI** | Plugin system · affective dialog · proactive audio · unlimited sessions |
| **OII** | Voice picker · live theming · reactive HUD · recallable memory · undo · real confirmation · audio device picker · session continuity |
| **OIII** | Wake word · Gemini 3.1 Flash Live · instant acknowledgment · self-describing action/plugin architecture |
| **OIV** | Holographic avatar · viseme lip-sync · facial acting · face-as-status · push-to-talk · self-echo guard · runtime self-knowledge & limits |
| *shared* | The last five above also shipped to LIII, LIV and LV at the same time — moving up a Mark never loses them |
| **OV+** | Interrupt by voice · conversation history · plugin files: email · quiz mode · calendar · home assistant · 3D-printer |

---

## ⚡ Quick Start

```bash
git clone https://github.com/ShayanMitra/ORION-main
cd ORION
python setup.py        # installs deps for YOUR OS + the browser automation engine
python main.py
```

`setup.py` only ever installs what your operating system needs — the Windows-only libraries are skipped automatically on macOS and Linux, and vice-versa. It also checks your Python version up front, so a wrong interpreter fails with a sentence instead of a wall of pip output. Prefer to do it by hand? `pip install -r requirements.txt` works too.

> ⚠️ **Installation Note:** If you hit a `ModuleNotFoundError` for an OS-specific package, install it with `pip install <module_name>`. The optional **wake word** engine is *not* installed here — grab it in one click from **⚙ → WAKE WORD** inside the app.

---

## 📋 Requirements

| Requirement | Details |
| --- | --- |
| **OS** | Windows 10/11, macOS, or Linux |
| **Python** | 3.11, 3.12 or 3.13 |
| **Microphone** | Required for voice interaction (and for the "Hey Jarvis" wake word) |
| **Speakers** | Required for voice replies |
| **API Key** | Free Gemini API key (entered on first launch → `config/api_keys.json`) |
| **GPU** | **Not required.** The avatar is rendered in software |
| **Wake word** *(optional)* | One-click download from ⚙ → WAKE WORD (`openwakeword`, a few MB, fully local) |

---

## 🗂️ Project Structure

```
ORION/
├── main.py                   # Core loop — Gemini Live session, audio I/O, viseme extraction, tool dispatch
├── ui.py                     # PyQt6 HUD — avatar canvas, waveform, log panel, settings drawer, camera feed
├── setup.py                  # OS-aware installer (skips wrong-OS dependencies, checks your Python)
├── .gitignore                # Keeps your API key, TLS key and memories out of the repository
├── plugins/
│   ├── quiz.py               # Interactive quiz — ATLAS writes the questions, you answer on screen
│   ├── document_review.py    # Contracts and policies in plain language, ordered by what matters
│   ├── _google_core.py       # Shared OAuth for the Gmail/Calendar plugins (not a plugin itself)
│   ├── _printer_core.py      # Shared printer connectivity (not a plugin itself)
│   ├── _template.py          # Copy this to write a new plugin — one file, drop in, done
│   └── ...                   # Drop-in skills (each self-describes via a PLUGIN dict + run())
├── actions/                  # Bundled skills — each self-describes via a TOOL dict + handler
│   ├── web_search.py         # Gemini + DDG parallel search (news, research, price, compare)
│   ├── screen_processor.py   # Screen & webcam capture for vision
│   ├── background_monitor.py # User-configured topic watching — daily DDG check
│   ├── proactive.py          # Proactive 2.0 — time/context/rotation-aware check-ins
│   ├── reminder.py           # OS-native scheduled notifications
│   ├── system_monitor.py     # CPU / RAM / GPU / temperature telemetry
│   ├── computer_settings.py  # Volume, brightness, WiFi, power (per-OS)
│   ├── computer_control.py   # Keyboard shortcuts, mouse, window management
│   ├── open_app.py           # Application launcher (per-OS name map)
│   ├── browser_control.py    # Web browser control
│   ├── file_controller.py    # File system operations
│   ├── file_processor.py     # Document reading and summarization
│   ├── send_message.py       # Messaging integration
│   ├── weather_report.py     # Live weather data
│   ├── flight_finder.py      # Flight search
│   ├── youtube_video.py      # YouTube playback control
│   ├── game_updater.py       # Game update management (Steam / Epic)
│   ├── code_helper.py        # Code review and generation
│   ├── dev_agent.py          # Developer task agent
│   └── desktop.py            # Desktop and taskbar control
├── memory/
│   ├── memory_manager.py     # Load/save long_term.json — sessions, monitors, identity
│   ├── config_manager.py     # api_keys.json access — key, OS, name, voice, colour, toggles
│   └── long_term.json        # Persistent store — created on first run
├── core/
│   ├── prompt.txt            # All prompt wording — {tokens} are filled from the live system at startup
│   ├── avatar.py             # Avatar renderer — lighting, pose, expression, mouth (QPainter)
│   ├── avatar_mesh.py        # Head geometry — loads the face, generates skull/neck/rigs
│   ├── face_model.obj        # The face itself (MediaPipe canonical model, Apache-2.0, 25 KB)
│   ├── viseme.py             # Transcript → mouth shapes, fused with the audio's timing
│   ├── echo.py               # Tells your voice from the assistant's own echo; self-calibrating
│   ├── hotkey.py             # Push-to-talk chord — global on Windows, windowed fallback elsewhere
│   ├── undo.py               # One shared undo stack — actions register how to reverse themselves
│   ├── confirm.py            # Irreversible-action gate — the token is issued by the UI, not the model
│   ├── audio_devices.py      # Microphone / speaker list — filtered, measured, resolved by name
│   ├── plugin_loader.py      # Plugin engine — discovery, validation, crash isolation
│   ├── action_loader.py      # Bundled-action engine — the built-in twin of plugin_loader
│   └── wake_word.py          # Local "Hey Atlas" detector — own thread, offline, opt-in
└── config/
    ├── api_keys.json         # API key, name, voice, colour, toggles — created on first launch (git-ignored)
    └── certs/                # Self-signed TLS pair for the phone dashboard — generated locally (git-ignored)
```


---

## 🔒 Your Data

Everything stays on your machine. There is no MARK server, no telemetry and no account.

| What | Where | Notes |
|---|---|---|
| Gemini API key, plugin credentials | `config/api_keys.json` | **Plaintext.** Anyone with your user account can read it. Treat it like a password file. |
| Dashboard TLS certificate + private key | `config/certs/` | Generated locally, self-signed, never leaves the machine. |
| What the assistant remembers about you | `memory/long_term.json` | Delete the file to make it forget everything. |

All three are listed in `.gitignore`, so a fork or a pull request cannot leak them by accident. **If you have already committed `config/api_keys.json` anywhere public, revoke that key** at [aistudio.google.com](https://aistudio.google.com/app/apikey) and generate a new one — removing the file in a later commit does not remove it from the history.

Your voice is streamed to Google's Gemini Live API while a session is open; that is the one thing that leaves your computer, and it stops when you mute or close the app.

---

## ⚠️ License

Personal and non-commercial use only.
Licensed under **[Creative Commons BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)**.

---

## 👤 Connect with the Creator

Engineered by a developer building a real-world ATLAS-style assistant.
⭐ **Star the repository to support the journey to Mark 100.**

| Platform | Link |
| --- | --- |
| LinkedIn | [@ShayanMitra](https://www.linkedin.com/in/shayan-mitra-31929937a) |
| Instagram | [@ShayanMitra](https://www.instagram.com/bong.mitra_07/) |
