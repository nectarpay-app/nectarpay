# 🍯 NectarPay Pro (v2.0.1)

Welcome to NectarPay Pro – a sleek, high-performance desktop wallet and payment management application designed to streamline digital asset handling, coordinate multi-method global transfers, and maintain synchronized transaction tracking. Built with a responsive, modern glassmorphic web interface, NectarPay Pro provides an integrated financial hub straight to your local operating system.

---

## 🚀 Tech Stack

NectarPay Pro is built using **HiveFramework**, a specialized framework that compiles native C++ asset-routing pipelines into highly fluid, hardware-accelerated desktop web views. 

*   **Frontend:** HTML5, CSS3 (Custom Glassmorphism engine), and HiveFX.js
*   **Database:** HiveDB (A secure, locally encrypted, append-only ledger)
*   **Core:** Node.js desktop wrapper

---

## 🛠️ Installation & Setup

Getting started is simple. You do not need any complex runtimes or global environments.

1. Download the latest `NectarPay_Pro_Setup.exe` (Windows) or `NectarPay_Pro.dmg` (macOS) from the releases page.
2. Run the installer and follow the on-screen prompts.
3. Launch the application from your desktop or applications folder.

---

## 📜 Version History & Updates

### v0.1.0 (Alpha)
*   Initial proof-of-concept release.
*   Added basic wallet UI layout with a crude yellow gradient background.
*   Added support for creating localized mock wallets.
*   Fixed a major memory leak caused by spamming the "Refresh Balance" button.
*   Fixed application crashes occurring when the host computer was set to specific time zones.

### v0.5.0 (Beta)
*   First public beta release with the completed glassmorphic dashboard interface.
*   Added integration with testnet APIs for multi-asset tracking.
*   Moved local wallet data out of plain text files into encrypted HiveDB files.
*   Optimized background syncing loops, reducing idle CPU usage from 45% down to 4%.

### v1.0.0
*   First official stable production release.
*   Added P2P local ledger synchronization across devices on the same local network.
*   Added multi-method global transfer queues (simultaneous bank wires and digital asset transfers).
*   Complete UI overhaul with dynamic lighting that shifts based on system time.
*   Dropped support for legacy 32-bit operating systems to ensure security compliance.

### v2.0.0
*   Major architectural rewrite to separate the UI thread from payment processing.
*   Added automated currency conversion pathways to automatically find the lowest global fees.
*   Added automated recurring transaction rules.
*   Fixed a bug where rapidly changing asset values caused the dashboard UI elements to shake or vibrate on-screen.
*   Upgraded HiveDB engine to support fast zero-knowledge cryptographic verification.

### v2.0.1 (Current)
*   Fixed an issue where local network synchronization would freeze if a peer device disconnected unexpectedly mid-transfer.
*   Optimized GPU memory footprint for glassmorphic blur rendering by 35% on macOS systems.
*   Improved contrast ratios on text elements to meet accessibility standards.
