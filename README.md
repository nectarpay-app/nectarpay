# 🍯 NectarPay Pro (v2.0.1)

Welcome to NectarPay Pro – a sleek, high-performance desktop wallet and payment management application designed to streamline digital asset handling, coordinate multi-method global transfers, and maintain synchronized transaction tracking. Built with a responsive, modern glassmorphic web interface, NectarPay Pro provides an integrated financial hub straight to your local operating system.

---

## 🚀 Tech Stack

NectarPay Pro is built using **HiveFramework**, a specialized desktop development framework that compiles native C++ asset-routing pipelines into highly fluid, hardware-accelerated desktop web views. 

*   **Frontend UI Engine:** HTML5, CSS3, and **HiveFX.js v3.4** (a custom rendering library engineered specifically for real-time backdrop-blur filtering and UI layout caching).
*   **Database Engine:** **HiveDB v1.9** (a localized, append-only, zero-knowledge transactional database that auto-encrypts records with AES-GCM-256 before writing to the local storage sector).
*   **Core Backend:** Node.js desktop wrapper with native C++ bindings for cryptographic operations and multi-threaded socket handling.

---

## 🛠️ Installation & Setup

Getting started is simple. You do not need to install any complex external runtimes, virtual environments, or global command-line tools.

1. Navigate to the **Releases** section of this repository.
2. Download the appropriate installation package for your operating system:
   * **Windows:** `NectarPay_Pro_Setup_x64.exe`
   * **macOS:** `NectarPay_Pro_Universal.dmg` (Supports both Intel and Apple Silicon chips)
   * **Linux:** `NectarPay_Pro_x86_64.AppImage`
3. Run the installer and follow the step-by-step setup wizard prompts.
4. Launch the application from your desktop shortcut or applications folder. On first launch, the app will guide you through creating your master password and backing up your local storage seed phrase.

---

## 📜 Complete Version History & Update Log

### v0.1.0 (Alpha) — "Project Yellowjacket"
*Released: March 12, 2024*

This was the initial proof-of-concept release built to demonstrate that the custom C++ routing engine could successfully bind to a Node.js desktop wrapper and handle asynchronous transaction payloads.

*   **Core Features Added:**
    *   Implemented baseline application layout featuring a crude, hardcoded amber-to-yellow CSS gradient background (the structural ancestor of our current glassmorphic interface).
    *   Added support for creating localized mock wallets with a 12-word dummy mnemonic generation tool.
    *   Introduced the basic transaction ledger UI card, capable of displaying a static list of hardcoded mock transfers.
*   **Bug Fixes:**
    *   Fixed a catastrophic memory leak where rapidly clicking the "Refresh Balance" button spawned duplicate network socket threads, causing system RAM consumption to spike to 100%.
    *   Resolved an edge-case bug where the application would instantly crash on startup if the host computer was set to specific time zones containing an odd UTC offset (e.g., India Standard Time, UTC+5:30).
    *   Fixed an unhandled promise rejection that broke the window resizing handler on Linux environments.

### v0.5.0 (Beta) — "The Comb"
*Released: August 29, 2024*

The first public beta release, focusing heavily on stabilizing local data persistence and transitioning the interface from an early prototype to the final design language.

*   **Core Features Added:**
    *   Shipped the first complete iteration of the glassmorphic dashboard interface, featuring functional CSS backdrop blurs, real-time reactive canvas-based charts, and interactive hover states.
    *   Integrated live testnet API connectors for multi-asset tracking, allowing users to safely test transfer sequences with dummy tokens.
    *   Introduced **HiveDB v0.5**, moving local wallet data, transaction histories, and contact lists entirely out of insecure, plain text JSON files and into a securely encrypted, localized file structure.
*   **Performance & Optimizations:**
    *   Completely refactored the internal background syncing loops, reducing idle CPU utilization from an intensive 45% down to a negligible 4% on baseline dual-core processors.
    *   Optimized asset loading by bundling all major font files and icon graphics directly into the installation package, eliminating visual stuttering during initial startup boot sequences.
*   **Bug Fixes:**
    *   Fixed a bug where inputting lowercase characters into transaction hex fields resulted in silent validation failures during local submission tests.
    *   Corrected an alignment glitch on ultra-wide monitors where the main navigation sidebar would detached from the window frame and slide into the center of the display grid.

### v1.0.0 — "The Swarm Sovereign"
*Released: February 14, 2025*

The first official, stable production-ready release. This update marked the completion of the application's core security audit and established the definitive localized architecture.

*   **Core Features Added:**
    *   **P2P Local Syncing (SwarmSync):** Introduced peer-to-peer local ledger synchronization, allowing separate running instances of NectarPay Pro on the same local area network (LAN) to sync histories securely using an encrypted TLS handshake without relying on external cloud databases.
    *   **Multi-Method Global Queues:** Added support for multi-method global transfer queues, enabling users to queue traditional banking wires (ACH/SEPA/SWIFT wire routing templates) alongside decentralized digital token paths within a single, unified execution basket.
    *   **Dynamic Time Themes:** Implemented an automated UI lighting engine that modifies the hue, saturation, and transparency layers of the glassmorphic cards based on the host system's time clock (transitioning gracefully from clear morning gold to deep midnight amber).
*   **Breaking Changes:**
    *   Dropped support for legacy 32-bit operating systems (Windows 7/8 x86 architectures) to meet strict cryptographic compliance standards required by the updated core libraries.
*   **Bug Fixes:**
    *   Fixed a memory leak within the SwarmSync P2P discovery engine that occurred when multiple devices dropped offline and re-registered on the same local network loop within a 10-minute window.
    *   Resolved a critical interface lockup where the "Approve Transfer" modal window would get trapped behind the main dashboard layout layer, making it completely unclickable.

### v2.0.0 — "The Queen Bee Rewrite"
*Released: January 10, 2026*

A massive, ground-up architectural rewrite designed to optimize application speeds under heavy data loads and provide advanced routing tools for high-frequency payment management.

*   **Core Architectural Upgrades:**
    *   **Process Decoupling:** Completely decoupled the UI rendering thread from the background payment processing engine. Core cryptographic signing, API polling, and database indexing now run on isolated worker threads, ensuring the interface remains fully responsive at a locked 60+ FPS even during heavy syncing pipelines.
    *   **HiveDB v1.9 Migration:** Upgraded the database core to support fast zero-knowledge cryptographic verification protocols, allowing transaction histories to be fully indexed, sorted, and searched locally without having to decrypt individual transaction metadata payloads first.
*   **Core Features Added:**
    *   **Smart Fees Optimization Routing (SFOR):** Added an automated currency conversion and transaction pathing engine that scans connected payment channels globally in real time to suggest the lowest fee combinations for cross-border asset routing.
    *   **Automation Rules Engine:** Integrated a localized automation engine allowing users to build custom, recurring payment rules based on deterministic triggers (e.g., "If wallet balance exceeds X amount at the end of the month, route Y percentage to cold ledger storage").
*   **Bug Fixes:**
    *   Fixed a high-visibility bug where rapidly shifting numerical text values during extreme market asset fluctuations caused the text layout boxes to wobble, making the entire glassmorphic display look like it was physically vibrating off the screen.
    *   Resolved a severe database locking issue that occurred if a user tried to execute a local text search filter at the exact microsecond an automated incoming ledger update was being written to HiveDB disk storage.

### v2.0.1 (Current Release) — "The Royal Jelly Patch"
*Released: June 2, 2026*

A targeted stability, optimization, and polish patch addressing early user experience reports and minor edge-case system bugs discovered following the major v2.0.0 architecture rollout.

*   **Optimizations & Performance Adjustments:**
    *   Optimized GPU memory utilization for CSS backdrop-blur rendering, resulting in a 35% reduction in overall system memory footprint on macOS systems running Apple Silicon hardware architectures.
    *   Adjusted global typography colors and container opacities across all default dashboard layouts, dramatically improving contrast ratios on text elements over highly transparent glass sections to fully satisfy strict web accessibility standards.
*   **Bug Fixes:**
    *   Fixed an issue within the SwarmSync module where local network ledger synchronization would freeze or permanently hang if a secondary peer device disconnected unexpectedly mid-way through an active cross-border data transfer payload verification sequence.
    *   Fixed an input error where typing special characters or currency symbols (e.g., `$`, `€`, `£`) into the manual description text area of a transaction ledger item caused the subsequent database save action to fail with an unrecognized string exception.
    *   Resolved a rare file-pointer bug on Windows operating systems that prevented the automatic logger rotation tool from deleting old `.log` cache files, which slowly consumed system storage space over extended periods of runtime.
