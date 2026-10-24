# Awesome-Web-Conferencing-Virtual-Classroom

# Awesome-Web-Conferencing-Virtual-Classroom

# Top Web Conferencing & Virtual Classroom Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Self-Hosted Pedagogy Tools, WebRTC Scalability & LMS Integration*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Web Conferencing & Virtual Classroom**. These tools handle real-time audio, video, screen sharing, and the teaching-specific features that separate a lecture from a meeting — whiteboards, breakout rooms, polls, and learning analytics — with a spectrum running from polished commercial suites to self-hosted platforms where you control the data and the pedagogy.

**Examples** include Jitsi Meet, BigBlueButton, Galène, OpenMeetings, and EduMeet (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, classroom-specific tooling, and transparent resource requirements — ideal for schools and organizations that need data sovereignty and teaching features without per-seat SaaS fees.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **Zoom Meetings** — **The ubiquitous commercial standard.** Reliable video, breakout rooms, whiteboard, and broad ecosystem integrations. **Free tier** with 40-minute group call limits; paid plans per-host. **Trade-offs**: cloud-only, privacy concerns around data routing, and the 40-minute cap on free group calls. **Best for teams wanting the most frictionless commercial experience** and accepting vendor dependency.

- **Microsoft Teams** — **The Microsoft 365 collaboration hub.** Deep integration with Office apps, calendar, and organizational identity. **Included with many Microsoft 365 plans**. **Best for Microsoft-centric organizations** already standardized on the ecosystem.

- **Google Meet** — **The Google Workspace video standard.** Browser-based, no install required, with recording and live captions on paid Workspace tiers. **Best for Google Workspace organizations** wanting native calendar and Drive integration.

- **Cisco Webex** — **The enterprise conferencing veteran.** Strong security controls, large meeting support, and deep integration with Cisco infrastructure. **Best for large enterprises** with existing Cisco investments.

## Open-Source GitHub Projects

- **Jitsi Meet** — **The general-purpose self-hosted video conferencing standard.** Apache-2.0 licensed, **30,100+ GitHub stars** [citation:1][citation:12]. **No account required for participants** — anyone with the link joins directly in the browser [citation:1]. **Deploys in ~10 minutes via official Docker Compose** with four containers (web, Prosody XMPP, Jicofo, JVB) [citation:1][citation:5]. **Runs on 4 GB RAM minimum, 8 GB recommended** — significantly lighter than classroom-specific alternatives [citation:1]. **Supports screen sharing, chat, reactions, virtual backgrounds, lobby mode, and end-to-end encryption** via Insertable Streams [citation:1][citation:6]. **Recording and RTMP streaming via Jibri** on a separate server component [citation:1][citation:6]. **Iframe and JavaScript API** for embedding into your own product [citation:1]. **The honest limitation**: **no native whiteboard or built-in classroom structure** — Excalidraw integration fills the whiteboard gap, but it's not a teaching-first platform [citation:1]. **Best for general meetings and team standups** where lightweight deployment and no-account access matter more than pedagogy tools.

- **BigBlueButton** — **The virtual classroom standard built for teaching.** LGPL-3.0 licensed, **9,200+ GitHub stars** [citation:1][citation:12]. **Pedagogy-first design** with **multi-user whiteboard**, **breakout rooms with timers**, **shared notes**, **polls and quizzes**, **presentation upload with slide-by-slide navigation**, and **built-in recording** with searchable playback [citation:1][citation:7]. **Native LMS integration** with Moodle, Canvas, Sakai, and others via LTI [citation:1]. **The resource reality**: **16 GB RAM and 8 CPU cores recommended for production**, with 10+ services and installation via `bbb-install.sh` (no official lightweight Docker Compose) [citation:1][citation:3][citation:12]. **Scalability**: a single node handles roughly 200 concurrent users before needing Scalelite load balancer [citation:3]. **The honest limitation**: **overkill for simple two-person calls** — the classroom depth comes with operational weight [citation:1]. **Best for schools, universities, and training programs** where teaching features justify the heavier footprint.

- **Galène** — **The minimalist Go-based video conferencing server.** **Single Go binary with no external dependencies** — no database, no message queue, no application server [citation:7]. **Uses WebRTC with Pion** (pure-Go implementation) for extreme resource efficiency — **~50 MB RAM at idle**, **0.25 CPU cores can handle a 100-student lecture** [citation:1][citation:7]. **Group-based room system configured via JSON files** with access tokens — highly scriptable but less user-friendly for non-technical admins [citation:7]. **Built-in TURN server** and a self-contained web client [citation:11]. **The honest limitation**: **pure video/audio only** — no whiteboard, no classroom tools, no built-in recording without plugins [citation:1][citation:7]. **Best for technical teams** wanting a fast, reliable, minimal-footprint conferencing server for developer standups or hackathons.

- **Apache OpenMeetings** — **The Apache-governed virtual classroom suite.** **Java-based**, with **whiteboard, document sharing (PDF, Office, images), screen sharing, session recording, polls, quizzes, and calendar scheduling** [citation:7]. **Integrates with LDAP, OAuth, and CalDAV** for institutional authentication and scheduling [citation:7]. **REST APIs** for LMS integration [citation:7]. **The trade-off**: **Java backend requires 4 GB RAM minimum** and is heavier than Galène or EduMeet [citation:7]. **Best for institutions** wanting a comprehensive Apache-licensed classroom platform with mature governance.

- **EduMeet** — **The modern WebRTC virtual classroom built on mediasoup.** **Low-latency, high-quality video** without the overhead of a traditional application server [citation:7]. **Handles 50-200 participants per room** via mediasoup's efficient SFU architecture [citation:7]. **The honest limitation**: **no whiteboard, quizzes, or file sharing out of the box** — pairs well with a separate LMS [citation:7]. **Best for organizations already using Moodle/Canvas** that need a reliable video component without classroom tooling.

### Additional Strong Open-Source Options

- **plugNmeet** — Scalable high-performance web conferencing system. MIT licensed, Go-based, with a powerful AI Meeting Agent [citation:14]. Best for teams wanting a modern Go alternative to Jitsi with built-in recording.
- **MiroTalk SFU** — Simple, secure, scalable WebRTC conferencing up to 4K. AGPL-3.0 licensed [citation:9]. Best for teams wanting a lightweight browser-based conferencing tool with screen sharing.
- **VibeMeeting** — Self-hostable web meeting system with audio/video, screen sharing, chat, host controls, and MP4 recording. Built on Django, Flutter Web, and LiveKit, Apache-2.0 licensed [citation:4]. Best for Django developers wanting a self-hosted meeting stack.

**Frameworks for building custom systems**: Combine **Jitsi Meet** for lightweight general-purpose meetings with Docker-native deployment and no-account access, **BigBlueButton** for teaching-first virtual classrooms with whiteboard, breakout rooms, and LMS integration, **OpenMeetings** for Apache-governed classroom tooling with LDAP/OAuth, and **Galène** for minimal-footprint video-only conferencing — to build a conferencing stack tailored to your teaching requirements, resource constraints, and administrative capacity.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Web conferencing tools differ significantly in classroom depth, resource requirements, and deployment complexity. **Jitsi Meet deploys in ~10 minutes via Docker** and runs on 4 GB RAM, but **lacks native whiteboard and classroom structure** [citation:1]. **BigBlueButton has the deepest teaching features** — whiteboard, polls, breakout rooms with timers, shared notes, built-in recording — but requires **16 GB RAM and 8 CPU cores recommended for production**, and has **no official lightweight Docker Compose** [citation:1][citation:3]. **Galène runs in ~50 MB RAM** and 0.25 CPU cores for 100 students, but is **video-only** — no whiteboard, no classroom tools [citation:1][citation:7]. **OpenMeetings requires 4 GB RAM** for its Java backend but offers Apache governance and LDAP/OAuth integration [citation:7]. **The choice often comes down to one question**: do you need teaching tools (BigBlueButton) or a reliable meeting room (Jitsi Meet)?
- Self-hosted open-source solutions require proper TURN/STUN server configuration for participants behind symmetric NATs, reverse proxy setup for SSL termination, and awareness that WebRTC media ports (UDP 10000 for Jitsi, UDP 16384-32768 for BigBlueButton) need firewall rules [citation:1][citation:11].

---

**Made for educators, IT administrators, and organizations choosing self-hosted conferencing that matches their teaching needs and infrastructure.**
Let's make web conferencing and virtual classrooms more open, pedagogy-aware, and self-hostable.
