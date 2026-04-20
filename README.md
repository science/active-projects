# Active Projects

A directory of my active personal projects -- web apps, tools, and utilities.

## Web Apps

### [WolfeChat](https://github.com/science/WolfeChat)
**Live:** [science.github.io/WolfeChat](https://science.github.io/WolfeChat/)

Browser-based multi-provider AI chat interface supporting OpenAI (GPT-5.2, GPT-4.1) and Anthropic (Claude Opus, Sonnet) models. Bring your own API keys, no subscription needed. Features streaming responses, reasoning windows, per-conversation settings, image uploads, and TTS.

*Svelte + TypeScript + Vite -- deployed to GitHub Pages*

---

### [AI Translator](https://github.com/science/ai-translator)
**Live:** [science.github.io/ai-translator](https://science.github.io/ai-translator/)

Convert and translate PDF files to markdown in any language using LLM technology. Upload a PDF, pick a target language, and get clean translated markdown output. Bring your own API keys, no subscription needed. 

*SvelteKit + TypeScript -- deployed to GitHub Pages*

---

### [Hot Tub Controller](https://github.com/science/HotTubController)
**Live:** [misuse.org/tub](https://misuse.org/tub)

Web-based automation system for intelligent hot tub temperature management and equipment control. Controls heater, pump, and ionizer remotely via a mobile-friendly interface with scheduling, temperature monitoring, and safety features. Uses IFTTT webhooks to control SmartLife/Tuya smart relays with an ESP32 temperature sensor.

*PHP backend + SvelteKit frontend + ESP32 firmware -- deployed to cPanel shared hosting*

---

### [Movie Night](https://github.com/science/movie-night)
**Live:** [misuse.org/dinner-and-a-movie](https://misuse.org/dinner-and-a-movie/)

*In progress.* A tool for planning movie nights with friends -- find a movie nobody has seen yet. Features a slot-machine randomizer for picking movies and a voting system.

*PHP backend + SvelteKit frontend -- deployed to cPanel shared hosting*

---

### [Google Docs Comments to Markdown](https://github.com/science/gdoc-comments-md)
**Live:** [science.github.io/gdoc-comments-md](https://science.github.io/gdoc-comments-md/)

Extract Google Docs comment threads and convert them to clean, readable markdown with inline anchors and threaded replies. Uses Google OAuth2 for browser-based auth with no backend required.

*SvelteKit + TypeScript + Tailwind -- deployed to GitHub Pages*

### [Recipe Measurements Converter](https://github.com/science/recipe-measurements-converter)
**Live:** [science.github.io/recipe-measurements-converter](https://science.github.io/recipe-measurements-converter/)

Standalone webapp that converts recipe volume and weight measurements to grams
using USDA food density data for 400 cooking ingredients. Features single-ingredient lookup
and a bulk recipe converter that uses AI to parse entire ingredient lists. No server required.

*SvelteKit + TypeScript + OpenAI embeddings -- static site*

---

### [Google Calendar Time Slot Generator](https://github.com/science/gcal-timeslot-generator)

Google Apps Script web app that reads your Google Calendar and generates copyable time-slot text for scheduling emails and messages. Scans the next N business days, computes free slots within working hours, supports multi-calendar merging, meeting fatigue breaks, timezone display, and two output formats (bullets or compact).

*TypeScript + Rollup + Google Apps Script + Jest*

---

## Linux Desktop

### [PDF Simple Signing](https://github.com/science/pdf-simple-signing)

Minimal desktop tool to stamp text and signature images onto PDFs without re-rendering the original layout. Features a full undo stack (add, delete, reposition, resize), per-image size memory, configurable date/name variables, and a dirty-flag save prompt. Writes directly to PDF content streams via PyMuPDF.

*Python3 + PyQt6 + PyMuPDF + pytest*

---

### [Multi-Row Panel Launchers](https://github.com/science/cinnamon-multirow-panellauncher)

Cinnamon applet that wraps panel launcher icons into multiple rows on tall panels. Forked from the stock panel-launchers applet. Supports 1–4 rows with auto-sizing, manual icon size override, max-width caps, overflow popup with chevron, and drag-and-drop reordering.

*GJS (Clutter/St) + Node.js tests*

---

### [Multi-Row Window List](https://github.com/science/cinnamon-multirow-windowlist)

Cinnamon applet that wraps window-list buttons into multiple rows on tall panels. Forked from the stock window-list applet. Features adaptive button sizing, app grouping, drag-and-drop reordering, hover thumbnails, middle-click close, and attention alerts.

*GJS (Clutter/St) + Node.js tests + VM E2E tests (libvirt/KVM)*

---

### [System Tray with Overflow](https://github.com/science/cinnamon-systray-overflow)

Unified system tray applet for Cinnamon 6.0+ that merges XEmbed and XApp status icons into a single applet with an overflow popup. Drag-and-drop promotion/demotion between visible and overflow sections, plus a system applet proxy.

*GJS (Clutter/St) + Node.js tests + VM E2E tests (SPICE/virtio-fs)*

---

### [Audio Switcher](https://github.com/science/audio-switcher)

PipeWire auto-routing and recovery daemon for Linux. Built for the Sennheiser BTD-800 USB Bluetooth dongle -- detects headset connection via HID reports, routes audio automatically, falls back to S/PDIF speakers on disconnect, and recovers PipeWire after crashes and sleep/resume cycles.

*Bash + systemd + PipeWire + udev*

---

### [PAM Fingerprint Sudo](https://github.com/science/pam-fprintd-sudo)

PAM module enabling fingerprint-authenticated sudo in non-TTY contexts like IDE terminals and Claude Code. Uses `pam_exec.so` to launch a GTK3 fingerprint popup instead of a terminal password prompt. Includes a `sudo -i` escape hatch for password fallback.

*Bash + Python3 (GTK3) + PAM + fprintd*

---

### [Anomalous Monitor](https://github.com/science/anomalous-mon)

Desktop anomaly monitor that detects sustained CPU hogging and OOM kills on Linux workstations. Uses dual-track state (PID + process name) to catch both stuck processes and crash-looping services. Alerts via desktop notifications after 5 consecutive high-CPU samples. Built after an rclone mount silently consumed 1.9GB RSS without alerting.

*Bash + systemd user timer + journalctl*

---

### [Mouse Tools](https://github.com/science/mouse-tools)

Mouse management daemon for Linux built on evdev. Handles button debounce (fixes phantom releases on worn mice during drags) and button-to-key remapping (e.g., side buttons to volume control). Includes movement diagnostics and drag monitoring.

*Python3 (evdev/uinput) + systemd + pytest*

---

### [stay-awake](https://github.com/science/stay-awake)

Temporarily inhibit system suspend for long-running overnight jobs. Thin, tested wrapper over `systemd-inhibit` with duration or command-wrapping modes. Respects the machine's xidlehook-based idle/lock config.

*Python3 + systemd-inhibit + pytest*

---

## Android

### [DateTime Widget](https://github.com/science/datetime-widget)

A simple Android 1x1 home screen widget that displays the current date (day of week + month + day). Font auto-scales to fill the widget. Solves the simple problem of seeing today's date at a glance.

*Kotlin + Android -- [download APK](https://github.com/science/datetime-widget/raw/main/downloads/datetime-widget.apk)*
