# DPRO Control 1.2.1 — Independent Edition

Created by Loud and Beyond to keep the NA2-IO-DPRO useful with a maintainable, native Apple Silicon controller.

- Two-channel input/output control with verified readback.
- Mic/Line labels, Line-only PAD, Mic-only gain/phantom UI availability.
- Output attenuation displayed in dB with half-dB steps.
- Input/output linking with synchronization and mirrored changes.
- Four live dBFS meters with stale/offline handling.
- Adapter-based Bonjour discovery and automatic IP fill.
- Separate Device status view for feedback and session activity.
- Cleaner overview with the device name and no output explanation block.
- Native AppKit/WKWebView host with bundled Python, automatic localhost port and parent-exit cleanup.
- Built app distribution; copyright Loud and Beyond, with project and runtime notices included.

Apple Silicon only. macOS 15 deployment target; tested on macOS 26.5.2. This release is ad-hoc signed, not Developer ID signed or notarized. Other models and future OS versions are not validated. PAD writes/linking were validated offline against captured commands; live PAD checks read hardware state without changing it.

This release distributes the app ZIP and its checksum only. The separately uploaded source archive has been removed.
